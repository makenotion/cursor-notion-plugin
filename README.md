# Notion Plugin for Cursor

This repository provides an official Cursor plugin that bundles:

- **Notion Skills** that teach the AI how to work intelligently inside your Notion workspace
- The **[Notion MCP Server](https://developers.notion.com/docs/mcp)**, which enables secure search, read, and update operations on your Notion content
- A curated set of **Skills** that make common Notion workflows fast and natural

This plugin allows Cursor users to install everything — Skills + MCP server — with one click.

---

## Features

### Notion Skills

Includes high-quality skills for working with Notion:

| Skill | Description |
|-------|-------------|
| **Database designer** | Design Notion databases |
| **Knowledge capture** | Turn conversations into reusable docs |
| **Meeting intelligence** | Prepare meetings and follow-ups |
| **Research documentation** | Research and write cited docs |
| **Spec to implementation** | Turn specs into plans and tasks |
| **Weekly project digest** | Summarize progress, blockers, and next steps |
| **Build my engineering wiki** | Bring technical docs and projects together |
| **Create my team handbook** | Organize team knowledge and procedures |
| **Organize my semester** | Keep courses, notes, and deadlines together |
| **Plan marketing campaigns** | Organize campaigns, content, and production |
| **Set up my project** | Create a project home with tasks and docs |
| **Set up Notion** | Connect Notion and get started |

These workflows are synced from the [Notion cookbook MCP client skills](https://github.com/makenotion/notion-cookbook/tree/main/skills/mcp-clients), including their examples, references, and display metadata. When syncing, keep each packaged `SKILL.md` frontmatter `name` equal to its existing Cursor folder name (for example, `knowledge-capture`, without the cookbook’s `notion-` prefix), as required by [Cursor’s skill format](https://cursor.com/docs/skills#frontmatter-fields). The existing quick-action skills below remain available.

### Integrated Notion MCP Server

Cursor automatically connects to Notion's hosted MCP server at:

```
https://mcp.notion.com/mcp
```

This provides tools to:

- Search your workspace
- Retrieve pages & databases
- Create and update pages
- Append notes or blocks
- Insert database rows
- Work with properties safely

### Available Skills

| Skill | Description |
|-------|-------------|
| `search` | Search your entire Notion workspace |
| `find` | Quick title-based search for pages/databases |
| `create-page` | Create a new page under a given parent |
| `create-task` | Create a task in a Tasks-style database |
| `create-database-row` | Insert a row in any database |
| `database-query` | Query a database by name or ID |
| `tasks-setup` | Set up a Notion task board for tracking |
| `tasks-build` | Build a task from a Notion page URL |
| `tasks-plan` | Create implementation plan from a spec |
| `tasks-explain-diff` | Generate a Notion doc explaining code changes |
| `database-designer` | Design Notion databases |
| `knowledge-capture` | Turn conversations into reusable docs |
| `meeting-intelligence` | Prepare meetings and follow-ups |
| `research-documentation` | Research and write cited docs |
| `spec-to-implementation` | Turn specs into plans and tasks |
| `weekly-project-digest` | Summarize progress, blockers, and next steps |
| `build-my-engineering-wiki` | Bring technical docs and projects together |
| `create-my-team-handbook` | Organize team knowledge and procedures |
| `organize-my-semester` | Keep courses, notes, and deadlines together |
| `plan-marketing-campaigns` | Organize campaigns, content, and production |
| `set-up-my-project` | Create a project home with tasks and docs |
| `setup` | Set up Notion for your agent |

---

## Installation

### 1. Add the plugin

In Cursor, add this plugin from the marketplace or install directly from GitHub:

```
makenotion/cursor-notion-plugin
```

---

## Authentication

The Notion MCP server supports **OAuth**. You'll be prompted to authenticate with your Notion account when first using the plugin.

---

## Usage Examples

### Search your workspace

Ask Cursor to search for content:
- "Search my Notion for Q1 roadmap documents"
- "Find pages about customer feedback"

### Create content

- "Create a new meeting notes page for tomorrow's standup"
- "Add a task to fix the login bug, due Friday"
- "Insert a row in my Projects database for the new feature"

### Prepare for meetings

- "Prep me for tomorrow's product review meeting"
- "Create a pre-read for the customer call with Acme Corp"

### Document research

- "Research and document our API architecture decisions"
- "Create a comparison report of the authentication options we discussed"

### Implement specs

- "Create an implementation plan from the Payment Integration spec"
- "Break down the Mobile App Redesign PRD into tasks"

---

## Directory Structure

```
cursor-notion-plugin/
├── .cursor-plugin/
│   └── plugin.json              # Plugin manifest
├── mcp.json                     # MCP server configuration
├── README.md                    # This file
└── skills/                      # All skills as SKILL.md files
    ├── search/
    ├── find/
    ├── create-page/
    ├── create-task/
    ├── create-database-row/
    ├── database-query/
    ├── tasks-setup/
    ├── tasks-build/
    ├── tasks-plan/
    ├── tasks-explain-diff/
    ├── database-designer/
    ├── knowledge-capture/
    ├── meeting-intelligence/
    ├── research-documentation/
    ├── spec-to-implementation/
    ├── weekly-project-digest/
    ├── build-my-engineering-wiki/
    ├── create-my-team-handbook/
    ├── organize-my-semester/
    ├── plan-marketing-campaigns/
    ├── set-up-my-project/
    └── setup/
```

---

## Credits

- **Skills** by Notion
- **MCP Server** by Notion
- **Plugin Specification** by Cursor
