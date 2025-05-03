# Node.js Authentication App with PostgreSQL & Passport.js

A full-stack authentication system built using Node.js, Express, PostgreSQL, and Passport.js. EJS is used as the templating engine for the frontend.

## 🔧 Features

- User registration with email and password
- Secure password hashing using bcrypt
- Session-based authentication with Passport.js
- Protected route (`/secrets`) accessible only after login
- Login, logout functionality

## 🧰 Tech Stack

- Backend: Node.js, Express.js
- Authentication: Passport.js (Local Strategy), bcrypt
- Database: PostgreSQL
- Frontend: EJS (Embedded JavaScript Templates)
- Session Management: express-session

## 🗃️ Database Setup

1. Make sure PostgreSQL is installed and running on your local machine.
2. Create a new PostgreSQL database. Use the file db.sql to create a table in PostgreSQL

Use the following sql code to create a user table using postgreql 
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email VARCHAR(255) UNIQUE NOT NULL,
  password VARCHAR(255) NOT NULL
);

