# Workspace Source of Truth Policy

## Policy Statements

```text
GitHub is the official project memory.
Figma is the official design workspace.
Agent chat output is temporary until committed.
Human decisions must be recorded in GitHub.
Agent handovers must be committed as markdown.
```

## GitHub as Source of Truth

All official project artifacts — requirements, product plans, architecture, decisions,
approval records — must exist in GitHub. Version history, pull request reviews, and
issue tracking provide auditability.

## Figma as Design Workspace

UX/UI design work happens in Figma. GitHub stores links to Figma files, approval notes,
UX rationale, sample data definitions, and design handover documents.

## Agent Chat Is Temporary

Conversations with AI agents in Gemini Enterprise or other tools are working sessions.
Outputs become official only when committed to GitHub via pull request.

## Human Decision Recording

Every human approval or rejection at an approval gate must be recorded — as a PR review
comment, issue status change, or decision log entry.

## Handover Commit Requirement

When one agent hands off to another, the handover artifact (requirement spec, product
plan, UX handover, etc.) must be committed to the appropriate `docs/` directory before
the next agent activates.
