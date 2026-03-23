# HEARTBEAT.md

## Task Polling

Every heartbeat, Hermes checks the Task API for pending tasks.

```bash
curl -s "http://localhost:18793/api/tasks?assignee=hermes&status=inbox"
curl -s "http://localhost:18793/api/tasks?assignee=hermes&status=active"
```

If tasks found, include in heartbeat response:
`🔔 You have N pending task(s) — review inbox.`

## Notes

- Keep polling lightweight — just GET requests, no paginated loops
- Track last check times in memory/heartbeat-state.json
