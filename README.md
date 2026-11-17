# Full Stack MERN Blog (WS06)

This repository contains a fully functional Full-Stack MERN (MongoDB, Express, React, Node.js) blog application. It was originally built as part of the WS06 React + REST API workshop.

## Features

- **REST API:** Node.js & Express backend providing complete CRUD operations.
- **Database:** MongoDB integration with strict Mongoose schema validation.
- **Frontend:** React SPA (Single Page Application) built with Vite and React Router.
- **Proxy Routing:** Seamless frontend-to-backend communication via Vite proxy.

## Project Structure

```text
WS06_React/
├─ Starter/         # The completed working application
│  ├─ backend/      # Express API & MongoDB models
│  └─ frontend/     # React UI components & pages
├─ README.md
└─ requirements.md
```

## Run Instructions

You will need two separate terminal windows to run the frontend and backend simultaneously.

### 1. Start the Backend

Open your first terminal and run:

```bash
cd Starter/backend
npm install
cp .env.example .env
```
Note: Ensure you add your MongoDB connection string (MONGODB_URI) to the newly created .env file before starting the server.
```bash
npm run dev
```
### 2. Start the Frontend
Open a new terminal window:
```bash
cd Starter/frontend
npm install
npm run dev
```
Vite will start the development server (usually on http://localhost:5173). The frontend is configured to automatically proxy API requests (/api/posts) to the backend.