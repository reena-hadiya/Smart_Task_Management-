# 📝 Smart Task & Notes Management System (MERN)

A premium, full-stack application for managing tasks with a modern UI, featuring secure authentication, real-time filtering, and a sleek dark mode.

---

## 🚀 Quick Access (Running Project)

- **Frontend UI**: [http://localhost:5173](http://localhost:5173)
- **Backend API**: [http://localhost:5000](http://localhost:5000)

> [!TIP]
> Ensure both servers are running (`npm run dev` in both folders) before accessing these links.

---

## ✨ Features

- **🔐 Secure Auth**: Register and Login with JWT authentication and bcrypt password hashing.
- **📊 Real-time Dashboard**: Interactive stats for Total, Pending, Completed, and Overdue tasks.
- **🛠 Full CRUD**: Create, read, update, and delete tasks with ease.
- **🎨 Modern UI**: Clean, professional design built with vanilla CSS and Lucide icons.
- **🌓 Dark Mode**: Fully integrated dark/light mode toggle (persisted in local storage).
- **📱 Responsive**: mobile-first design with a collapsible sidebar.
- **🔍 Smart Search**: Filter tasks instantly by title or description.
- **⏳ Due Dates**: Track deadlines with automatic overdue detection.

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|-----------|
| **Frontend** | React 19, Vite, Axios, React Router, Lucide Icons |
| **Backend** | Node.js, Express 5 |
| **Database** | MongoDB + Mongoose |
| **Security** | JWT (JSON Web Tokens), bcryptjs |
| **Styling** | Vanilla CSS (Custom Design System) |

---

## 📂 Project Structure

```text
/
├── backend/               # Express API
│   ├── controllers/      # Route logic
│   ├── middleware/       # Auth & Error handlers
│   ├── models/           # Mongoose schemas
│   ├── routes/           # API endpoints
│   └── server.js         # Entry point
│
└── frontend/              # Vite + React
    ├── src/
    │   ├── components/    # Reusable UI parts
    │   ├── context/       # Auth & Theme state
    │   ├── pages/         # View components
    │   ├── services/      # Axios API logic
    │   └── assets/        # Styles & Icons
    └── index.html
```

---

## 🚀 Getting Started

### 1. Prerequisites
- Node.js (v18+)
- MongoDB (Local or Atlas)

### 2. Backend Setup
1. Navigate to the backend folder: `cd backend`
2. Install dependencies: `npm install`
3. Create a `.env` file and add:
   ```env
   PORT=5000
   MONGO_URI=mongodb://localhost:27017/smarttasks
   JWT_SECRET=your_secret_key
   ```
4. Start the server: `npm run dev`

### 3. Frontend Setup
1. Navigate to the frontend folder: `cd frontend`
2. Install dependencies: `npm install`
3. Create a `.env` file and add:
   ```env
   VITE_API_URL=/api
   ```
4. Start the dev server: `npm run dev`

---

## 🔌 API Endpoints

### Authentication
- `POST /api/auth/register` - Create new account
- `POST /api/auth/login` - Get access token
- `GET /api/auth/me` - Get user profile (Protected)

### Tasks (Protected)
- `GET /api/tasks` - Get all user tasks
- `POST /api/tasks` - Create a new task
- `PUT /api/tasks/:id` - Update a task
- `DELETE /api/tasks/:id` - Remove a task

---

## ☁️ Deployment

- **Backend**: Recommended for [Render](https://render.com) or [Railway](https://railway.app).
- **Frontend**: Recommended for [Netlify](https://netlify.com) or [Vercel](https://vercel.com).
- **Database**: Use [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) for a managed cloud database.

---

## 📄 License
MIT License - Feel free to use this for your own projects!
