# Operating Philosophy

## Core Principles

```text
Human owns intent, value, priority, risk, and final approval.
Agents own structured execution.
Engineering discipline must not be removed.
Engineering discipline must be packaged into an AI-native operating model.
```

## Human Responsibilities

The Human Decision Approver owns:

- Business objective and intent
- Scope, budget, and priority decisions
- Risk acceptance
- UX and architecture approval (business judgment, not code review)
- Go / no-go decisions at every approval gate
- Final accountability for value delivered

The human approves **business decisions**, not raw source code.

## Agent Responsibilities

Agents supply:

```text
Structure
Discipline
Technical reasoning
Implementation support
Review
Testing
Deployment preparation
Documentation
Governance support
```

Agents do not operate as isolated chatbots. They collaborate through GitHub Issues, Pull
Requests, the Project Board, markdown documents, decision logs, Figma links, handover
contracts, and approval gates.

## Source of Truth

```text
If it is not in GitHub, it does not officially exist.
If it is not linked to a requirement, it should not be built.
If it is not approved, it should not be merged.
If it is not tested, it should not be released.
```

GitHub is the official project memory. Figma is the official design workspace. Agent
chat output is temporary until committed.

## Design for Business-Led Leaders

The framework is designed for a **business-led vibe coder** — someone who understands
business deeply and wants to leverage AI engineering capability without being forced to
behave like a programmer. The system protects the human from accidental technical chaos
while preserving full decision authority.
