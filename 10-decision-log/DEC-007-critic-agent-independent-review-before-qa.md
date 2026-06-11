# DEC-007 - Critic Agent As Independent Review Before QA

## Status

Accepted

## Date

2026-06-12

## Context

After Builder Agent setup, the framework needs an independent review function before QA
Agent setup. Builder Agent can prepare approved implementation work, but it must not be
the sole reviewer of its own output.

The framework must preserve separation between implementation, review, QA execution,
deployment, release approval, and human decision rights.

## Options Considered

1. **Builder self-review only** - Rejected: weak separation of duties
2. **Critic Agent as independent review before QA** - Selected
3. **Wait for QA Agent to perform all review** - Rejected: QA should receive reviewed
   work, not unreviewed Builder output

## Decision

Define Critic Agent as an independent review agent after Builder Agent and before QA
Agent.

Critic Agent reviews Builder outputs for requirement traceability, product scope
conformance, UX/UI handover conformance when applicable, architecture conformance,
governance conformance, code quality, maintainability, security concerns, reliability
concerns, test evidence sufficiency, pull request readiness, and unresolved risks.

Critic Agent must not implement fixes, approve final merge, deploy code, replace QA
Agent, or replace Human Decision Approver approval.

## Consequences

- Builder output receives independent review before QA handover.
- Finding severity is standardized from Level 1 through Level 4.
- Blocking findings return to Builder Agent for correction.
- QA Agent remains a future execution role.
- Human Decision Approver approval remains the final authority where required.
