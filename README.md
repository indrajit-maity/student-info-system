# Student Information System — MERN Mini Project

A simple, clean, and functional Student Information System built as a college-level MERN mini project. It focuses on the core fundamentals of the MERN stack (MongoDB, Express, React, Node) using pure JavaScript and native CSS.

## Features
- **Authentication**: JWT-based login with bcrypt password hashing
- **Dashboard**: Simple overview statistics
- **Student Management**: Full CRUD operations for student records
- **Search & Filter**: Search by name/ID/email and filter by department/semester
- **Responsive Design**: Mobile-friendly layout using plain CSS

## Tech Stack
- **Frontend**: React.js, Vite, React Router, HTML, Plain CSS, native `fetch()`
- **Backend**: Node.js, Express.js
- **Database**: MongoDB, Mongoose
- **Auth**: jsonwebtoken, bcryptjs

---

## College Practical Mapping

This project is intentionally designed to demonstrate the following 10 college practicals:

1. **Practical 1 (Responsive Webpage)**: Handled via `App.css` and `index.css` using CSS media queries and flex/grid layouts.
2. **Practical 2 (Form + JS Validation)**: The `StudentForm.jsx` component uses custom JavaScript logic to validate email, phone, semester bounds, and required fields before submission.
3. **Practical 3 (React Components + Props)**: UI is split into reusable components like `StudentCard`, `StudentTable`, `StudentForm`, passing data and callbacks via props.
4. **Practical 4 (Node.js + Express REST API)**: The backend provides RESTful endpoints (`GET`, `POST`, `PUT`, `DELETE`) with proper HTTP status codes.
5. **Practical 5 (MongoDB CRUD)**: The `studentController.js` performs real CRUD operations against a connected MongoDB database using Mongoose.
6. **Practical 6 (React Fetching API)**: The `api.js` service uses the native browser `fetch()` API to communicate with the Express backend.
7. **Practical 7 (User Login Authentication)**: Uses bcrypt to hash passwords and JWTs for secure login, protecting all API endpoints and React routes.
8. **Practical 8 (Git + GitHub)**: The project includes a `.gitignore` and is version controlled with logical commits.
9. **Practical 9 (Cloud Deployment)**: Configured via environment variables (`.env`) allowing independent deployment of the frontend (Vercel) and backend (Render) connected to MongoDB Atlas.
10. **Practical 10 (Student Information System)**: The final working application tying everything together.

---

## Project Structure

```
.
├── client/                 # React Frontend
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── layouts/        # Page layouts (Dashboard layout)
│   │   ├── pages/          # Full page components
│   │   ├── services/       # API integration
│   │   ├── App.jsx         # Main routing component
│   │   └── App.css         # Responsive styling
│   └── package.json
│
├── server/                 # Express Backend
│   ├── config/             # DB connection
│   ├── controllers/        # Route logic
│   ├── middleware/         # JWT auth middleware
│   ├── models/             # Mongoose schemas (User, Student)
│   ├── routes/             # Express routes
│   ├── seed.js             # Database seeder
│   └── server.js           # Entry point
│
└── package.json            # Root monorepo (starts both)
```

## Setup Instructions

### 1. Environment Setup
Create a `.env` file in both `client/` and `server/` directories based on the `.env.example` templates.

### 2. Install Dependencies
From the root folder, run:
```bash
npm run install:all
```

### 3. Seed Database
To populate the database with a demo admin user and 10 dummy students:
```bash
npm run seed
```

### 4. Run Locally
To run both the frontend and backend simultaneously:
```bash
npm run dev
```

The application will be available at:
- **Frontend**: `http://localhost:5173`
- **Backend API**: `http://localhost:5000`

---

## Demo Credentials
- **Email**: `admin@example.com`
- **Password**: `password123`

---

## Deployment Strategy
- **Database**: MongoDB Atlas cluster
- **Backend**: Render Web Service (using `npm start` in the `server` directory)
- **Frontend**: Vercel/Netlify (build command: `npm run build`, publish directory: `dist`)
