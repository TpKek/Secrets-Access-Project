# Welcome to Secret Access Project 👋

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

> A server-side web application built with Node.js and Express.js that demonstrates fundamental security workflows using custom middleware to validate user input and control access to restricted content.

## 🛠 How it Works

This project uses a custom middleware function called `passwordCheck`:
- Intercepts the `POST` request from the login form
- Verifies the password before the request reaches the final `/check` route
- Uses `body-parser` to handle incoming form data
- Implements authentication state management with `isAuthenticated` flag

## Prerequisites

- Node.js (v14 or higher recommended)
- npm (comes with Node.js)

## Project Structure
```
.
├── index.js           # Main server file with Express routes and middleware
├── index.html         # Login page with password form
├── secret.html        # Protected page with secrets (accessible after authentication)
├── package.json       # Project dependencies and metadata
└── README.md          # Project documentation
```

## Install
```sh
npm install
```

This will install the required dependencies:
- `express` - Web framework for Node.js
- `body-parser` - Middleware to parse incoming request bodies

## Usage

1. Start the server:
```sh
   node index.js
```

2. Open your browser to `http://localhost:3000`

3. Enter the secret password: `ILoveProgramming`

4. If authenticated successfully, you'll be granted access to the secret page containing fun life tips!

## Features

✅ Custom middleware for authentication
✅ Password-protected content
✅ Form handling with body-parser
✅ Separation of public and protected routes
✅ ES6 modules syntax

## Learning Objectives

This project is ideal for understanding:
- How Express.js middleware works
- Request/response cycle in Node.js
- Basic authentication implementation
- Form data handling
- File serving with Express

## Security Note

⚠️ **This is a learning/demonstration project only!** The authentication method used here is NOT secure for production use. In real applications, you should:
- Never hardcode passwords in source code
- Use proper authentication libraries (Passport.js, JWT, etc.)
- Hash passwords with bcrypt
- Implement session management
- Use HTTPS

## Author

👤 **Bertin Dreyer**

* Github: [@TpKek](https://github.com/TpKek)

## Show your support

Give a ⭐️ if this project helped you!

---

_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator) and edits by Bertin Dreyer_
