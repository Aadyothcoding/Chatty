# Realtime Chat App

A full-stack real-time chat application built with **React**, **Vite**, **Tailwind CSS**, **DaisyUI**, **Zustand**, **Socket.IO**, **Express**, **MongoDB**, and **Cloudinary**.

---

## Features

- **User Authentication**: Sign up, login, logout, and JWT-based session management.
- **Profile Management**: Update profile picture (with Cloudinary upload).
- **Real-time Messaging**: Send and receive messages instantly using Socket.IO.
- **Image Attachments**: Send images in chat.
- **Online Status**: See which users are online.
- **Theme Switching**: Choose from multiple DaisyUI themes.
- **Responsive UI**: Works on desktop and mobile.

---

## Tech Stack

- **Frontend**: React 19, Vite, Tailwind CSS, DaisyUI, Zustand, React Router, Socket.IO Client, Axios
- **Backend**: Node.js, Express, MongoDB (Mongoose), Socket.IO, Cloudinary, JWT, bcryptjs
- **Dev Tools**: ESLint, PostCSS, concurrently

---

## Project Structure

```
chat-app/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── lib/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   └── seeds/
│   ├── .env
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── constants/
│   │   ├── lib/
│   │   ├── pages/
│   │   ├── store/
│   │   └── index.css
│   ├── index.html
│   ├── tailwind.config.js
│   ├── postcss.config.js
│   └── package.json
├── package.json
└── readme.md
```

---

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- MongoDB Atlas account (or local MongoDB)
- Cloudinary account (for image uploads)

### 1. Clone the repository

```sh
git clone https://github.com/yourusername/chat-app.git
cd chat-app
```

### 2. Install dependencies

```sh
npm run install-all
```

### 3. Configure environment variables

Create a `.env` file in `backend/`:

```
PORT=3000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

### 4. Seed the database (optional)

You can run the seed script in `backend/src/seeds/user.seed.js` to add demo users.

### 5. Start the app (development)

```sh
npm run dev
```

- Frontend: [http://localhost:5173](http://localhost:5173)
- Backend: [http://localhost:3000](http://localhost:3000)

---

## Scripts

- `npm run dev` — Start both frontend and backend in development mode
- `npm run build` — Build frontend for production
- `npm run start` — Start backend server (after building frontend)

---

## Customization

- **Themes**: Change or