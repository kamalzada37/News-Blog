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
