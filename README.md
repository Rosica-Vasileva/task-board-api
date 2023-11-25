## TaskBoard API

TaskBoard exposes a RESTful API for managing tasks and boards. The base URL for the API is [https://taskboardjsv02.softuniqa.repl.co/api](https://taskboardjsv02.softuniqa.repl.co/api) or in your case `http://{yoursite}/api`.

### Endpoints

- **GET /api**
  - List all API endpoints.
  
   https://taskboardjsv02.softuniqa.repl.co/api
- **GET /api/tasks**
  - List all tasks (returns JSON array of tasks).

   https://taskboardjsv02.softuniqa.repl.co/api/tasks
- **GET /api/tasks/id**
  - Returns a task by the given id.

  https://taskboardjsv02.softuniqa.repl.co/api/tasks/3
- **GET /api/tasks/search/keyword**
  - List all tasks matching the given keyword.

  https://taskboardjsv02.softuniqa.repl.co/api/tasks/search/tasks
- **GET /api/tasks/board/boardName**
  - List tasks by board name.

- **POST /api/tasks**
  - Create a new task (post a JSON object in the request body, e.g., `{"title":"Add Tests", "description":"API + UI tests", "board":"Open"}`).

- **PATCH /api/tasks/id**
  - Edit a task by id (send a JSON object in the request body, holding the fields to modify, e.g., `{"title":"changed title", "board":"Done"}`).

- **DELETE /api/tasks/id**
  - Delete a task by id.

- **GET /api/boards**
  - List all boards.

### Example

To list all tasks, make a GET request to [https://taskboardjsv02.softuniqa.repl.co/api/tasks](https://taskboardjsv02.softuniqa.repl.co/api/tasks).




