# Taskflow Manager – Backend

This is the backend for Taskflow Manager, a simple employee and task management system.
It’s built using Node.js, Express, and MongoDB. The backend exposes clean REST APIs that the frontend uses to manage employees and tasks.

# What this backend does

Connects to MongoDB

Provides APIs for employees and tasks

Uses Express router for clean structure

Handles JSON data and enables CORS

Runs a simple server with a health check route

The code is easy to understand and beginner-friendly.

# Tech Stack

Node.js

Express

MongoDB / Mongoose

dotenv

CORS

# Project Structure
config/

db.js

routes/

employeeRoutes.js
taskRoutes.js

server.js

.env
package.json

# Getting Started
1. Clone the repo
git clone https://github.com/Samriti-Raj/Taskflow-manager.git
cd Taskflow-manager

2. Install dependencies
npm install

3. Create a .env file

Add the following:

MONGO_URI=your_mongo_connection_string
PORT=5000

4. Start the server
npm start


If everything works, we will see:

Server running on PORT 5000

# Available API Routes
Employees

GET /api/employees

GET /api/employees/:id

POST /api/employees

PUT /api/employees/:id

DELETE /api/employees/:id

Tasks

GET /api/tasks

GET /api/tasks/:id

POST /api/tasks

PUT /api/tasks/:id

DELETE /api/tasks/:id

Health Check

We can visit this in the browser:

http://localhost:5000/


We should see:

API is running...

# About the Server

The main server file sets up Express, connects to MongoDB, enables CORS, parses JSON and registers the employee and task routes.
It’s clean and minimal, making it easy to maintain or scale later.