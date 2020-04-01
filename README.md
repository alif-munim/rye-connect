# Rye Connect

A social network for Ryerson University computer science students.

Created using MongoDB, Express, React, and Node.js.

## Features

- [ ] Registration and login
- [ ] User profiles
- [ ] Posts and discussions
- [ ] GitHub connectivity via GitHub API

## Dependencies

- express

  A framework for Node.js. Minimal tools for handling HTTP request and response.

- mongoose

  An Object Data Modeling (ODM) for MongoDB and Node.js. Used to create document schemas and model data.

- bcryptjs

  For hashing passwords before storing them in MongoDB.

- express-validator

  For validating user input and sending the appropriate error response on invalid input.

- jsonwebtoken

  Return a json web token upon user registration or login. Users will be able to access protected routes with this token in request headers.

- config
- request
- gravatar

## Dev Dependencies

- nodemon
- concurrently
