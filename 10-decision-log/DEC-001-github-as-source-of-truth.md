# DEC-001: GitHub as Source of Truth

## Decision ID

DEC-001

## Decision Title

GitHub as Source of Truth

## Date

2026-01-01

## Decision Owner

Human Decision Approver

## Prepared By

Enterprise Architect Agent

## Reviewed By

Environment Engineering Agent

## Context

The AI Engineering Crew Framework requires a permanent, version-controlled collaboration
workspace. Agent conversations are ephemeral and cannot serve as project memory.

## Options Considered

1. **Agent chat history as source of truth** — Rejected: no versioning, no review, no
   traceability
2. **Shared document platform (Google Docs, Notion)** — Rejected: lacks PR workflow,
   branch protection, and developer integration
3. **GitHub as source of truth** — Selected: versioning, PRs, issues, project board,
   CODEOWNERS, decision history

## Decision

GitHub is the official source of truth for the AI Engineering Crew Framework and for
future project workspaces.

## Reason

Agent conversations are temporary. GitHub provides versioning, traceability, review,
pull requests, and decision history.

## Impact

- All agent deliverables must be committed to GitHub via pull requests
- Figma links and approval records are stored in GitHub
- Agent chat output is temporary until committed
- Branch protection and CODEOWNERS enforce review discipline

## Follow-up Action

Environment Engineering Agent to configure GitHub workspace with templates, labels, and
branch protection as part of Gate 0.
