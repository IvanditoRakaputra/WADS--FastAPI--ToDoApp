# WADS--FastAPI--ToDoApp
Create and design RestAPI using FastAPI for TodoAPP

| Endpoint         | Method   | Description           | Body Request                                             | Body Response                                          |
|------------------|----------|-----------------------|----------------------------------------------------------|--------------------------------------------------------|
| `/tasks`         | `GET`    | Fetch all tasks       | None                                                     | `[{ "id": {id}, "title": {title}, "description": {description}, "completed": {completed} }]` |
| `/tasks/{id}`    | `GET`    | Fetch a single task   | None                                                     | `{ "id": {id}, "title": {title}, "description": {description}, "completed": {completed} }`  |
| `/tasks`         | `POST`   | Create a new task     | `{ "title": {title}, "description": {description}, "completed": {completed} }` | `{ "message": "Task created successfully", "id": {id} }` |
| `/tasks/{id}`    | `PUT`    | Update an existing task | `{ "title": {title}, "description": {description}, "completed": {completed} }` | `{ "id": {id}, "title": {title}, "description": {description}, "completed": {completed} }` |
| `/tasks/{id}`    | `DELETE` | Delete a task         | None                                                     | `{ "error": {error}, "message": "Task deleted successfully" }` |
