# 🧩 MERN Stack Integration — Week 4 Assignment

## 📖 Project Overview
This project is part of the **PLP MERN Stack Development Program (Week 4: Deep Dive into MERN Stack Integration)**.  
The goal of this assignment is to build a **full-stack blog application** demonstrating seamless integration between:
- **MongoDB** (database)
- **Express.js** (backend API)
- **React.js (Vite)** (frontend interface)
- **Node.js** (server environment)

The project covers complete CRUD functionality, authentication, image uploads, pagination, search, and comments — showcasing modern MERN stack development and integration skills.

---

## 🚀 Features Implemented
✅ **Full CRUD operations** for blog posts  
✅ **RESTful API** built with Express and MongoDB (Mongoose)  
✅ **React front-end** with component-based architecture  
✅ **User authentication** using JWT (register & login)  
✅ **Category management** for organizing posts  
✅ **Image upload** using Multer  
✅ **Pagination, search & filtering**  
✅ **Comments system** for user interaction  
✅ **Protected routes** and state management with React Context  
✅ **Environment variables** for configuration  
✅ **Responsive design** and clean UI  

---

## 🧱 Project Structure

mern-stack-integration-Jsews/
<br>├── client/ # React front-end (Vite)</br>
<br>│ ├── public/</br>
<br>│ ├── src/</br>
<br>│ │ ├── components/</br>
<br>│ │ ├── pages/</br>
<br>│ │ ├── hooks/</br>
<br>│ │ ├── services/</br>
<br>│ │ ├── context/</br>
<br>│ │ └── App.jsx</br>
<br>│ └── package.json</br>
<br>├── server/ # Express.js back-end</br>
<br>│ ├── config/</br>
<br>│ ├── controllers/</br>
<br>│ ├── models/</br>
<br>│ ├── routes/</br>
<br>│ ├── middleware/</br>
<br>│ ├── uploads/</br>
<br>│ ├── server.js</br>
<br>│ └── package.json</br>
<br>└── README.md</br>


---

## ⚙️ Installation & Setup Guide

### 🧩 Prerequisites
Make sure you have installed:
- **Node.js** (v18+)
- **npm** (comes with Node)
- **MongoDB** (local or MongoDB Atlas)
- **Git**

---

### 🖥️ 1. Clone the Repository
```bash
git clone https://github.com/PLP-MERN-Stack-Development/mern-stack-integration-Jsews.git
cd mern-stack-integration-Jsews

🗄️ 2. Server Setup
cd server
npm install


Create an .env file using the example provided:

cp .env.example .env


Then add your environment variables:

# Port your Express server will run on
PORT=5000

# MongoDB connection string (local)
MONGO_URI=mongodb://localhost:27017

# JWT secret for authentication
JWT_SECRET=supersecretkey



Start the development server:

npm run dev

💻 3. Client Setup
cd ../client
npm install


Create an .env file:

VITE_API_BASE_URL=http://localhost:5000/api


Start the React front-end:

npm run dev


Open your browser at http://localhost:5173

🧠 API Documentation
🔐 Authentication
Method	Endpoint	Description
POST	/api/auth/register	Register new user
POST	/api/auth/login	Login and get JWT token
📝 Blog Posts
Method	Endpoint	Description
GET	/api/posts	Get all posts (supports page, limit, search, category)
GET	/api/posts/:id	Get single post by ID
POST	/api/posts	Create a new post (requires token)
PUT	/api/posts/:id	Update post (requires token)
DELETE	/api/posts/:id	Delete post (requires token)
🏷️ Categories
Method	Endpoint	Description
GET	/api/categories	Get all categories
POST	/api/categories	Create a category
💬 Comments
Method	Endpoint	Description
GET	/api/posts/:postId/comments	Get approved comments for a post
POST	/api/posts/:postId/comments	Submit a comment for a post
🧩 Technologies Used
Layer	Technology
Frontend	React.js (Vite), React Router, Axios, React Hook Form
Backend	Express.js, Node.js
Database	MongoDB, Mongoose
Authentication	JWT, bcryptjs
Validation	express-validator, Joi
File Uploads	Multer
State Management	React Context API, Hooks
Styling	CSS / Tailwind (optional)

	
	
🧪 Testing

Use Postman or cURL to test your endpoints.
Example:

curl -X POST http://localhost:5000/api/posts \
  -H "Authorization: Bearer <token>" \
  -F "title=My Blog Post" \
  -F "content=This is a test post"

💾 Environment Files
server/.env.example
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/blog
JWT_SECRET=your_jwt_secret
PORT=5000

client/.env.example
VITE_API_BASE_URL=http://localhost:5000/api

🧹 Folder Notes
Folder	Description
/client/src/components	UI components like NavBar, PostCard, Pagination
/client/src/pages	Page-level components (Home, Post, Login, Register, etc.)
/client/src/context	React Context for authentication
/server/models	Mongoose models for User, Post, Category, Comment
/server/routes	Express API routes
/server/middleware	Authentication, error handling, validation
/server/uploads	Local storage for images
🧭 Advanced Features (Implemented)

🔐 User authentication with JWT tokens

🖼️ Image uploads using Multer

💬 Comment system

🔍 Search and filter posts

⏩ Pagination for blog list

⚡ Optimistic UI updates

🧱 Proper input validation and error handling

🏁 Expected Outcome

Fully functional MERN Blog Application

Proper integration between MongoDB, Express, React, and Node

Clean code organization and clear separation of concerns

Responsive front-end and smooth user experience

📚 References

MongoDB Documentation

Express.js Guide

React Docs

Node.js Docs

Mongoose Docs

👩🏽‍💻 Author

Janice Tusiime Sewava
MERN Stack Developer — PLP MERN Stack Development Program

🧾 License

This project is for educational purposes under the PLP MERN Stack Development Program.
