---
name: tasks-plan
description: Create an implementation plan from a Notion task or specification. Breaks down requirements into actionable steps with estimates and dependencies.
---

# Plan Task Implementation

Create a detailed implementation plan from a Notion task or specification page.

## Input

The user provides a Notion page URL containing a task or specification.

## Workflow

### 1. Fetch the specification

Use the Notion MCP tools to:
- Get the page content including requirements, acceptance criteria, and constraints
- Read any linked pages or references for additional context
- Identify dependencies and blockers

### 2. Analyze requirements

Extract and categorize:
- Functional requirements (what the system should do)
- Non-functional requirements (performance, security, etc.)
- Acceptance criteria (how to verify completion)
- Dependencies (what needs to happen first)

### 3. Break down into tasks

Create a structured implementation plan:
- Group work into logical phases or milestones
- Break each phase into specific, actionable tasks
- Identify the technical approach for each task
- Note any risks or uncertainties

### 4. Create the plan in Notion

Use the Notion MCP to create a new page with:
- Title: "Implementation Plan: [Feature Name]"
- Overview section summarizing the approach
- Phases with task checklists
- Dependencies and risks sections
- Link back to the original specification

### 5. Optionally create tasks

If the user has a task database, offer to create individual task items for each step in the plan.

## Output Format

The plan should include:
- **Overview**: Brief summary of what will be built
- **Specification Link**: Reference to the source document
- **Technical Approach**: High-level architecture decisions
- **Phases**: Numbered phases with task checklists
- **Dependencies**: What needs to be in place first
- **Risks**: Potential issues and mitigations
