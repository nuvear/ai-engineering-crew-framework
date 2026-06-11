# Collaboration Workspace Architecture

## Central Principle

The collaboration workspace is central, not optional. It consists of GitHub (project memory and source of truth) and Figma (design workspace).

## Without a Workspace

```text
Agents repeat questions.
Agents contradict each other.
Decisions are forgotten.
Scope expands uncontrolled.
Builder may build unapproved features.
QA may test the wrong thing.
```

## With a Workspace

```text
Requirements are traceable.
Decisions are recorded.
Approvals are visible.
Design is linked.
Build is linked to requirements.
Testing is linked to acceptance criteria.
```

## Components

| Component | Role |
|---|---|
| GitHub Repository | Official project memory, versioning, PRs, decision logs |
| GitHub Project Board | Workflow status tracking across all phases |
| GitHub Issues | Work items linked to requirements and features |
| Figma | UX/UI design workspace with structured pages |
| Markdown Documents | Agent deliverables committed via pull requests |
| Decision Log | Recorded major decisions with context and rationale |

## Agent Interaction Model

Agents read committed workspace artifacts before producing outputs. All outputs are committed back to the workspace via pull requests. No deliverable is official until committed.
