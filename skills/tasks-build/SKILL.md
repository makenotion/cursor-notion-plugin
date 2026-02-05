---
name: tasks-build
description: Build a task from a Notion page URL. Fetches task details, marks it in progress, implements the work, and updates status in Notion.
---

# Build Task from Notion

Build a task that is tracked in Notion. The user may be watching the Notion board, so all feedback should be sent through Notion.

## Input

The user provides a Notion task URL.

## Workflow

### 1. Fetch the task details

Use the Notion MCP tools to:
- Get the page content including title, description, and any relevant properties
- Look for acceptance criteria, requirements, or specifications
- Read any linked pages or references if needed

### 2. Mark in progress

- Change the status of the task to "In progress"
- Update the "Agent status" field (if present) to contain a short description: an emoji followed by a word like "Starting..." or "Working..."

### 3. Build it

- Work on the task per the specification. If this is a codebase, implement the code changes.
- At each step, update the "Agent status" field to explain what's currently happening, so the user can see progress. Keep it brief: a relevant emoji followed by a few words. Examples: "Searching relevant files...", "Updating color scheme...", "Running tests..."
- If you need user input to clarify the spec or answer questions, add a comment to the task prefixed with "Message from AI:" and set any "Agent blocked" field to true.

### 4. Update the task status

Once complete:
- Update the task status in Notion to "Done"
- If you made a code change, consider using the `tasks-explain-diff` skill to generate documentation
- Add a final comment summarizing the results

## Notes

- If the URL is invalid or inaccessible, ask the user to verify the URL and their Notion connection
- If requirements are unclear, ask clarifying questions before implementing
