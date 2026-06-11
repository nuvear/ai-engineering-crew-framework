# DEC-004: Human Approval Gates

## Decision ID

DEC-004

## Decision Title

Human Approval Gates

## Date

2026-01-12

## Decision Owner

Human Decision Approver

## Prepared By

Enterprise Architect Agent

## Reviewed By

All baseline agents

## Context

The framework serves business-oriented leaders who must retain decision authority. Without explicit gates, agents may proceed through phases without human validation.

## Options Considered

1. **Agent-autonomous progression** — Rejected: removes human accountability
2. **Single approval at release only** — Rejected: scope and design errors discovered too late
3. **Mandatory gates at each phase transition** — Selected: human validates at every critical point

## Decision

Human approval gates are mandatory at environment, requirement, product scope, UX, UI, architecture, and release stages.

## Reason

The human owns business judgment, risk acceptance, value, and final accountability.

## Impact

- Seven approval gates defined (Gates 0–6)
- No agent proceeds to next phase without gate approval
- Human approves business decisions, not raw source code
- Gate documentation in `04-approval-gates/`
- Project Board statuses align with gate checkpoints

## Follow-up Action

Configure GitHub Project Board with gate-aligned statuses and gate labels. Train all agents to respect gate boundaries.
