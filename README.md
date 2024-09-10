# ToDoApp

## Description
ToDoApp is an application for managing tasks (To-Do) using API and Docker containerization.

The application allows users to create, view, update, and delete tasks. It provides a user-friendly interface for managing tasks, making it easy to add new tasks, track their status, and prioritize them.

## Installation and Setup

Requirements
Docker: Install Docker on your machine.

## Installation Steps
1. Clone the ToDoApp repository to your local machine
```
$ git clone https://github.com/your-username/ToDoApp.git
```
2. Navigate to the project directory:
```
$ cd ToDoApp
```
3. Build and start the Docker containers using the following command:
```
$ docker-compose up -d
```
This command will build and start the application and database containers.

4. The ToDoApp will be accessible at http://localhost:8000.


## Using the API

### Getting a list of tasks (Read)
URL: `/api/todo/`
Method: GET
Returned data: List of all tasks

### Get task details (Update)
URL: `/api/todo/<id>/`
Method: GET
URL parameters:
- `<id>`: Task ID
Returned data: Details of the task with the specified ID

### Create a new task (Create)
URL: `/api/todo/create/`
Method: POST
Request parameters:
- Task fields in JSON format
Returned data: Created task

### Deleting a task (Delete)
URL: `/api/todo/<id>/delete/`
Method: DELETE
URL parameters:
- `<id>`: Task ID
Returned data: Task deletion status



