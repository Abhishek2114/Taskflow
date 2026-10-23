# 🚀 TaskFlow — Production Ready Team Task Manager

<p align="center">
  <img src="https://img.shields.io/badge/Frontend-Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white" />
  <img src="https://img.shields.io/badge/Backend-Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white" />
  <img src="https://img.shields.io/badge/Database-MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/Auth-JWT-black?style=for-the-badge" />
  <img src="https://img.shields.io/badge/UI-TailwindCSS-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/Architecture-FullStack-blue?style=for-the-badge" />
</p>

<p align="center">
  <b>Plan • Collaborate • Track • Deliver</b>
</p>

---

## 🌐 Live Demo

* **Frontend:** https://task-flow-sh.netlify.app/
* **Backend API:** https://task-flow-sh.up.railway.app/api/

---

## 📌 Overview

**TaskFlow** is a production-ready SaaS-style team task management platform built to simulate real-world product development.

It enables teams to:

* Plan work using projects
* Assign ownership
* Track progress
* Monitor productivity
* Deliver efficiently

Inspired by modern tools like **Linear, Notion, and Jira**, TaskFlow focuses on simplicity, performance, and usability.

---

## ✨ Features

### 🔐 Authentication & Security

* JWT-based authentication
* Secure login & signup
* Password hashing using bcrypt
* Protected API routes

---

### 👥 Role-Based Access Control

* **Admin**

  * Full access to projects, tasks, and members
* **Member**

  * View assigned projects
  * Update task status

---

### 📁 Project Management

* Create and manage projects
* Add members to projects
* View project details
* Track project progress (based on completed tasks)

---

### 📝 Task Management

* Create, assign, update, and delete tasks
* Status workflow:

  * TODO
  * IN_PROGRESS
  * DONE
* Priority levels:

  * LOW / MEDIUM / HIGH
* Due date tracking

---

### 📊 Dashboard & Analytics

* Total tasks
* Completed tasks
* Pending tasks
* Overdue tasks
* High priority tasks
* Recent work section
* Project health overview

---

### 📋 Task Views

* 🧩 Kanban Board (default)
* 📊 Table View (toggle)

---

### ⚙️ Profile Management

* View profile
* Edit name
* Change password (with validation)

---

### 🎨 UI/UX

* Premium SaaS-style interface
* Dark mode (default)
* Light mode support
* Sidebar layout
* Responsive design
* Clean spacing and typography

---

### 🔎 Additional Features

* Task search
* Filters (status, priority, project)
* Toast notifications
* Loading states
* Empty states

---

## 🛠 Tech Stack

### Frontend

* React (Vite)
* Tailwind CSS
* Axios
* React Router
* Lucide Icons

### Backend

* Node.js
* Express.js
* MongoDB (Mongoose)
* JWT Authentication
* bcrypt
* dotenv
* cors

### Deployment

* Frontend: Netlify
* Backend: Railway
* Database: MongoDB Atlas

---

## 📁 Project Structure

```bash
taskflow/
│
├── frontend/          # React (Vite) application
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/           # Express API
│   ├── src/
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   └── package.json
│
└── README.md
```

---

## ⚙️ Environment Variables

### Backend (.env)

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
CLIENT_URL=https://task-flow-sh.netlify.app
```

### Frontend (.env)

```env
VITE_API_URL=https://task-flow-sh.up.railway.app/api
```

---

## ▶️ Local Setup

### 1. Clone repository

```bash
git clone https://github.com/your-username/taskflow.git
cd taskflow
```

---

### 2. Install dependencies

```bash
cd backend
npm install

cd ../frontend
npm install
```

---

### 3. Run Backend

```bash
cd backend
npm run dev
```

API runs on:

```
http://localhost:5000/api
```

---

### 4. Run Frontend

```bash
cd frontend
npm run dev
```

App runs on:

```
http://localhost:5173
```

---

## 🧪 Seed Demo Data

```bash
cd backend
npm run seed
```

Creates:

* Admin user
* Member user
* Sample project
* Sample tasks

### Demo Credentials

* Admin: `admin@admin.com` / `Admin@123`
* Member: `member@member.com` / `Member@123`

---

## ⚙️ PM2 (Backend Production)

```bash
cd backend
pm2 start src/server.js --name taskflow-api
```

---

## 🏗 Build Frontend

```bash
cd frontend
npm run build
```

Output:

```
frontend/dist
```

---

## 🚀 Deployment

### Backend (Railway)

1. Push repository to GitHub
2. Create Railway project
3. Set root directory:

```
/backend
```

4. Add environment variables:

```env
MONGO_URI=your-mongodb-atlas-connection-string
JWT_SECRET=your-secret
CLIENT_URL=https://task-flow-sh.netlify.app
NODE_ENV=production
```

5. Deploy and generate domain

---

### Frontend (Netlify)

1. Connect GitHub repository
2. Configure build:

* Base directory: `frontend`
* Build command: `npm run build`
* Publish directory: `dist`

3. Add environment variable:

```env
VITE_API_URL=https://task-flow-sh.up.railway.app/api
```

4. Deploy

---

## 📡 API Routes

### Authentication

* `POST /api/auth/signup`
* `POST /api/auth/login`
* `GET /api/auth/me`

### Users

* `GET /api/users/me`
* `PUT /api/users/profile`
* `PUT /api/users/change-password`

### Projects

* `GET /api/projects`
* `POST /api/projects`
* `GET /api/projects/:id`
* `POST /api/projects/:id/members`

### Tasks

* `GET /api/tasks`
* `POST /api/tasks`
* `PUT /api/tasks/:id`
* `DELETE /api/tasks/:id`

### Dashboard

* `GET /api/dashboard/stats`

---

## 🧠 Design Philosophy

* Simplicity over complexity
* Clean UI over flashy design
* Scalable backend architecture
* Real-world SaaS approach
* Maintainable codebase

---

## 📌 Highlights

* Full-stack production-ready app
* Deployed on Netlify + Railway
* Role-based access system
* Clean and modern UI
* Real-world feature implementation

---

## 👨‍💻 Author

**Priyanshu Shroti**
📧 [priyanshushroti@gmail.com](mailto:priyanshushroti@gmail.com)

---

## ⭐ Support

If you found this project useful, consider giving it a star ⭐
