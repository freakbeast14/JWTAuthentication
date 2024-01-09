# Web Application Authentication using JSON Web Tokens (JWT)

## Overview

This web application leverages the power of JSON Web Tokens (JWT) for authentication, providing a secure and efficient method to manage user identity. JWTs are generated upon user login and serve as a means to validate user authenticity, ensuring authorized access to specific routes and enhancing the overall security of the application.

## Technologies Used

* **JWT**: JSON Web Tokens provide a compact and self-contained way to securely transmit information between parties as a JSON object.
  
* **Node.js**: A server-side JavaScript runtime for building scalable network applications.

* **Express.js**: A fast, unopinionated, minimalist web framework for Node.js, ideal for building robust and scalable web applications.

* **JavaScript**: The programming language used for both server-side and client-side logic.

* **SCSS**: A preprocessor scripting language that is interpreted or compiled into Cascading Style Sheets (CSS).

## Authentication Flow

1. **User Login**: When a user successfully logs in, a unique JWT is generated on the server.

2. **JWT Creation**: The server creates a JWT containing relevant user information and a signature to verify its authenticity.

3. **Token Issuance**: The JWT is issued to the client, typically stored in a secure manner such as an HTTP-only cookie.

4. **Authorization**: Subsequent requests from the client include the JWT, allowing the server to validate the user's identity and authorize access to protected routes.

5. **Token Expiry**: To enhance security, JWTs often have an expiration time. The client needs to refresh the token or re-authenticate once it expires.

## Project Structure

* **`/src`**: Contains server-side code written in Node.js and Express.
  
* **`/public`**: Holds client-side assets, including HTML, CSS (SCSS), and client-side JavaScript.

* **`/config`**: Configuration files for JWT secret, algorithm, and other settings.

* **`/routes`**: Express route handlers for different parts of the application, including authentication routes.

* **`/middleware`**: Custom middleware functions, such as JWT verification middleware.

## Getting Started

1. Clone the repository: `git clone https://github.com/freakbeast14/JWTAuthentication.git`

2. Install dependencies: `npm install`

3. Set up your environment variables, including the JWT secret.

4. Start the server: `npm start`

5. Access the application at `http://localhost:3000` (or another specified port).
