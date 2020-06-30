# Rye Connect

A social network for Ryerson University computer science students.

Created using MongoDB, Express, React, and Node.js.

### What is the MERN Stack?
The MERN Stack is a free, open-source JavaScript software stack used to build end-to-end full-stack applications. It is comprised of the following technologies:
* **MongoDB** <br/>
  MongoDB is a document-based, "NoSQL" database program. Data in MongoDB is stored in collections consisting of documents in JSON-like format, with data modeled through user-defined schemas.
* **Node.js** <br/>
  Node.js is a JavaScript runtime powered by Chrome's V8 JavaScript engine. It is asynchronous, event-driven, and uses non-blocking I/O, which makes it lightweight and efficient. It is commonly used to build servers which are both fast and scalable due to its single-threaded architecture.
* **Express** <br/>
  Express is a web application framework for Node.js used to build web applications and APIs. It makes processes such as starting up a server much more efficient in comparison to starting from scratch in Node.js.
* **React** <br/>
  React is a JavaScript-based web framework used to build flexible user-interfaces. Complex interfaces can be broken down into a few fundamental components which can hold their own state and reflect data from a server. In React, UI and logic can be considered in parallel while maintaining separation of concerns. 
  
### Why use the MERN Stack for this project?
Rye-Connect was designed to be a fully-fledged social network for students across Ryerson's computer science program to build their portfolios and communicate with one another, much like LinkedIn. The concept, although relatively simple, included functionality which were unfamiliar to a developer coming from a purely HTML, CSS, and JavaScript background. Such functionality includes login & registration, user data storage, authentication, conditionally loaded components, and much more. The MERN Stack proved to be the perfect choice as it provided greater flexibility by breaking down the user interface into components, and relatively simple mechanisms for integrating these components with data retrieved from the server-side. 

<br/>
<br/>


# Back-End 

The most sensible approach to begin a project like this was to start with the back-end. Once the routing is complete and the API constructed, completing the remainder of the project is a matter of building around it. Using express made starting up the server and creating routes for simple `get`, `post`, `put`, and `delete` requests required in a REST API much simpler. Much of the data also needed to be modeled to verify user input, and for these tasks **MongoDB Atlas** was used. 

### Dependencies

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

<br/><br/>

# Front-End 

The front-end of this application, although seemingly simpled, proved to be the most challenging part. Managing state among so many different components turned out to be a tedious endeavor, but react-redux came to the rescue. Although it initially seemed merely to add an another layer of complexity, redux provided an intuitive way to connect to the back-end API and manage application-wide state using types, actions, and reducers.

### Dependencies

- axios: to make http requests
- react-dom: package for working with the DOM
- react-router-dom: to create routes and links to different react components.
- moment, react-moment: package for formatting date and time
- redux, redux-devtools-extension, redux-thunk: a javascript library for managing application-level state, commonly referred to a "single source of truth"
