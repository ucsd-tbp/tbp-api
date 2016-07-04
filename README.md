*Still a work in progress! Working on documentation, JWT authentication, permission groups, tests, and eventually some front-end framework.*

### Overview

This project is an API written in Node.js for keeping track of event attendance between members and initiates at UCSD TBP. The API uses the [Express framework](http://expressjs.com) along with [Bookshelf](http://bookshelfjs.org) as an ORM for a familiar MVC structure to help with code maintainability.

### Development Setup

Install the latest version of [Node.js](https://nodejs.org/en/).

Copy `.env.example` to a new file, `.env`, and replace the placeholder values with the configuration for your environment. The `.env` file is loaded in `server/database/knexfile.js` so that the Knex CLI can see the environment variables, and so that the `.env` file loads as early in the application as possible.

Install application dependencies.
```
npm install
```
To run the application in development:
```
npm run start
```
The start script uses `nodemon` to restart the server when files are changed.

### Contributing

Loosely following the [Airbnb ES6 style guide](https://github.com/airbnb/javascript). A lint script is also provided:
```
npm run lint
```
For more info on how the project is set up, check out the wiki and the [data layer README](server/database/README.md).
