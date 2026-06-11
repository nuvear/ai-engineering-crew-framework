# AI Usage Policy

## Purpose

Define practical boundaries for AI tool and agent use so the Human Decision Approver
understands what AI is doing, what data it may access, and what decisions must remain
human-owned.

## Scope

Applies to all AI Engineering Crew agents, AI-assisted development tools, and project
workspaces documented in GitHub.

## Principles

```text
AI assists structured execution; humans own judgment, risk, and final approval.
AI must not silently expand scope, data use, or release authority.
Every AI usage pattern must be documented and reviewable in GitHub.
```

## Allowed Uses

| Use Category                           | Examples                                  | Typical Risk Level |
| -------------------------------------- | ----------------------------------------- | ------------------ |
| Documentation drafting                 | Requirements, plans, governance reviews   | Level 1-2          |
| Design support                         | Wireframes, UX narratives, handover notes | Level 2            |
| Architecture analysis                  | Blueprint drafts, integration review      | Level 2-3          |
| Code assistance (future Builder phase) | Implementation under approved scope       | Level 3-4          |

## Prohibited Uses

```text
Using unapproved AI tools on production credentials or secrets
Sending restricted or confidential data to unapproved external models
Allowing AI to make final business, legal, or release decisions
Using AI to bypass approval gates or governance controls
Autonomous deployment or production changes without human approval
```

## AI Usage Declaration Requirement

Every project must maintain an AI Usage Declaration using
`07-templates/ai-usage-declaration-template.md`.

The declaration must list:

```text
Tools and agents used
Purpose of each tool
Data accessed by each tool
Human review requirements
Restrictions and escalation triggers
```

## Human-Owned Decisions

These decisions must never be delegated to AI:

```text
Risk acceptance
Budget approval
Scope approval
Architecture approval
UX approval
Release go/no-go
Final accountability
Regulatory or legal acceptance
```

## Governance Agent Responsibilities

The Governance Agent reviews AI usage for each project and confirms:

- [ ] Tools are appropriate for the risk level
- [ ] Data access is justified and classified
- [ ] Human review points are defined
- [ ] Restrictions are documented in GitHub

## Evidence Requirements

```text
AI Usage Declaration committed to docs/06-governance/
Linked requirement IDs for AI-assisted deliverables
PR records showing human review of AI-generated outputs
Decision log entries for AI boundary exceptions
```

## Escalation

Escalate to the Human Decision Approver when:

- AI tools require access to sensitive or regulated data
- A new AI tool is introduced mid-project
- AI output conflicts with approved requirements or policy
- Risk level increases due to AI usage changes
