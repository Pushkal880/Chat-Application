# Chat Application 💬

A full-stack real-time chat application built with the MERN stack and Socket.io. Users can sign up, log in, update their profile, and exchange real-time messages (including images) with other users, with online status shown live.

## Features

- 🔐 Authentication & authorization with JWT (httpOnly cookies)
- 💬 Real-time one-on-one messaging with Socket.io
- 🟢 Live online/offline user status
- 🖼️ Image sharing in chat via Cloudinary
- 🎨 Theme switching (DaisyUI themes)
- 👤 Profile management (avatar upload, account info)
- 🧠 Global state management with Zustand
- ⚠️ Error handling on both client and server

## Tech Stack

**Frontend**
- React + Vite
- Zustand (state management)
- Tailwind CSS + DaisyUI
- Socket.io-client
- Axios, React Router, React Hot Toast

**Backend**
- Node.js + Express
- MongoDB with Mongoose
- Socket.io
- JWT authentication
- Cloudinary (image uploads)

## Project Structure

```
Chat-Application/
├── backend/
│   └── src/
│       ├── controllers/   # Auth & message logic
│       ├── lib/           # DB, Socket.io, Cloudinary, utils
│       ├── middleware/    # Route protection
│       ├── models/        # User & Message schemas
│       ├── routes/        # API routes
│       └── seeds/         # Seed data
└── frontend/
    └── src/
        ├── components/    # Chat UI, sidebar, skeletons, etc.
        ├── pages/         # Login, Sign up, Home, Profile, Settings
        └── store/         # Zustand stores (auth, chat, theme)
```

## Getting Started

### Prerequisites
- Node.js
- A MongoDB instance (e.g. MongoDB Atlas)
- A Cloudinary account (for image uploads)

### Setup

1. Clone the repository
   ```bash
   git clone https://github.com/Pushkal880/Chat-Application.git
   cd Chat-Application
   ```

2. Create a `.env` file inside `backend/`:
   ```
   MONGODB_URI=...
   PORT=5001
   JWT_SECRET=...

   CLOUDINARY_CLOUD_NAME=...
   CLOUDINARY_API_KEY=...
   CLOUDINARY_API_SECRET=...

   NODE_ENV=development
   ```

3. Build the app (installs backend + frontend dependencies and builds the frontend)
   ```bash
   npm run build
   ```

4. Start the app
   ```bash
   npm start
   ```

## License

This project is for personal/educational purposes.
