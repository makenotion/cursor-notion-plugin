---
name: create-page
description: Create a new Notion page, optionally under a specific parent. Automatically structures content based on page type (meeting notes, project pages, etc.).
---

# Create Notion Page

Use the Notion MCP server to create a new page for the user.

## Workflow

1. Parse the request into:
   - Page title
   - Optional parent page/database (if the user mentions a parent)
2. If the parent is ambiguous, ask a brief clarification question before creating the page.
3. Create the page with a sensible default structure based on the title:
   - For "Meeting notes", include sections like Attendees, Agenda, Notes, Action items.
   - For "Project" pages, include sections for Overview, Goals, Timeline, Tasks, Risks.
4. Confirm creation back to the user with:
   - Page title
   - Parent location
   - Link or identifier.

## Important

Be careful not to overwrite existing pages. If a page with the exact same name exists in the same parent, confirm with the user whether to reuse it or create a new one.
