# Code Change Control Policy

## Purpose

This policy defines how code changes are controlled once Builder Agent begins governed
implementation support.

## Source of Truth

GitHub is the source of truth for code changes, implementation evidence, pull request
discussion, reviews, and approvals.

## Branching

Code changes must be made on feature branches using the documented branch naming format:

```text
agent/<agent-name>/<work-item-id>-short-description
```

## Pull Request Control

Every implementation change must enter through a pull request that includes:

- Linked requirement IDs
- Linked GitHub issue or approved work item
- Product scope reference
- Architecture reference
- Governance conditions
- Files changed summary
- Test evidence
- Known limitations
- Builder-to-Critic handover

## Review and Approval

Builder Agent must not approve or merge its own pull request.

Critic Agent must independently review Builder Agent pull requests before QA handover.
Critic Agent must not implement fixes, approve final merge, or merge the pull request it
reviews.

QA Agent must independently validate reviewed implementation work before future DevOps
handover. QA Agent must not implement fixes, merge pull requests, deploy code, or
approve final release.

Implementation pull requests require review for:

- Requirement traceability
- Product scope conformance
- Architecture conformance
- Governance condition conformance
- Test evidence
- QA validation evidence
- Security and data handling concerns
- Maintainability and reliability concerns
- Human approval where required

## Test Evidence

Code changes must include test evidence appropriate to the work. If tests cannot be run
or written, Builder Agent must document why and escalate before merge. QA Agent
validates the sufficiency of test evidence after Critic review.

## Sensitive Data Control

Builder Agent must not introduce, access, transform, or store sensitive data unless data
classification and handling rules are approved.

## Merge Control

Merge approval remains human-owned or assigned to an approved reviewer. Builder Agent,
Critic Agent, and QA Agent may prepare evidence, but they must not be the final approver
for their own work.
