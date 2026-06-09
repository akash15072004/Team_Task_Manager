# 🚀 Team Task Manager (MERN Stack)

A full-stack **Team Task Management Web Application** where users can create projects, assign tasks, and track progress with role-based access control (Admin / Member).

---

## 🌐 Live Demo
  
* **Link:**  https://akash-team-task-manager-app.lumi.ing 

---

## 📌 Features

* 🔐 Authentication (Login / Signup with JWT)
* 👥 Role-Based Access (Admin / Member)
* 📁 Project Management
* ✅ Task Creation & Assignment
* 📊 Dashboard (Task status, overdue tasks)
* 🔔 Notifications system
* 🌙 Dark / Light Mode
* 🍪 Secure cookie-based authentication

---

## 🛠️ Tech Stack

### Frontend

* React.js (Vite)
* Redux Toolkit (RTK Query)
* Tailwind CSS

### Backend

* Node.js
* Express.js
* MongoDB (MongoDB Atlas)
* JWT Authentication

### Deployment

* Frontend → Lumi
* Backend → Render
* Database → MongoDB Atlas

---

## 📁 Project Structure

```
Team Task Manager
│
├── frontend/          # React + Vite
├── server/            # Node + Express
└── README.md
```

---

## ⚙️ Setup Instructions

### 🔹 Clone Repository

```bash
git clone https://github.com/your-username/team-task-manager.git
cd team-task-manager
```

---

### 🔹 Backend Setup

```bash
cd server
npm install
```

#### `.env`

```env
PORT=5000
MONGO_URI=your_mongodb_atlas_url
JWT_SECRET=your_secret_key
NODE_ENV=development
FRONTEND_URL=https://task-manager-6oklg4.lumi.ing/
```

```bash
npm start
```

---

### 🔹 Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## 🔗 API Configuration

### Production

```env
VITE_API_URL=https://team-task-manager-4q1s.onrender.com
```

---

## 🐞 Common Issues

### Failed to fetch

* Check API URL
* Check backend deployment
* Fix CORS

---

### MongoDB Error

* Use MongoDB Atlas (not localhost)

---

### Cookie Issue

```js
secure: true
sameSite: "none"
```

---

## 👨‍💻 Author

**Akash Chaudhary**
B.Tech IT | Full Stack Developer

---

## ⭐ License

MIT License
