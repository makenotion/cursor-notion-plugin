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
| **Knowledge Capture** | Transform conversations into structured Notion documentation |
| **Meeting Intelligence** | Prepare meeting materials with context and research |
| **Research Documentation** | Search, synthesize, and document research findings |
| **Spec to Implementation** | Turn specs into tasks with progress tracking |

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
| `knowledge-capture` | Capture knowledge from conversations |
| `meeting-intelligence` | Prepare comprehensive meeting materials |
| `research-documentation` | Research and document topics from Notion |
| `spec-to-implementation` | Convert specs to implementation plans |

---

## Installation

### 1. Add the plugin

In Cursor, add this plugin from the marketplace or install directly from GitHub:

```
makenotion/cursor-notion-plugin
```

### 2. Restart Cursor

This ensures the MCP server starts correctly.

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
├── .cursor/
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
    ├── knowledge-capture/
    ├── meeting-intelligence/
    ├── research-documentation/
    └── spec-to-implementation/
```

---

## Credits

- **Skills** by Notion
- **MCP Server** by Notion
- **Plugin Specification** by Cursor
