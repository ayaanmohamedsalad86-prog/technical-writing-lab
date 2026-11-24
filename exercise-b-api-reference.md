# Exercise B: API Reference Entry

## Create a New Task API

### 1. Overview

This API endpoint allows an authenticated user to create a new task in a project management application.

The user can provide a task title, description, assignee, due date, and priority level. After successful creation, the API returns the details of the newly created task.

### 2. HTTP Method and Endpoint

- **HTTP Method:** POST
- **Endpoint:** `/api/v1/projects/{project_id}/tasks`

**Description:** The POST method is used to send new task information to the server and create a task inside a specific project.
