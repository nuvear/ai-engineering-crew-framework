# Auditability Policy

## Purpose

Define what evidence must exist in GitHub so decisions, deliverables, approvals, and releases can be reviewed after the fact.

## Principle

```text
If it is not in GitHub, it does not officially exist.
```

## Auditable Events

The following must leave a GitHub trace:

```text
Business intent and scope decisions
Requirement and product approvals
UX and UI approvals
Architecture approvals
Governance and risk acceptance
Build deliverables (future)
Test results (future)
Release approvals
Decision log entries
```

## Required Evidence by Phase

| Phase | Minimum Evidence |
|---|---|
| Requirements | Requirement spec, acceptance criteria, approval record |
| Product | Product plan, MVP scope, approval record |
| UX/UI | UX plan, Figma links, approval record |
| Architecture | Architecture blueprint, review notes, approval record |
| Governance | Governance review, risk classification, risk acceptance |
| Build (future) | PR history, linked issues, test evidence |
| Release | Gate 6 checklist, release notes, rollback plan |

## Evidence Quality Rules

```text
Every deliverable links to a business goal or requirement ID
Every approval is recorded via PR review, issue status, or decision log
Every major risk has an owner and acceptance record
Every exception is documented with reason and follow-up action
```

## Governance Agent Responsibilities

The Governance Agent defines:

- What evidence is required for the project's risk level
- What is missing before build authorization
- What must be collected before Gate 6 release approval
- What the Human Decision Approver must review at each checkpoint

## Audit Package for Human Review

For each governance review, provide:

```text
List of approved artifacts reviewed
Risk register summary
Open risks and accepted risks
Missing evidence blocking progress
Recommended human decisions
```

## Retention

Project audit evidence remains in GitHub for the life of the repository unless a separate retention policy applies. Do not rely on agent chat history as audit evidence.

## Non-Compliance Escalation

If required evidence is missing:

1. Document the gap in GitHub
2. Block the next phase until resolved or explicitly accepted as residual risk
3. Escalate Level 3 and Level 4 gaps to the Human Decision Approver immediately
