# Governance Agent

## Overview

The Governance Agent defines the minimum enterprise risk management system required
before Builder Agent begins implementation. It helps a business-oriented Human Decision
Approver understand risks, data use, AI tool boundaries, required evidence, and release
conditions in plain language.

Governance is practical, not bureaucratic. It answers whether work can proceed safely
and what the human must approve before build, release, or deployment.

## Files in This Folder

| File                    | Purpose                                                |
| ----------------------- | ------------------------------------------------------ |
| `agent-purpose.md`      | Defines what this agent owns and does not own          |
| `system-instruction.md` | Exact system instruction for agent configuration       |
| `setup-guide.md`        | Step-by-step setup in Gemini Enterprise Agent Designer |
| `test-plan.md`          | Validation prompts and success criteria                |
| `output-template.md`    | Standard output structure for governance deliverables  |
| `handover-contracts.md` | Inputs, outputs, and handover obligations              |

## Related Framework Documents

- [AI Usage Policy](../../05-policies/ai-usage-policy.md)
- [Data Governance Policy](../../05-policies/data-governance-policy.md)
- [Auditability Policy](../../05-policies/auditability-policy.md)
- [Release Governance Policy](../../05-policies/release-governance-policy.md)
- [Value Realization Policy](../../05-policies/value-realization-policy.md)
- [Gate 6 — Release Approval](../../04-approval-gates/gate-6-release-approval.md)
- [Approval Policy](../../05-policies/approval-policy.md)

## Builder Agent Block

Builder Agent must not begin implementation unless Governance Agent has completed risk
classification and the Human Decision Approver has accepted the required governance
conditions.
