# Rye Connect

A social network for Ryerson University computer science students.

Created using MongoDB, Express, React, and Node.js.

## Features

Features to be implemented.

### Back-End

Currently creating API routes.

#### Setup

- [ ] Install dependencies
- [ ] Build server, create basic routes
- [ ] Connect to database

#### Registration & Login

- [ ] Create user schema
- [ ] POST request for user registration
- [ ] POST request for user login
- [ ] User authentication & protected routes with JWT

### Front-End

To be implemented using React and Redux.

## Dependencies

- **express**

  A framework for Node.js. Minimal tools for handling HTTP request and response.

- **mongoose**

  An Object Data Modeling (ODM) for MongoDB and Node.js. Used to create document schemas and model data.

- **bcryptjs**

  For hashing passwords before storing them in MongoDB.

- **express-validator**

  For validating user input and sending the appropriate error response on invalid input.

- **jsonwebtoken**

  Return a json web token upon user registration or login. Users will be able to access protected routes with this token in request headers.

- **config**

  Set configurations for app deployment. Store environment variables, database connection URI.

- **request**
- **gravatar**

## Dev Dependencies

- nodemon
- concurrently
