---
name: spec-to-implementation
description: Turn product or tech specs into concrete Notion tasks. Breaks down spec pages into detailed implementation plans with clear tasks, acceptance criteria, and progress tracking.
---

# Spec to Implementation

Transforms specifications into actionable implementation plans with progress tracking. Fetches spec documents, extracts requirements, breaks down into tasks, and manages implementation workflow.

## Quick Start

When asked to implement a specification:

1. **Find spec**: Search Notion to locate specification page
2. **Fetch spec**: Read specification content
3. **Extract requirements**: Parse and structure requirements from spec
4. **Create plan**: Create implementation plan page in Notion
5. **Find task database**: Search for tasks database
6. **Create tasks**: Create individual tasks in task database
7. **Track progress**: Update status as work progresses

## Implementation Workflow

### Step 1: Find the specification

Search for spec with name or topic. Look for spec title or keyword matches. If not found or ambiguous, ask user for spec URL/ID.

Example searches:
- "User Authentication spec"
- "Payment Integration specification"
- "Mobile App Redesign PRD"

### Step 2: Fetch and analyze specification

1. **Fetch spec page**: Read full content including requirements, design, constraints

2. **Parse specification**:
   - Identify functional requirements
   - Note non-functional requirements (performance, security, etc.)
   - Extract acceptance criteria
   - Identify dependencies and blockers

### Step 3: Create implementation plan

Break down into:
1. Phases/milestones
2. Technical approach
3. Required tasks
4. Effort estimates
5. Risks and mitigations

### Step 4: Create implementation plan page

Create in Notion with:
- Title: "Implementation Plan: [Feature Name]"
- Content: Structured plan with phases, tasks, timeline
- Link back to original spec
- Add to appropriate location (project page, database)

### Step 5: Find and use task database

1. Search for "Tasks" or "Task Management" database
2. Fetch database schema to understand properties
3. If not found, ask user for database location

### Step 6: Create implementation tasks

For each task in plan:
1. Create task in database
2. Set properties: Name, Status (To Do), Priority, Related Tasks
3. Add implementation details in content

### Step 7: Track progress

Regular updates:
- Update task status
- Add progress notes (completed, current focus, blockers)
- Update implementation plan with milestone completion
- Link to deliverables (PRs, designs, etc.)

## Implementation Plan Structure

- **Overview**: Brief summary
- **Linked Spec**: Reference to source document
- **Requirements Summary**: Key requirements extracted
- **Technical Approach**: Architecture decisions
- **Implementation Phases**:
  - Phase goal
  - Tasks checklist
  - Estimated effort
- **Dependencies**: What needs to happen first
- **Risks & Mitigation**: Potential issues
- **Success Criteria**: How to verify completion

## Task Breakdown Patterns

| Pattern | Use When |
|---------|----------|
| **By Component** | Database, API, frontend, integration, testing |
| **By Feature Slice** | Vertical slices (auth flow, data entry, reports) |
| **By Priority** | P0 (must have), P1 (important), P2 (nice to have) |

## Best Practices

1. **Always link spec and implementation**: Maintain bidirectional references
2. **Break down into small tasks**: Each completable in 1-2 days
3. **Extract clear acceptance criteria**: Know when "done" is done
4. **Identify dependencies early**: Note blockers in plan
5. **Update progress regularly**: Daily notes for active work
6. **Track changes**: Document spec updates and their impact
7. **Use checklists**: Visual progress indicators help everyone
8. **Link deliverables**: PRs, designs, docs should link back to tasks

## Common Issues

| Issue | Solution |
|-------|----------|
| Can't find spec | Search with name/topic, try broader terms, ask user for URL |
| Multiple specs found | Ask user which spec to implement |
| Can't find task database | Search for "Tasks", ask user for location |
| Spec unclear | Note ambiguities in plan, create clarification tasks |
| Requirements conflicting | Document conflicts, create decision task |
| Scope too large | Break into smaller specs/phases |
