# 🚀 Team Task Manager - Full Stack Project

**Developed by:** Akash Chaudhary
**Project Type:** Full Stack Web Application (MERN Stack)
**Year:** 2026

---

## 🔗 Live Deployment

* **Frontend:** https://task-manager-6oklg4.lumi.ing/
* **Backend API:** https://team-task-manager-4q1s.onrender.com

---

## 🎯 What I Built

A full-stack **Team Task Management System** that allows teams to collaborate efficiently by creating projects, assigning tasks, tracking progress, and managing workflows.

This application solves real-world team productivity problems by providing structured task management with role-based access control.

---

## 🔥 Core Features

### 1. Authentication System

* User Signup & Login
* JWT-based authentication
* Secure HTTP-only cookies
* Protected routes

---

### 2. Role-Based Access Control

* **Admin**

  * Manage users
  * Assign tasks
  * View team performance
* **Member**

  * View assigned tasks
  * Update task status

---

### 3. Task Management System

* Create tasks with:

  * Title
  * Description
  * Priority
  * Deadline
* Assign tasks to users
* Track task progress:

  * Pending
  * In Progress
  * Completed

---

### 4. Dashboard & Analytics

* Task status overview
* Progress tracking
* Overdue task monitoring
* Team performance insights

---

### 5. Notification System

* Task assignment alerts
* Status update notifications
* Real-time feedback

---

### 6. UI/UX Enhancements

* Dark/Light theme toggle
* Responsive design
* Smooth animations
* Clean modern UI

---

## 🧠 Key Technical Decisions

### 1. MERN Stack Selection

* **MongoDB:** Flexible schema for tasks & users
* **Express.js:** Lightweight backend framework
* **React:** Component-based UI
* **Node.js:** Scalable server runtime

---

### 2. JWT Authentication

* Stateless authentication
* Secure token handling
* Cookie-based session management

---

### 3. Redux Toolkit (RTK Query)

* Efficient API handling
* Caching & state management
* Reduced boilerplate

---

### 4. Deployment Strategy

* Frontend → Lumi
* Backend → Render
* Database → MongoDB Atlas

---

## 🛠️ Tech Stack

### Frontend

* React.js (Vite)
* Redux Toolkit (RTK Query)
* Tailwind CSS

### Backend

* Node.js
* Express.js

### Database

* MongoDB Atlas

### Deployment

* Lumi (Frontend)
* Render (Backend)

---

## 📁 Project Structure

Team Task Manager
│
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── redux/
│   └── utils/
│
├── server/
│   ├── controllers/
│   ├── routes/
│   ├── middleware/
│   ├── models/
│   └── utils/
│
└── README.txt

---

## ⚙️ Setup Instructions

### 1. Clone Repository

git clone https://github.com/your-username/team-task-manager.git
cd team-task-manager

---

### 2. Backend Setup

cd server
npm install

Create `.env` file:

PORT=5000
MONGO_URI=your_mongodb_atlas_url
JWT_SECRET=your_secret_key
NODE_ENV=development
FRONTEND_URL=http://localhost:3000

Run backend:

npm start

---

### 3. Frontend Setup

cd frontend
npm install
npm run dev

---

## 🔐 Authentication Flow

1. User logs in or registers
2. Backend generates JWT token
3. Token stored in HTTP-only cookie
4. Protected routes verified via middleware

---

## 🌍 Deployment Details

### Backend (Render)

* Uses MongoDB Atlas
* CORS configured for frontend
* Environment variables set

### Frontend (Lumi)

* Connected with backend API
* Environment variable configured

---

## 🐞 Common Issues & Fixes

### Failed to fetch

* Check API base URL
* Ensure backend is deployed
* Fix CORS

---

### MongoDB Error

* Use MongoDB Atlas
* Allow network access (0.0.0.0/0)

---

### Cookie Issues

secure: true
sameSite: none

---

## 🚀 Future Improvements

* Real-time updates (WebSockets)
* File attachments in tasks
* Email notifications
* Mobile app version
* Advanced analytics dashboard

---

## 📊 Project Highlights

* Full-stack MERN application
* Real-world team collaboration system
* Secure authentication implementation
* Clean and responsive UI
* Deployed and production-ready

---

## 👨‍💻 Author

Akash Chaudhary
B.Tech Information Technology
Full Stack Developer

---

## 📜 License

MIT License

---

## 🎤 Interview Summary (Use This)

"I built a full-stack Team Task Manager using MERN stack. It includes authentication, role-based access, task assignment, and a dashboard for tracking progress. I deployed it using Render and Lumi, and used MongoDB Atlas for scalable database management."

---

**Thank you! 🚀**
