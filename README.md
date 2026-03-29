# Travelers Blog

## Overview
Travelers Blog is a web application built with Node.js, Express.js, EJS, and MongoDB. It includes user authentication, an admin panel for user management, and pages that display data from two external APIs. The application uses a responsive layout with a shared navigation bar and footer across all pages.

## Features
- User signup and login
- Admin panel for managing users
- Integration with two external APIs
- History page for user interactions
- Shared navbar and footer across pages
- Responsive design

## Tech Stack
- **Backend:** Node.js, Express.js
- **Frontend:** EJS, HTML, CSS, JavaScript
- **Database:** MongoDB
- **Environment Management:** dotenv

## Project Structure
```text
project/
├── .env                 # Environment variables such as API keys and MongoDB URI
├── package.json         # Project metadata and dependencies
├── README.md            # Project documentation
├── seed.js              # Script for inserting initial data into the database
├── server.js            # Main server file and routing logic
├── views/
│   ├── admin.ejs        # Admin panel for managing users
│   ├── api1.ejs         # Page for displaying data from API 1
│   ├── api2.ejs         # Page for displaying data from API 2
│   ├── footer.ejs       # Shared footer
│   ├── history.ejs      # Page showing user interaction history
│   ├── login.ejs        # Login page
│   ├── main.ejs         # Main page after login
│   ├── navbar.ejs       # Shared navigation bar
│   └── signup.ejs       # Signup page

Requirements

Before running the project, make sure you have installed:

Node.js
 (recommended: LTS version)
npm
MongoDB locally, or a MongoDB Atlas connection string
Installation and Setup
1. Clone the repository
git clone <your-repository-link>
cd <your-project-folder>
2. Install dependencies
npm install
3. Create a .env file

In the project root, create a file named .env and add your environment variables.

Example:

MONGODB_URI=your_mongodb_connection_string
API_KEY_1=your_first_api_key
API_KEY_2=your_second_api_key
PORT=3000
SESSION_SECRET=your_secret_key
4. Seed the database (if needed)

If your project requires initial data:

node seed.js
5. Start the application
node server.js

If the project uses nodemon, you can run:

npx nodemon server.js
6. Open in browser

Go to:

http://localhost:3000
Admin Access

Use the following credentials for admin login:

Username: Mustafa jan
Password: 12345

For security, hardcoded credentials should be replaced with environment variables or securely stored user records in production.

Design Choices
EJS is used as the templating engine to render dynamic HTML pages.
Express.js handles routing, middleware, and server-side logic.
The project structure separates views and server logic to keep the application organized and easier to maintain.
Shared components such as the navbar and footer provide a consistent user experience across all pages.
Notes
Make sure MongoDB is running if you are using a local database.
Check that all API keys in the .env file are valid.
Do not upload your .env file to GitHub.
Future Improvements
Add password hashing with bcrypt
Add role-based authorization
Improve admin dashboard features
Add error handling and validation messages
Deploy the application online
Acknowledgments

Thanks to all resources and contributors that supported the development of this project.
