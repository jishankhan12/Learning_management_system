# Learning_management_system

Learning Management System (LMS) - MERN Stack


A full-stack Learning Management System built with the MERN stack (MongoDB, Express.js, React, Node.js) that provides a complete online learning platform for students, instructors, and administrators.




🚀 Live Demo

Frontend: learninggmanagementsystem.netlify.app

🖼 Screenshots Dashboard overview Course player interface Instructor course creation Admin panel


📋 Table of Contents

Features Tech Stack Installation Environment Variables API Endpoints Project Structure Screenshots Contributing License ✨ Features

👨‍🎓 Student Features

Browse and search courses Enroll in courses Watch video lessons with progress tracking Take quizzes and assignments Track learning progress Participate in course discussions Receive completion certificates 👨‍🏫 Instructor Features

Create and manage courses Upload multimedia content (videos, PDFs, images) Create quizzes and assignments Track student progress and performance Manage course curriculum Rich text editor for course content 👨‍💼 Admin Features

User management (students, instructors) Course approval system Analytics and reporting System configuration Revenue tracking (if monetized) 🛠 Tech Stack

Frontend

React - UI framework Redux Toolkit - State management Material-UI - Component library Axios - HTTP client React Router - Navigation Socket.io-client - Real-time features Backend

Node.js - Runtime environment Express.js - Web framework MongoDB - Database Mongoose - ODM JWT - Authentication bcryptjs - Password hashing Cloudinary - Media storage Socket.io - Real-time communication Deployment

Netlify - Frontend hosting Render/Railway - Backend hosting MongoDB Atlas - Cloud database 🚀 Installation

Prerequisites

Node.js (v14 or higher) MongoDB (local or Atlas) npm or yarn Steps

Clone the repository

Backend Setup

bash cd backend npm install Frontend Setup

bash cd frontend npm install Environment Setup

Create .env files in both frontend and backend directories Add environment variables (see below) Run the application


bash



Backend (from backend directory)

npm run dev

Frontend (from frontend directory)

npm run dev 🔧 Environment Variables

Backend (.env)

env PORT=5000 MONGO_URI=your_mongodb_connection_string JWT_SECRET=your_jwt_secret_key CLOUDINARY_CLOUD_NAME=your_cloudinary_name CLOUDINARY_API_KEY=your_cloudinary_key CLOUDINARY_API_SECRET=your_cloudinary_secret Frontend (.env)

env VITE_API_URL=http://localhost:5000 VITE_CLOUDINARY_CLOUD_NAME=your_cloudinary_name 📡 API Endpoints

Authentication


POST /auth/register - User registration POST /auth/login - User login POST /auth/refresh - Refresh token POST /auth/logout - User logout Courses

GET /student/course - Get all courses (students) GET /student/course/:id - Get single course POST /instructor/course - Create course (instructor) PUT /instructor/course/:id - Update course DELETE /instructor/course/:id - Delete course Enrollment & Progress


POST /student/order - Enroll in course GET /student/courses-bought - Get enrolled courses PUT /student/course-progress - Update lesson progress Media

POST /media/upload - Upload course media DELETE /media/:id - Delete media

Dashboard overview Course player interface Instructor course creation Admin panel

Material-UI for the component library Cloudinary for media management MongoDB Atlas for database hosting Netlify for frontend deployment


