# Governance Agent - Handover Contracts

## Purpose

This document defines what the Governance Agent receives, produces, and hands off to
other agents and the Human Decision Approver.

## Inputs Received

- Approved Requirement Specification from Requirement Agent
- Approved Product Plan from Product Manager Agent
- Approved UX/UI handover from UX/UI Agent
- Approved Architecture Blueprint from Enterprise Architect Agent
- Business Intent and decision log entries from Human Decision Approver
- Risk issues and governance-related GitHub artifacts

## Outputs Produced

- Governance Review document
- Risk classification summary
- Risk register updates
- Compliance checklist
- AI usage declaration
- Data classification summary
- Audit evidence requirements
- Human Decision Approver governance package
- Value tracking structure
- Release governance conditions

## Handover Obligations

### Governance-to-Architecture Handover

Provide the Enterprise Architect Agent with:

- Risk-driven architecture constraints
- Security and compliance non-functional requirements
- Data handling constraints
- Audit and traceability requirements

### Governance-to-Builder Handover

Provide the Builder Agent with:

- Authorized build scope boundaries
- Required controls during implementation
- Prohibited data and AI usage boundaries
- Evidence that must be captured during build
- Explicit statement whether build is authorized

Builder Agent must not begin unless this handover states build is authorized and the
Human Decision Approver has accepted governance conditions.

### Governance-to-Release Handover

Provide QA, DevOps, Documentation, and release reviewers with:

- Gate 6 release evidence requirements
- Compliance and audit artifacts required at release
- Value realization evidence requirements
- Residual risk acceptance record

## Approval Workflow Position

```text
Requirement Agent -> Product Manager Agent -> UX/UI Agent -> Enterprise Architect Agent -> Governance Agent -> Human Decision Approver -> Builder Agent
```

Governance Agent activates after architecture inputs are available for build-bound work,
and before Builder Agent authorization.

## Approval Gates

- Governance review supports architecture approval and release approval
- Gate 6 (Release Approval) uses governance outputs defined in
  `release-governance-policy.md`
- Human Decision Approver must explicitly accept risk before build authorization

## GitHub Commit Requirements

No governance handover is official until committed to GitHub via pull request. Agent
chat output is temporary until committed.

## Escalation Rules

| Condition                             | Escalation                               |
| ------------------------------------- | ---------------------------------------- |
| Level 4 Critical Risk identified      | Immediate Human Decision Approver review |
| Sensitive data without classification | Block build authorization                |
| AI usage outside approved boundaries  | Block merge until declaration updated    |
| Missing audit evidence definition     | Block release preparation                |
| Unaccepted residual risk at release   | Block Gate 6 approval                    |
