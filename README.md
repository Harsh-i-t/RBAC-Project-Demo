# RBAC REST API with Node.js, MongoDB, Passport & Session
A comprehensive Role-Based Access Control (RBAC) system designed to manage authentication and authorization for users, ensuring secure and efficient access control in a Node.js environment.

# Features
- Secure Authentication: Users can register, log in, and log out securely using Passport.js.
- Role-Based Authorization: Manage access control based on roles (Admin, User, Moderator), with permissions defined for specific resources and endpoints.
- Session Management: Sessions are securely managed using express-session with a MongoDB-based store.
- Middleware for Role Enforcement: Middleware ensures only authorized users can access protected routes.
- Flash Messaging: Notifications for success and error messages during user interactions.
- EJS Templates: Provides a clean, user-friendly interface for login, registration, and other views.

# Prerequisites
Before running this project, ensure the following software is installed:

Node.js: JavaScript runtime for the server.
MongoDB: NoSQL database to manage user sessions and role-based data.

# Build Setup
- Clone the repository:
`
git clone https://github.com/Harsh-i-t/RBAC-Project-Demo.git
cd rbac-project-demo
`

- Install dependencies:
`npm install`

- Create a .env file in the root directory and configure the following environment variables:
`
PORT=4000
MONGO_URI=mongodb://127.0.0.1:27017/rbac_db
SESSION_SECRET=harshit
ADMIN_EMAIL=admin@gmail.com
`
- Start the development server:
`npm run dev`

# Security Best Practices
- Passwords are hashed using bcrypt.
- User sessions are secured with a session secret and stored in MongoDB.
- Role-based middleware restricts unauthorized access to sensitive route
