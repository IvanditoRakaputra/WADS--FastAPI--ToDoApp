# WADS--FastAPI--ToDoApp
Create and design RestAPI using FastAPI for TodoAPP

# Task Management API

This API allows for managing tasks within a database. Users can create, retrieve, update, and delete tasks.

## API Reference

### Endpoints

#### GET `/tasks`
- **Description**: Fetch all tasks
- **Body Request**: None
- **Body Response**: `[{ "id": {id}, "title": {title}, "description": {description}, "completed": {completed} }]`

#### GET `/tasks/{id}`
- **Description**: Fetch a single task by ID
- **Body Request**: None
- **Body Response**: `{ "id": {id}, "title": {title}, "description": {description}, "completed": {completed} }`

#### POST `/tasks`
- **Description**: Create a new task
- **Body Request**: `{ "title": {title}, "description": {description}, "completed": {completed} }`
- **Body Response**: `{ "message": "Task created successfully", "id": {id} }`

#### PUT `/tasks/{id}`
- **Description**: Update an existing task
- **Body Request**: `{ "title": {title}, "description": {description}, "completed": {completed} }`
- **Body Response**: `{ "id": {id}, "title": {title}, "description": {description}, "completed": {completed} }`

#### DELETE `/tasks/{id}`
- **Description**: Delete a task
- **Body Request**: None
- **Body Response**: `{ "error": {error}, "message": "Task deleted successfully" }`

## Setup

To set up and run the server:

1. Install dependencies:
   ```bash
   pip install fastapi uvicorn
