# 📝 MERN Stack Note Taking App (ThinkBoard)

A modern full-stack note-taking application built using the MERN stack (MongoDB, Express, React, Node.js), styled with TailwindCSS & DaisyUI, and rate-limited via Upstash Redis.

---

## ✨ .env Setup

### Backend (`/backend/.env`)

Create a `.env` file inside the `backend` folder and add the following:

```env
PORT=5001
MONGO_URI=<your_mongo_uri>

UPSTASH_REDIS_REST_URL=<your_redis_rest_url>
UPSTASH_REDIS_REST_TOKEN=<your_redis_rest_token>

NODE_ENV=development
```

---

## 🔧 Run the Backend

```bash
cd backend
npm install
npm run dev
```

The backend server runs on `http://localhost:5001`.

---

## 💻 Run the Frontend

```bash
cd frontend
npm install
npm run dev
```

The frontend application runs on `http://localhost:5173`.

---

## 🚀 Features

- **CRUD Operations**: Create, read, update, and delete notes.
- **Rate Limiting**: Protected endpoints using Upstash Redis.
- **Modern UI**: Styled with Tailwind CSS and DaisyUI.
- **Toasts & Feedback**: Interactive notifications using `react-hot-toast`.

