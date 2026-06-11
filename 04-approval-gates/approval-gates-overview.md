# Approval Gates Overview

## Purpose

Approval gates are mandatory checkpoints where the Human Decision Approver reviews agent
deliverables and makes go / no-go decisions before the project proceeds.

## Gate Summary

| Gate | Name                   | Prepared By                                    | Approved By             |
| ---- | ---------------------- | ---------------------------------------------- | ----------------------- |
| 0    | Environment Readiness  | Environment Engineering Agent                  | Human Decision Approver |
| 1    | Requirement Approval   | Requirement Agent                              | Human Decision Approver |
| 2    | Product Scope Approval | Product Manager Agent                          | Human Decision Approver |
| 3    | UX Approval            | UX/UI Agent (Experience Design Mode)           | Human Decision Approver |
| 4    | UI Approval            | UX/UI Agent (Visual Design Mode)               | Human Decision Approver |
| 5    | Architecture Approval  | Enterprise Architect Agent                     | Human Decision Approver |
| 6    | Release Approval       | QA, DevOps, Documentation, Governance (future) | Human Decision Approver |

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
