---
name: tasks-setup
description: Set up a Notion task board for tracking tasks. Guides users through using a template or connecting an existing board.
---

# Notion Task Board Setup

Help the user set up their Notion workspace to work with the task skills in this plugin.

## Setup Options

### Option 1: Use a Template

If the user wants to start fresh:

1. Point them to duplicate this template: https://notion.notion.site/code-with-notion-board
2. Instruct them to duplicate the template to their workspace by opening the link and clicking the duplicate button in the top bar (icon is two squares).
3. Once duplicated, have them share the URL of their new board - tell them to click the share button in the top-right and then Copy Link.

### Option 2: Use an Existing Board

If the user already has a Notion board they want to use:

1. Ask them to provide the URL to their existing board
2. Use the Notion MCP tools to inspect the board structure
3. Verify it has the necessary properties for task management (e.g., Status, Title, etc.)
4. If properties are missing, suggest what they should add

## After Setup

Once the user has a board configured:

1. Confirm you can access it via the Notion MCP
2. Let them know they can now use other skills:
   - `tasks-build` to build a specific task
   - `tasks-explain-diff` to generate documentation for code changes

Remember: Be conversational and helpful. This is a setup wizard, not a one-shot command.
