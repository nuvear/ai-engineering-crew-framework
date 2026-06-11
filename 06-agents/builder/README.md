# Builder Agent

## Overview

The Builder Agent is a governed implementation-support agent. It helps translate
approved, traceable work into implementation tasks, code changes, tests, pull request
summaries, and handover notes.

The Builder Agent is not an autonomous software engineer. It must operate under approved
requirements, approved product scope, approved UX/UI handover when applicable, approved
architecture, completed governance risk classification, and Human Decision Approver
acceptance of required governance conditions.

## Files in This Folder

| File                    | Purpose                                            |
| ----------------------- | -------------------------------------------------- |
| `agent-purpose.md`      | Defines what this agent owns and does not own      |
| `system-instruction.md` | Exact system instruction for agent configuration   |
| `setup-guide.md`        | Step-by-step setup guidance                        |
| `test-plan.md`          | Validation prompts and success criteria            |
| `output-template.md`    | Standard output structure for Builder deliverables |
| `handover-contracts.md` | Inputs, outputs, and handover obligations          |

## Related Framework Documents

- [Builder Implementation Policy](../../05-policies/builder-implementation-policy.md)
- [Code Change Control Policy](../../05-policies/code-change-control-policy.md)
- [Testing Policy](../../05-policies/testing-policy.md)
- [Traceability Policy](../../05-policies/traceability-policy.md)
- [Governance Agent Handover Contracts](../governance/handover-contracts.md)
- [Approval Policy](../../05-policies/approval-policy.md)

## Governance Constraint

Builder Agent must not begin implementation unless Governance Agent has completed risk
classification and the Human Decision Approver has accepted the required governance
conditions.

## Merge Constraint

Builder Agent must not approve or merge its own pull requests. Human approval and the
required review path remain mandatory.
