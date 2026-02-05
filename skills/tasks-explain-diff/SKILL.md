---
name: tasks-explain-diff
description: Generate a rich Notion document explaining code changes. Creates comprehensive documentation with background, intuition, code walkthrough, and verification steps.
---

# Explain Code Changes

Create a rich explanation of code changes as a new Notion page.

## Input

The user will point to code changes to explain. If not explicitly specified, explain the most recent batch of changes made in the conversation.

## Document Sections

### Background

Explain the existing system relevant to this change:
- Broadly explore surrounding code for context
- Include deep background for beginners (can be skipped by familiar readers)
- Provide narrow background directly relevant to the change

### Intuition

Explain the core intuition for the code change:
- Focus on the essence, not full details
- Use concrete examples with toy data
- Use figures and mermaid diagrams liberally

### Code

High-level walkthrough of the changes:
- Group and order changes in an understandable way
- Explain the purpose of each significant change
- Link to specific files and line numbers

### Verification

Explain how the code change was verified:
- Unit tests, integration tests, etc.
- Step-by-step guide for manual QA

### Alternatives

Describe 1-2 alternative approaches (if identifiable):
- Each alternative includes pros and cons
- Layout pros/cons in 2 columns
- Only include if it represents an orthogonal approach
- Omit this section if no meaningful alternatives exist

### Quiz

5 questions testing reader's knowledge:
- Medium difficulty - requires understanding the substance
- Multiple choice with explanations
- Use toggle blocks for answers:

```markdown
1. Question
   > Option 1
     - Explanation for why incorrect
   > Option 2
     - Explanation for why correct
```

## Formatting Guidelines

- Use the Notion MCP to create the page and return its URL
- Write with clarity and flow - engaging, classic style
- Smooth transitions between sections
- Use consistent diagram families throughout
- Include callouts for key concepts, definitions, and edge cases
