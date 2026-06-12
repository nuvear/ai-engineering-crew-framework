# QA Agent - Handover Contracts

## Purpose

This document defines what QA Agent receives, validates, sends back for correction, and
hands forward to future DevOps.

## Inputs Received

- Critic-to-QA Handover
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

## Outputs Produced

- QA Test Plan
- Test Case Set
- Test Execution Report
- Defect Report
- Acceptance Criteria Coverage Matrix
- Regression Risk Notes
- UX Acceptance Validation Notes when applicable
- Governance Validation Notes
- QA Pass/Fail Recommendation
- QA-to-DevOps Handover

## Critic-to-QA Handover

Critic Agent must provide:

- Pull request link
- Review summary
- Requirement traceability status
- Architecture conformance status
- Governance conformance status
- Test evidence summary
- Known limitations
- Residual risks
- QA focus areas
- Confirmation that no unresolved Level 3 or Level 4 finding blocks QA

## QA-to-Builder Defect Feedback

QA Agent sends defects back to Builder Agent when correction is required. Feedback must
include:

- Defect IDs
- Severity levels
- Failed acceptance criteria
- Evidence or reproduction notes
- Required correction or clarification
- Release progression impact
- Any Human Decision Approver visibility required for Level 4 defects

## QA-to-DevOps Handover

QA Agent prepares DevOps handover only when QA findings do not block release
preparation. The handover must include:

- Pull request link
- QA result
- Acceptance criteria coverage status
- Test execution summary
- Defects resolved or deferred with approval
- Regression risk notes
- Governance validation notes
- Release validation readiness recommendation
- DevOps focus areas

## Stop Conditions

QA Agent must stop or block DevOps handover if:

- Critic review is missing
- Unresolved Level 3 or Level 4 Critic findings remain
- Requirement acceptance criteria are missing or unclear
- Test environment or sample data is insufficient
- Required test evidence is missing
- Defects block acceptance criteria
- Security, privacy, compliance, or data handling validation is unresolved
- QA-to-DevOps handover cannot be completed

## GitHub Commit Requirements

No QA deliverable is official until committed to GitHub via pull request. QA Agent must
not implement fixes, merge pull requests, deploy code, or approve final release.
