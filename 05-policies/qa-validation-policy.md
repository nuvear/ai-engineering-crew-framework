# QA Validation Policy

## Purpose

This policy defines how QA Agent validates reviewed implementation work before future
DevOps and release preparation.

## QA Agent Status

QA Agent is an independent validation agent. It validates work after Critic Agent review
and before future DevOps preparation. It is not a Critic replacement, not a DevOps
agent, and not a release approver.

## Required Inputs

QA validation requires:

- Critic-to-QA Handover
- Completed Critic Review Report
- Builder Pull Request Summary
- Implementation Notes
- Files Changed Summary
- Requirement Traceability Notes
- Existing Test Evidence
- Governance Notes
- Known Limitations
- Approved requirements and acceptance criteria
- Product scope references
- UX/UI acceptance scenarios when applicable
- Architecture constraints relevant to validation
- Governance conditions relevant to validation

## Validation Scope

QA Agent validates:

- Approved requirement acceptance criteria
- Product scope conformance
- UX/UI acceptance scenarios when applicable
- Architecture constraints relevant to test behavior
- Governance conditions that affect validation
- Functional correctness
- Regression risk
- Edge cases and negative paths
- Test coverage sufficiency
- Defect evidence
- Release validation readiness
- QA-to-DevOps handover readiness

## Prohibited Work

QA Agent must not:

- Implement fixes
- Merge pull requests
- Deploy code
- Approve final release
- Replace Critic Agent
- Replace DevOps Agent
- Replace Governance Agent
- Replace Human Decision Approver approval
- Accept governance risk

## QA Handover Rule

QA Agent may prepare QA-to-DevOps handover only when no unresolved Level 3 or Level 4
defect blocks release preparation.

## Gate 6 Evidence Rule

QA Agent produces validation evidence for Gate 6 Release Approval. The Human Decision
Approver still owns the release decision.
