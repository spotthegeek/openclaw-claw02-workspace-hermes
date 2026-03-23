# TASKS.md - Task Management

All tasks are managed via the Task API.

## Endpoints

- **Inbox:** `GET http://localhost:18793/api/tasks?assignee=hermes&status=inbox`
- **Active:** `GET http://localhost:18793/api/tasks?assignee=hermes&status=active`
- **Complete:** `PATCH http://localhost:18793/api/tasks/:id` with `{"status": "done"}`
- **Create:** `POST http://localhost:18793/api/tasks`

## Notes

- Tasks have: title, description, assignee, status (inbox|active|done), priority
- Always claim a task before starting (move inbox → active)
- Mark done when complete
