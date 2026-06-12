# Defect Management Policy

## Purpose

This policy defines how QA Agent identifies, classifies, reports, and routes defects.

## Defect Definition

A defect is any observed behavior, missing evidence, or validation result that fails an
approved acceptance criterion, governance validation condition, reliability expectation,
or release-readiness expectation.

## Defect Severity Model

| Level | Name     | Meaning                                                                                                                        |
| ----- | -------- | ------------------------------------------------------------------------------------------------------------------------------ |
| 1     | Minor    | Cosmetic, documentation, low-risk usability, or low-risk nonblocking issue                                                     |
| 2     | Moderate | Localized functional, regression, validation, or usability issue requiring correction                                          |
| 3     | Major    | Acceptance criteria failure, material regression, governance validation failure, or reliability issue blocking DevOps handover |
| 4     | Critical | Unsafe, noncompliant, data-risk, security-risk, production-impacting, or release-blocking defect                               |

## Defect Report Requirements

Every defect report must include:

- Defect ID
- Linked requirement ID
- Failed acceptance criteria or validation expectation
- Severity level
- Evidence or reproduction notes
- Impact on release readiness
- Required correction or decision
- Owner for correction
- Status

## Routing Rules

- Level 1 defects may be documented as nonblocking if accepted by the review path.
- Level 2 defects require Builder correction before release readiness unless explicitly
  deferred.
- Level 3 defects block DevOps handover until corrected or formally accepted by the
  required approver.
- Level 4 defects require Human Decision Approver visibility before work can proceed.

## QA Constraint

QA Agent reports defects and validation evidence. QA Agent must not implement fixes,
merge pull requests, deploy code, or approve final release.
