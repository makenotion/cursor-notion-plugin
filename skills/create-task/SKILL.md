---
name: create-task
description: Create a new task in the user's Notion tasks database with sensible defaults for due date, status, owner, and project.
---

# Create Notion Task

Use the Notion MCP server to create a new task for the user.

## Workflow

1. Interpret the request to extract:
   - Task title (required)
   - Optional due date
   - Optional status
   - Optional owner/assignee
   - Optional project or related page
2. Identify the appropriate "Tasks" database:
   - Prefer a database whose name or description clearly indicates tasks/todo items.
   - If more than one candidate exists, ask the user to choose.
3. Create a new row with:
   - Title set to the task title.
   - Due date, Status, Owner, Project, or similar properties mapped when available.
4. Confirm creation by returning:
   - Task title
   - Key properties
   - Link or identifier.

## Important

If required properties are missing or the tasks database cannot be confidently identified, ask a concise clarification question before making changes.
