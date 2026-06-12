# Human Decision Approver

## Role Definition

The Human Decision Approver is the business-oriented leader who owns intent, value,
priority, risk, and final approval for the software solution. They are the Business
Sponsor, Product Owner, Decision Approver, Value Owner, and Final Accountability Holder.

## What the Human Owns

```text
Business objective
Scope approval
Budget approval
Priority decisions
Risk acceptance
UX approval
Architecture approval
Go / no-go decisions
Final accountability
```

## What the Human Approves

```text
The human approves business decisions, not raw source code.
```

Specifically, the human approves:

| Decision Area   | Example                                                           |
| --------------- | ----------------------------------------------------------------- |
| Business intent | "Yes, build an inventory management system"                       |
| Requirements    | "These requirements capture what we need"                         |
| Product scope   | "This MVP scope is acceptable"                                    |
| UX wireframes   | "These user flows work for our users"                             |
| UI design       | "This visual design matches our brand"                            |
| Architecture    | "This architecture approach is acceptable for our risk tolerance" |
| Release         | "We are ready to go live"                                         |

## What the Human Does Not Do

- Write application code
- Configure development tools (agents handle this with human approval of standards)
- Line-by-line code review or QA execution (Critic Agent handles review; QA Agent
  handles validation)
- Bypass approval gates

## Decision Recording

Every major human decision must be recorded in GitHub - either as an approval comment on
a pull request, an issue status change, or a decision log entry.

## Relationship to Agents

Agents prepare structured recommendations, trade-off analyses, and decision packages.
The human evaluates these in business terms and approves, rejects, or requests revision.
The human never needs to understand implementation details to make valid decisions -
agents must explain technical concepts in business-friendly language first.
