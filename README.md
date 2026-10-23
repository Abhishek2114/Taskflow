# Taskora

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./taskflow-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="./taskflow-light.svg">
    <img src="./taskflow-light.svg" alt="Taskora logo" width="220" />
  </picture>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Frontend-Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white" alt="Frontend Netlify" />
  <img src="https://img.shields.io/badge/Backend-Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white" alt="Backend Railway" />
  <img src="https://img.shields.io/badge/Database-MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Database MongoDB" />
  <img src="https://img.shields.io/badge/Auth-JWT-black?style=for-the-badge" alt="Authentication JWT" />
  <img src="https://img.shields.io/badge/UI-TailwindCSS-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="UI Tailwind CSS" />
</p>

<p align="center">
  <strong>Plan • Assign • Track • Deliver</strong>
</p>

Taskora is a modern team productivity platform designed to help teams manage projects, assign tasks, and monitor execution in one clean workflow. It blends the clarity of Kanban boards with the structure of project management dashboards, creating a SaaS-style experience that feels fast, focused, and production-ready.

## Live Demo

- Frontend: https://task-flow-sh.netlify.app/
- Backend API: https://task-flow-sh.up.railway.app/api/

## Why Taskora?

Taskora helps teams:

- organize work into projects and milestones
- assign ownership with clear task responsibilities
- monitor progress through real-time status tracking
- identify blockers, delays, and overdue work
- keep collaboration structured without adding complexity

Built with a scalable full-stack architecture, Taskora is designed to simulate a real-world SaaS product experience while staying easy to run locally and expand further.

## Features

### Authentication & Security

- JWT-based authentication
- Secure signup and login flow
- Password hashing with bcrypt
- Protected API routes

### Role-Based Access

- Admin access for project-wide management
- Member access for task updates and assigned work

### Project Management

- Create and manage projects
- Add teammates to projects
- View project details and progress
- Track project health with workload insights

### Task Management

- Create, update, delete, and assign tasks
- Status workflow: TODO, IN_PROGRESS, DONE
- Priority levels: LOW, MEDIUM, HIGH
- Due date tracking and overdue detection
- Search and filter task views

### Dashboard & Analytics

- Total tasks
- Completed and pending tasks
- Overdue workload
- High-priority alerts
- Recent activity overview
- Project health summary

### Product Experience

- Kanban board interface by default
- Table view toggle
- Dark mode with light mode support
- Responsive and clean SaaS-style layout
- Loading, empty, and notification states

## Tech Stack

### Frontend

- React + Vite
- Tailwind CSS
- Axios
- React Router
- Lucide Icons

### Backend

- Node.js
- Express.js
- MongoDB + Mongoose
- JWT authentication
- bcrypt
- dotenv
- cors

### Deployment

- Frontend: Netlify
- Backend: Railway
- Database: MongoDB Atlas

## Project Structure

```bash
taskora/
├── frontend/          # React + Vite client
│   ├── src/
│   ├── public/
│   └── package.json
├── backend/           # Express API server
│   ├── src/
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   └── package.json
├── taskflow-light.svg # branding asset
├── taskflow-dark.svg  # branding asset
├── README.md
└── netlify.toml
```

## Local Setup

### 1. Clone the repository

```bash
git clone https://github.com/Abhishek2114/Taskora.git
cd Taskora
```

### 2. Install dependencies

```bash
cd backend
npm install

cd ../frontend
npm install
```

### 3. Start the backend

```bash
cd backend
npm run dev
```

API will run at:

```text
http://localhost:5000/api
```

### 4. Start the frontend

```bash
cd frontend
npm run dev
```

The app will run at:

```text
http://localhost:5173
```

## Environment Variables

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

## Seed Demo Data

```bash
cd backend
npm run seed
```

This creates:

- admin user
- member user
- sample project
- sample tasks

### Demo credentials

- Admin: `admin@admin.com` / `Admin@123`
- Member: `member@member.com` / `Member@123`

## API Overview

### Authentication

- `POST /api/auth/signup`
- `POST /api/auth/login`
- `GET /api/auth/me`

### Users

- `GET /api/users/me`
- `PUT /api/users/profile`
- `PUT /api/users/change-password`

### Projects

- `GET /api/projects`
- `POST /api/projects`
- `GET /api/projects/:id`
- `POST /api/projects/:id/members`

### Tasks

- `GET /api/tasks`
- `POST /api/tasks`
- `PUT /api/tasks/:id`
- `DELETE /api/tasks/:id`

### Dashboard

- `GET /api/dashboard/stats`

## Design Philosophy

- simplicity over complexity
- clarity over clutter
- maintainable architecture
- real-world SaaS workflow design
- usability-first product experience

## Highlights

- Full-stack team productivity app
- production-ready workflow structure
- role-based access control
- clean modern interface
- deployment-ready stack

## Author

**Priyanshu Shroti**

- Email: [priyanshushroti@gmail.com](mailto:priyanshushroti@gmail.com)

## Support

If you found Taskora useful, please consider giving the project a star ⭐
