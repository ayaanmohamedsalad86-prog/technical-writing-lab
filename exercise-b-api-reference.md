# Exercise B: API Reference Entry

## Create a New Task API

### 1. Overview

This API endpoint allows an authenticated user to create a new task in a project management application.

The user can provide a task title, description, assignee, due date, and priority level. After successful creation, the API returns the details of the newly created task.

### 2. HTTP Method and Endpoint

- **HTTP Method:** POST
- **Endpoint:** `/api/v1/projects/{project_id}/tasks`

**Description:** The POST method is used to send new task information to the server and create a task inside a specific project.
### 3. Request Parameters

#### Path Parameters

| Parameter | Data Type | Required | Description |
|---|---|---|---|
| project_id | Integer | Yes | The unique ID of the project where the task will be created. |

#### Query Parameters

This endpoint does not require any query parameters.

#### Request Body Parameters

| Parameter | Data Type | Required | Description |
|---|---|---|---|
| title | String | Yes | The name of the task. |
| description | String | No | A short explanation of the task. |
| assignee_id | Integer | Yes | The ID of the user assigned to the task. |
| due_date | String (Date) | Yes | The task deadline in YYYY-MM-DD format. |
| priority | String | Yes | The priority level: low, medium, or high. |
