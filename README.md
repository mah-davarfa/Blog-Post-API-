## Blog-Post-API
Overview

Blog-Post-API is a RESTful API built with Express.js for managing blog posts and users. The project demonstrates core backend concepts including routing, middleware, controllers, and the MVC (Model–View–Controller) architecture. It supports full CRUD operations and is designed for learning, testing, and portfolio demonstration purposes.

## Features

RESTful API design
CRUD operations for blog posts
CRUD operations for users
Query-based filtering (e.g., users by role)
Centralized routing and controllers
MVC project structure
JSON request and response handling
Environment-based configuration

## Technologies Used
Node.js
Express.js
JavaScript (ES6+)
Postman (for API testing)
Git & GitHub

## Project Structure
Blog-Post-API/
│
├── controllers/
│ ├── postsController.js
│ └── usersController.js
│
├── routes/
│ ├── posts.js
│ └── users.js
│
│
├── server.js
├── package.json
├── README.md

## API Endpoints
Root & Health
Method	Endpoint	Description
GET	/	API documentation and available routes
GET	/health	Health check endpoint

Posts
Method	Endpoint	Description
GET	/api/posts	Get all posts
GET	/api/posts/:id	Get a post by ID
POST	/api/posts	Create a new post
PUT	/api/posts/:id	Update a post
DELETE	/api/posts/:id	Delete a post

Users
Method	Endpoint	Description
GET	/api/users	Get all users or filter by role
GET	/api/users/:id	Get user by ID
POST	/api/users	Create a new user
PUT	/api/users/:id	Update a user
DELETE	/api/users/:id	Delete a user

## Data Models
Post
{
"id": 1,
"title": "Post title",
"content": "Post content",
"author": "Author name",
"published": true,
"createdAt": "2025-01-01T00:00:00.000Z"
}
User
{
"id": 1,
"name": "User name",
"email": "user@example.com",
"role": "author",
"createdAt": "2025-01-01T00:00:00.000Z"
}

## Getting Started
Installation
git clone https://github.com/mah-davarfa/Blog-Post-API-.git
cd Blog-Post-API
npm install

## Run the Server
npm run dev
The server will start at:
http://localhost:3000

## Testing the API
Use Postman to test the endpoints:
Create requests for each endpoint
Use JSON bodies for POST and PUT requests
Verify status codes and responses

## Learning Objectives
This project demonstrates:
How to structure an Express app using MVC
How to separate routes and controllers
How to handle request validation and responses
How to design and test RESTful APIs

## Future Improvements
Database integration (MongoDB)
Authentication and authorization

## Author
Mahmoud Davarfara
This project is for educational purposes.