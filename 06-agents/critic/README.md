# Critic Agent

## Overview

The Critic Agent is an independent review agent. It reviews Builder Agent outputs for
correctness, traceability, maintainability, architecture conformance, governance
conformance, test evidence sufficiency, and readiness for QA.

The Critic Agent is not a Builder Agent extension and is not a QA replacement. It must
not implement fixes, approve its own findings, merge pull requests, deploy code, or
replace Human Decision Approver approval.

## Files in This Folder

| File                    | Purpose                                           |
| ----------------------- | ------------------------------------------------- |
| `agent-purpose.md`      | Defines what this agent owns and does not own     |
| `system-instruction.md` | Exact system instruction for agent configuration  |
| `setup-guide.md`        | Step-by-step setup guidance                       |
| `test-plan.md`          | Validation prompts and success criteria           |
| `output-template.md`    | Standard output structure for Critic deliverables |
| `handover-contracts.md` | Inputs, outputs, and handover obligations         |

## Related Framework Documents

- [Critic Review Policy](../../05-policies/critic-review-policy.md)
- [Review Separation Policy](../../05-policies/review-separation-policy.md)
- [Pull Request Policy](../../05-policies/pull-request-policy.md)
- [Code Change Control Policy](../../05-policies/code-change-control-policy.md)
- [Definition of Done](../../05-policies/definition-of-done.md)
- [Builder Handover Contracts](../builder/handover-contracts.md)

## Review Constraint

Critic Agent reviews Builder Agent outputs after Builder handover and before QA
handover. It may identify findings and required corrections, but it must not implement
fixes or merge the pull request it reviews.

## QA Constraint

Critic Agent does not replace QA Agent. It prepares a Critic-to-QA handover only when
review findings do not block QA readiness.
