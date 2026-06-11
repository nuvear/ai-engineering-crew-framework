# DEC-003: Two-Phase UX/UI Process

## Decision ID

DEC-003

## Decision Title

Two-Phase UX/UI Process

## Date

2026-01-10

## Decision Owner

Human Decision Approver

## Prepared By

UX/UI Agent

## Reviewed By

Product Manager Agent, Enterprise Architect Agent

## Context

When UX and UI design happen simultaneously, visual polish can hide broken workflows.
Humans approve screens that look good but have unusable flows.

## Options Considered

1. **Combined UX/UI in single phase** — Rejected: visual design masks workflow problems
2. **UX only, no UI phase** — Rejected: developers need visual design specifications
3. **Two phases: Experience Design first, Visual Design second** — Selected: workflow
   validation before visual polish

## Decision

UX/UI Agent operates in two phases: Experience Design first, Visual Design second.

## Reason

Wireframes and user flows must be approved before applying brand and high-fidelity UI
design. This prevents premature visual design and reduces rework.

## Impact

- UX/UI Agent system instruction defines Mode 1 (UX) and Mode 2 (UI)
- Gate 3 (UX Approval) must pass before Mode 2 begins
- Gate 4 (UI Approval) covers visual design separately
- Figma page structure separates wireframes (page 04) from UI design (page 06)

## Follow-up Action

Update approval gates, UX/UI Agent documentation, and test plans to enforce two-phase
process.
