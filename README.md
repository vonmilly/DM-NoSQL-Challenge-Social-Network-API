# Social Network API

## Overview

This Social Network API is a robust backend application designed to manage users, thoughts, reactions, and friendships within a social network setting. Built using Express.js, MongoDB, and Mongoose, it ensures efficient data storage and retrieval.

## Installation

To set up the Social Network API locally, follow these steps:

1. Clone the repository

2. Navigate to the project directory

3. Install dependencies

4. Configure the MongoDB database:
- Ensure MongoDB is installed on your machine.
- Update the MongoDB connection URL in `config/connection.js` if required.

5. Start the server


The API server will be accessible at `http://localhost:3001/`.

## Usage

Once the server is running, interact with the API using tools like Insomnia or Postman. Below are the available routes:

### User Routes:
- GET /api/users - Retrieve all users
- GET /api/users/:id - Retrieve a user by ID
- POST /api/users - Create a new user
- PUT /api/users/:id - Update a user by ID
- DELETE /api/users/:id - Delete a user by ID
- POST /api/users/:userId/friends/:friendId - Add a friend to a user's friend list
- DELETE /api/users/:userId/friends/:friendId - Remove a friend from a user's friend list

### Thought Routes:
- GET /api/thoughts - Retrieve all thoughts
- GET /api/thoughts/:thoughtId - Retrieve a thought by ID
- POST /api/thoughts - Create a new thought
- PUT /api/thoughts/:thoughtId - Update a thought by ID
- DELETE /api/thoughts/:thoughtId - Delete a thought by ID
- POST /api/thoughts/:thoughtId/reactions - Add a reaction to a thought
- DELETE /api/thoughts/:thoughtId/reactions/:reactionId - Remove a reaction from a thought

Ensure to replace the route parameters (`:id`, `:thoughtId`, `:userId`, `:friendId`, `:reactionId`) with actual values when making requests.

To create or update data, send POST or PUT requests with the required data in the request body, formatted as JSON.

Upon successful requests, the API will respond with the appropriate success status code. In case of errors, descriptive error messages will be returned.

## Testing

You can test the API functionality using tools like Insomnia or Postman. Here's what you can do:

1. Open Insomnia or Postman.
2. Test GET routes for users and thoughts to view formatted JSON data.
3. Test POST, PUT, and DELETE routes to create, update, and delete users and thoughts.
4. Test POST and DELETE routes to create and delete reactions to thoughts, and add and remove friends from a user's friend list.

## Author

This project was authored by Devonte Miller.

