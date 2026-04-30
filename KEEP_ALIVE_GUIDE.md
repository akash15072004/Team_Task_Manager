# 🔥 Keep Backend Alive Guide (Team Task Manager)

Your Render free tier backend spins down after 15 minutes of inactivity. Here are ways to keep it awake for your **Team Task Manager project**.

---

## 🌐 Project URLs

* **Frontend:** https://task-manager-6oklg4.lumi.ing/
* **Backend:** https://team-task-manager-4q1s.onrender.com

---

## 🧠 Problem

Render free tier:

* Sleeps after **15 minutes inactivity**
* First request takes **30–60 seconds (cold start)**

👉 Solution: Keep pinging backend regularly

---

# 🚀 Option 1: Browser Tab (Simple)

1. Create a file: `keep-alive.html`
2. Paste this:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Keep Backend Alive</title>
</head>
<body>
  <h2>Backend Keep Alive Running...</h2>

  <script>
    setInterval(() => {
      fetch("https://team-task-manager-4q1s.onrender.com/api/users/login")
        .then(() => console.log("Ping success"))
        .catch(() => console.log("Ping failed"));
    }, 10 * 60 * 1000); // every 10 min
  </script>
</body>
</html>
```

3. Open in browser
4. Keep tab open

---

# ⭐ Option 2: UptimeRobot (BEST - Recommended)

1. Go to: https://uptimerobot.com
2. Create free account

### Add Monitor:

* Type: HTTP(s)
* Name: Team Task Manager Backend
* URL:

```
https://team-task-manager-4q1s.onrender.com
```

* Interval: **5 minutes**

👉 Done! Backend will stay alive 24/7

---

# ⚡ Option 3: Cron-Job.org

1. Go to: https://cron-job.org
2. Add job:

```
URL: https://team-task-manager-4q1s.onrender.com
Time: Every 10 minutes
```

---

# 💻 Option 4: Node Script

Create file `keep-alive.js`

```js
setInterval(async () => {
  try {
    await fetch("https://team-task-manager-4q1s.onrender.com");
    console.log("Backend alive");
  } catch (err) {
    console.log("Error:", err.message);
  }
}, 10 * 60 * 1000);
```

Run:

```bash
node keep-alive.js
```

---

# 🔁 Option 5: GitHub Actions (Advanced)

Create:

```
.github/workflows/keep-alive.yml
```

```yaml
name: Keep Backend Alive

on:
  schedule:
    - cron: '*/10 * * * *'

jobs:
  ping:
    runs-on: ubuntu-latest
    steps:
      - name: Ping Backend
        run: curl -f https://team-task-manager-4q1s.onrender.com || exit 1
```

---

# ✅ Recommended Setup

| Use Case         | Best Option    |
| ---------------- | -------------- |
| Demo / Interview | Browser tab    |
| Production       | UptimeRobot    |
| Advanced Dev     | GitHub Actions |

---

# 📊 Backend Info

* **Backend URL:** https://team-task-manager-4q1s.onrender.com
* **Sleep Time:** 15 min
* **Cold Start:** 30–60 sec
* **Free Limit:** 750 hrs/month

---

# 🧪 Testing

1. Don’t use app for 20 min
2. Open frontend
3. If it loads instantly → working ✅
4. If delay → not working ❌

---

# 💡 Important Notes

* Always ping backend URL
* Avoid localhost ❌
* Use deployed URL only ✅
* Keep interval ≤ 10 min

---

# 🚀 Quick Start

👉 Fastest method:

1. Go to https://uptimerobot.com
2. Add URL:

```
https://team-task-manager-4q1s.onrender.com
```

3. Done 🎉

---

Happy Coding 🚀
