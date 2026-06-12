# Approval Gates Overview

## Purpose

Approval gates are mandatory checkpoints where the Human Decision Approver reviews agent
deliverables and makes go / no-go decisions before the project proceeds.

## Gate Summary

| Gate | Name                   | Prepared By                                                                                                                                   | Approved By             |
| ---- | ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------- |
| 0    | Environment Readiness  | Environment Engineering Agent                                                                                                                 | Human Decision Approver |
| 1    | Requirement Approval   | Requirement Agent                                                                                                                             | Human Decision Approver |
| 2    | Product Scope Approval | Product Manager Agent                                                                                                                         | Human Decision Approver |
| 3    | UX Approval            | UX/UI Agent (Experience Design Mode)                                                                                                          | Human Decision Approver |
| 4    | UI Approval            | UX/UI Agent (Visual Design Mode)                                                                                                              | Human Decision Approver |
| 5    | Architecture Approval  | Enterprise Architect Agent                                                                                                                    | Human Decision Approver |
| 6    | Release Approval       | Governance Agent for governance evidence; QA Agent for validation evidence; DevOps and Documentation as future release execution contributors | Human Decision Approver |

## Gate Structure

Each gate document contains:

```text
Purpose
Prepared by
Reviewed by
Approved by
Required artifacts
Approval checklist
Possible decisions
Proceed condition
Stop condition
```

## Principle

```text
If it is not approved, it should not be merged.
```

No agent may proceed to the next phase until the relevant gate is approved by the Human
Decision Approver.

## Build Authorization Control

Builder Agent setup does not create a new approval gate. It adds a controlled
implementation-support role that can begin implementation only after:

- Requirement approval exists
- Product scope approval exists
- UX/UI handover exists when user experience is affected
- Architecture approval exists
- Governance Agent risk classification is complete
- Human Decision Approver has accepted required governance conditions

Builder Agent must not approve or merge its own pull request.

## Critic Review Discipline

Critic Agent setup does not create a new approval gate. It adds an independent review
discipline between Builder Agent and QA Agent.

Critic Agent reviews Builder outputs for:

- Requirement traceability
- Product scope conformance
- UX/UI handover conformance when applicable
- Architecture conformance
- Governance condition conformance
- Code quality, maintainability, reliability, and security concerns
- Test evidence sufficiency
- Pull request readiness

Critic review may block QA handover, but it does not replace Human Decision Approver
approval and does not replace QA Agent execution.

## QA Validation Discipline

QA Agent setup does not create a new approval gate. It adds independent validation
discipline after Critic Agent review and before future DevOps preparation.

QA Agent validates:

- Approved requirement acceptance criteria
- Product scope conformance
- UX/UI acceptance scenarios when applicable
- Architecture constraints relevant to test behavior
- Governance conditions that affect validation
- Functional correctness, regression risk, edge cases, and negative paths
- Test coverage sufficiency
- Defect evidence
- Release validation readiness
- QA-to-DevOps handover readiness

QA validation becomes required release-readiness evidence for Gate 6, but Gate 6 Release
Approval remains owned by the Human Decision Approver.
