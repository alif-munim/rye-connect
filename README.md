# Rye Connect

A social network for Ryerson University computer science students.

Created using MongoDB, Express, React, and Node.js.
<br/>
<br/>

### 🧰 Back-End Dependencies

```bash
npm i express mongoose bcryptjs express-validator jsonwebtoken config request gravatar
```

- express: a framework for Node.js. Minimal tools for handling HTTP request and response.

- mongoose: an Object Data Modeling (ODM) for MongoDB and Node.js. Used to create document schemas and model data.

- bcryptjs: for hashing passwords before storing them in MongoDB.

- express-validator: for validating user input and sending the appropriate error response on invalid input.

- jsonwebtoken: return a json web token upon user registration or login. Users will be able to access protected routes with this token in request headers.

- config: set configurations for app deployment. Store environment variables, database connection URI.

- request: make http call to github API to load recent user repos.

- gravatar: globally recognized avatars. Fetches profile image associated with an email for display on posts and comments.

- nodemon: constant monitoring of server updates. Automatically restart on change.

- concurrently: allows server and client processes to run concurrently.

<br/>
<br/>

### 🕹 Front-End Dependencies

- axios: to make http requests
- react-dom
- react-router-dom: to create routes and links to different react components.
- moment
- react-moment
- redux
- redux-devtools-extension
- redux-thunk
