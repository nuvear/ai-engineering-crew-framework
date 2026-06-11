# DEC-006: Builder Agent as Governed Implementation Support

## Decision ID

DEC-006

## Decision Title

Builder Agent as Governed Implementation Support

## Date

2026-06-11

## Decision Owner

Human Decision Approver

## Prepared By

Enterprise Architect Agent

## Reviewed By

Governance Agent

## Context

After Governance Agent setup, the framework can define Builder Agent. The Builder Agent
introduces implementation capability, which must remain controlled by approved
requirements, product scope, UX/UI handover, architecture, governance risk
classification, and Human Decision Approver risk acceptance.

## Options Considered

1. **Autonomous coding agent** — Rejected: allows uncontrolled scope and risk
2. **Implementation-support agent under approved controls** — Selected
3. **Delay Builder Agent until Critic and QA exist** — Rejected: Builder can be defined
   now if handover and review constraints are explicit

## Decision

Builder Agent is defined as a governed implementation-support agent. It may only
implement approved, traceable work and must not begin implementation unless Governance
Agent has completed risk classification and the Human Decision Approver has accepted the
required governance conditions.

## Reason

The framework needs implementation support, but code generation must remain bounded by
human-approved scope, architecture, governance, testing, and pull request discipline.

## Impact

- New agent folder: `06-agents/builder/`
- New Builder policies in `05-policies/`
- New Builder templates in `07-templates/`
- Builder-to-Critic handover defined
- Builder Agent cannot approve or merge its own pull request
- Builder Agent cannot deploy to production
- Critic, QA, DevOps, and Documentation agents remain future steps

## Follow-up Action

Open Step 8 Builder Agent pull request for Human Decision Approver review. Do not start
application implementation until approved requirements, architecture, governance
acceptance, testing expectations, and PR review are available.
