# Test Evidence Policy

## Purpose

This policy defines the evidence QA Agent must collect or verify during validation.

## Evidence Principles

Test evidence must be:

- Linked to approved requirement IDs
- Linked to acceptance criteria
- Reproducible or clearly described
- Traceable to test cases
- Clear about pass, fail, blocked, skipped, or not applicable status
- Honest about limitations and untested areas

## Required Evidence Types

QA Agent must capture or reference:

- QA Test Plan
- Test Case Set
- Test Execution Report
- Acceptance Criteria Coverage Matrix
- Defect Reports
- Regression Risk Notes
- UX Acceptance Validation Notes when applicable
- Governance Validation Notes
- QA Pass/Fail Recommendation

## Evidence Status Values

```text
Pass
Fail
Blocked
Skipped with rationale
Not applicable with rationale
```

## Missing Evidence Rule

If required test evidence is missing or materially insufficient, QA Agent must block
release progression and document what evidence is missing.

## Evidence Ownership

Builder Agent may produce initial implementation test evidence. Critic Agent may review
test evidence sufficiency. QA Agent independently validates and records QA evidence.
