# DEC-005: Governance Agent Before Builder Agent

## Decision ID

DEC-005

## Decision Title

Governance Agent Before Builder Agent

## Date

2026-06-11

## Decision Owner

Human Decision Approver

## Prepared By

Governance Agent

## Reviewed By

Enterprise Architect Agent

## Context

Framework Baseline v1.0 documented agents through UX/UI setup. Builder Agent is the next
implementation phase, but ungoverned build work creates risk for business-oriented
approvers who must accept data use, AI boundaries, compliance exposure, and release
accountability without reading code.

## Options Considered

1. **Allow Builder Agent immediately after architecture approval** — Rejected:
   insufficient risk and evidence definition
2. **Add governance only at release** — Rejected: risks discovered too late
3. **Require Governance Agent classification and human risk acceptance before build** —
   Selected

## Decision

Governance Agent is added before Builder Agent. Builder Agent must not begin
implementation unless Governance Agent has completed risk classification and the Human
Decision Approver has accepted the required governance conditions.

## Reason

The minimum governance system must make AI-assisted software work safe, auditable, and
decision-ready before code implementation begins.

## Impact

- New agent folder: `06-agents/governance/`
- New governance policies in `05-policies/`
- New governance templates in `07-templates/`
- 4-level risk classification model adopted
- Builder Agent remains blocked until governance approval
- Gate 6 release governance connected to governance outputs
- Approval workflow extended with governance review before build

## Follow-up Action

Configure Governance Agent in Gemini Enterprise, apply governance review to the
reference project, and update approval matrix and agent topology in a future
documentation pass after Step 7 merge.
