# nodeJS-Task-Manager

# Task Manager API

A simple task management application built with Node.js and Express.

## Technologies

- Node.js
- Express
- MongoDB (with Mongoose)
- dotenv

## Dependencies

- **express**: Web framework for Node.js
- **mongoose**: MongoDB object modeling tool
- **dotenv**: Loads environment variables from a `.env` file
- **nodemon**: Automatically restarts the server during development

## Database

This application uses MongoDB for data storage. Make sure to have a MongoDB instance running and provide the connection string in the `.env` file.

## API Endpoints

### 1. Get All Tasks
- **Method**: `GET`
- **Endpoint**: `/api/v1/tasks`
- **Response**:
  ```json
  {
      "tasks": [
          {
              "id": "1",
              "name": "Task 1",
              "completed": false
          }
      ]
  }

### 2. POST
Endpoint: /api/v1/tasks
Request:
json
Copy code
{
    "name": "New Task",
    "completed": false
}

### 3 Method: PUT
Endpoint: /api/v1/tasks/:id
Request:
json
Copy code
{
    "name": "Updated Task",
    "completed": true
}

### 4 Method: DELETE
Endpoint: /api/v1/tasks/:id
