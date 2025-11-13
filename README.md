🧠 Thinkboard

A full-stack MERN application for creating, storing, and managing notes — built with MongoDB, Express, React, Node.js, and enhanced with Upstash Redis rate-limiting, Axios API layer, TailwindCSS, and Vite.

🚀 Features
🖥️ Frontend (React + Vite)

Fast Vite-powered React app

Pages:

HomePage – display all notes

CreatePage – create a new note

NoteDetailPage – view an individual note

Components:

Navbar

NoteCard

NotesNotFound

RateLimitedUI

API wrapper using Axios (src/lib/axios.js)

TailwindCSS + DaisyUI styling

🗄️ Backend (Node + Express)

REST API for notes

Endpoints:

GET /api/notes

POST /api/notes

GET /api/notes/:id

MongoDB connection via Mongoose

Upstash Redis rate-limiting

Organized MVC structure:

controllers/

models/

routes/

middleware/

📁 Project Structure
Thinkboard/
│
├── backend/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   └── server.js
│   └── package.json
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── lib/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── vite.config.js
│   └── package.json
│
└── package.json (root)

🛠️ Tech Stack
Frontend

React 19

React Router 7

Axios

TailwindCSS + DaisyUI

Vite

Backend

Node.js

Express

MongoDB + Mongoose

Upstash Redis (REST API)

Rate limiting middleware

🔧 Environment Variables

Create a .env file inside backend/:

MONGO_URI=your_mongodb_uri
UPSTASH_REDIS_REST_URL=your_upstash_url
UPSTASH_REDIS_REST_TOKEN=your_upstash_token
PORT=5001

▶️ Running Locally
Backend
cd backend
npm install
npm start


Backend runs on:
http://localhost:5001

Frontend
cd frontend
npm install
npm run dev


Frontend runs on:
http://localhost:5173

🌐 Deployment (Render)
Backend

Deploy as a Web Service

Build command:

cd backend && npm install


Start command:

cd backend && npm start

Frontend

Deploy as a Static Site

Build command:

cd frontend && npm install && npm run build


Publish folder:

frontend/dist

📝 API Routes
Get all notes

GET /api/notes

Create a note

POST /api/notes

{
  "title": "My Note",
  "content": "Note details"
}

Get a note by ID

GET /api/notes/:id

🧩 Future Improvements

Edit notes

Delete notes

User authentication

Cloud image uploads

Rich text editor
