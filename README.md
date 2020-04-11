# Rye Connect

A social network for Ryerson University computer science students.

Created using MongoDB, Express, React, and Node.js.

## Back-End

Currently creating API routes.
<br/>
<br/>

### 🔧 Dependencies

```bash
npm i express mongoose bcryptjs express-validator jsonwebtoken config request gravatar
```

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

### 📦 Dev Dependencies

- **nodemon**

  Constant monitoring of server updates. Automatically restart on change.

- **concurrently**

  Allows server and client processes to run concurrently.

### Setup

- [x] Install dependencies
- [x] Build server, create basic routes
- [x] Connect to database

### Registration & Login

- [x] Create user schema
- [x] POST request for user registration
- [x] POST request for user login
- [x] User authentication & protected routes with JWT

### User Profiles

- [x] Create profile schema
- [x] POST route to create new profile
- [x] PUT route to update existing profile
- [x] GET route for all profiles
- [x] GET route for single profile by id
- [x] DELETE route for profile and user
- [x] POST, DELETE routes for profile education
- [x] POST, DELETE routes for profile experience
- [x] Retrieve recent GitHub repos using GitHub API

### Posts

- [x] Create post schema
- [x] POST route to add a post
- [x] GET route for all post
- [x] GET route for single post by id
- [x] DELETE route to remove a post
- [x] PUT routes for liking and unliking
- [x] POST, DELETE routes for comments

## Front-End

To be implemented using React and Redux.
Starting on April 9th, 2020.
