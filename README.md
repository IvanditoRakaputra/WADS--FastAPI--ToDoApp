# WADS--FastAPI--ToDoApp
Create and design RestAPI using FastAPI for TodoAPP

| Endpoint        | Method   | Description           | Body Request                                             | Body Response                                          |
|-----------------|----------|-----------------------|----------------------------------------------------------|--------------------------------------------------------|
| `/task/`        | `GET`    | Fetch all tasks       | None                                                     | `[{ "id": id, "title": title, "description": description, "completed": completed }]` |
| `/task/{task_id}` | `GET`    | Fetch a single task   | None                                                     | `{ "id": id, "title": title, "description": description, "completed": completed }`  |
| `/task/`        | `POST`   | Create a new task     | `{ "title": title, "description": description, "completed": completed }` | `{"id": id, "title": title, "description": description, "completed": completed}` |
| `/task/{task_id}` | `PUT`    | Update an existing task | `{ "title": title, "description": description, "completed": completed }` | `{ "id": id, "title": title, "description": description, "completed": completed }` |
| `/task/{task_id}` | `DELETE` | Delete a task         | None                                                     | `{ "message": "Task deleted successfully", "id": id }` |
