# 📝 MERN Stack Note Taking App (ThinkBoard)

A modern full-stack note-taking application built with the MERN stack (MongoDB, Express, React, Node.js), styled with TailwindCSS & DaisyUI, and rate-limited via Upstash Redis.

---

## 🚀 Features

- **Full CRUD Operations**: Create, view, edit, and delete notes in real time.
- **Rate Limiting**: Protects backend APIs using **Upstash Redis** sliding window rate limiter.
- **Responsive & Modern UI**: Built with React, Tailwind CSS, Lucide icons, and DaisyUI themes.
- **Toasts & Feedback**: User-friendly alerts and notifications powered by `react-hot-toast`.
- **Production Ready**: Configured for single-command root build and static frontend serving in production.

---

## 🛠️ Tech Stack

- **Frontend**: React (Vite), React Router, TailwindCSS, DaisyUI, Lucide React, Axios, React Hot Toast
- **Backend**: Node.js, Express.js, MongoDB (Mongoose), CORS, Dotenv
- **Security & Rate Limiting**: Upstash Redis (`@upstash/ratelimit`, `@upstash/redis`)

---

## ✨ .env Setup

### Backend (`/backend/.env`)

Create a `.env` file inside the `backend` directory:

```env
PORT=5001
MONGO_URI=<your_mongo_uri>

UPSTASH_REDIS_REST_URL=<your_redis_rest_url>
UPSTASH_REDIS_REST_TOKEN=<your_redis_rest_token>

NODE_ENV=development
```

---

## 🔧 Local Development

### 1. Run the Backend
```bash
cd backend
npm install
npm run dev
```
Backend runs at `http://localhost:5001`.

### 2. Run the Frontend
```bash
cd frontend
npm install
npm run dev
```
Frontend runs at `http://localhost:5173`.

---

## 🌐 Production Build & Deployment

From the root directory:

```bash
# Install dependencies for both frontend & backend, and build frontend
npm run build

# Start the production backend server
npm start
```
