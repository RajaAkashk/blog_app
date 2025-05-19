# Full Stack Blog Editor Assignment

## Overview

This is a full-stack Blog Editor application built as part of an internship hiring task. The app allows users to write, edit, save drafts automatically, and publish blog posts. It features a React frontend with Tailwind CSS and Axios, and a MERN stack backend with Express.js, MongoDB, JWT authentication, and bcrypt for password hashing.

---

## Features

### Frontend
- Built with **React** (using Vite) and **Tailwind CSS**.
- Blog Editor page with:
  - Title input
  - Content textarea (or rich text editor)
  - Tags input (comma-separated)
- Buttons for **Save as Draft** and **Publish**.
- **Auto-save draft** feature triggered every 30 seconds or after 5 seconds of inactivity (debounced).
- Lists of all blogs showing published and drafts separately.
- Edit and update existing drafts and published posts.
- Visual notification (toast) on auto-save success.

### Backend
- Built with **Node.js**, **Express.js**, and **MongoDB** (MERN stack).
- User authentication with **JWT** and **bcrypt**.
- Blog model schema with:
  - `id`
  - `title`
  - `content`
  - `tags`
  - `status` (`draft` or `published`)
  - `created_at`
  - `updated_at`
- RESTful API endpoints:
  - `POST /api/blogs/save-draft` — Save or update draft.
  - `POST /api/blogs/publish` — Publish blog post.
  - `GET /api/blogs` — Retrieve all blogs.
  - `GET /api/blogs/:id` — Retrieve blog by ID.
- Error handling and validation.

---

## Setup Instructions

### Prerequisites

- Node.js and npm installed
- MongoDB instance (local or cloud)

### Backend Setup

1. Navigate to the backend folder Server

   ```bash
   cd server


2.Install dependencies: 
npm install

3.Create a .env file in the backend roo
MONGODB=<your-mongodb-connection-string>
JWT_SECRET=<your-jwt-secret-key>

4.Start the backend server:npm start


Frontend Setup
1.Navigate to the frontend folder
cd client/blogSite

2.Install dependencies:
npm install

3.Start the frontend dev server:
npm run dev

Usage
Register with email and password.

Login with email and password.

Write blog posts using the editor.

Drafts auto-save in backend.

Save drafts manually or publish posts.

View all blogs (drafts and published) in separate lists.

Edit existing drafts.

Technologies Used
Frontend: React, Vite, Tailwind CSS, Axios

Backend: Node.js, Express.js, MongoDB, Mongoose, bcrypt, JWT

Deployment: Local development

















   
