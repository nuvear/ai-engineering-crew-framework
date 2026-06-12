# QA Agent

## Overview

The QA Agent is an independent validation agent. It validates built and reviewed work
against approved requirements, acceptance criteria, product scope, UX/UI acceptance
scenarios when applicable, architecture constraints relevant to behavior, governance
conditions, defect evidence, and release-readiness expectations.

The QA Agent is not a Critic Agent replacement, not a DevOps Agent, and not a release
approver. It must not implement fixes, merge pull requests, deploy code, approve final
release, or replace Human Decision Approver approval.

## Files in This Folder

| File                    | Purpose                                       |
| ----------------------- | --------------------------------------------- |
| `agent-purpose.md`      | Defines what this agent owns and does not own |
| `system-instruction.md` | Exact system instruction for agent setup      |
| `setup-guide.md`        | Step-by-step setup guidance                   |
| `test-plan.md`          | Validation prompts and success criteria       |
| `output-template.md`    | Standard output structure for QA deliverables |
| `handover-contracts.md` | Inputs, outputs, and handover obligations     |

## Related Framework Documents

- [QA Validation Policy](../../05-policies/qa-validation-policy.md)
- [Test Evidence Policy](../../05-policies/test-evidence-policy.md)
- [Defect Management Policy](../../05-policies/defect-management-policy.md)
- [Testing Policy](../../05-policies/testing-policy.md)
- [Review Separation Policy](../../05-policies/review-separation-policy.md)
- [Critic Handover Contracts](../critic/handover-contracts.md)

## Validation Constraint

QA Agent validates work only after Critic Agent review is complete and no unresolved
Level 3 or Level 4 Critic findings block QA.

## Release Constraint

QA Agent produces validation evidence for release readiness, but it does not approve
release. Gate 6 Release Approval remains owned by the Human Decision Approver.
