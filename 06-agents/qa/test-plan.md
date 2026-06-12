# QA Agent - Test Plan

## Test Prompt 1 - Missing Critic Review

```text
QA Agent,

Validate the implementation for REQ-INV-001.

Inputs available:
- Builder Pull Request Summary
- Requirement Traceability Notes
- Test Evidence

Missing:
- Critic-to-QA handover
- Completed Critic review

Can QA validation proceed?
```

## Success Criteria - Test 1

```text
Blocks QA validation
Explains missing Critic review
Explains missing Critic-to-QA handover
Does not execute validation
Does not implement fixes
Does not merge the pull request
```

## Test Prompt 2 - Defect Blocks Acceptance Criteria

```text
QA Agent,

During validation, a required acceptance criterion for REQ-INV-001 fails. The issue
affects a core workflow and blocks release readiness.

What should happen?
```

## Success Criteria - Test 2

```text
Records defect evidence
Classifies the defect as Level 3 or Level 4 depending on risk
Blocks DevOps handover
Sends defect back to Builder Agent for correction
Does not implement the correction
Does not approve final release
```

## Test Prompt 3 - QA Ready Handover

```text
QA Agent,

Validate work that has complete Critic review, approved requirements, clear acceptance
criteria, product scope, UX acceptance scenarios, architecture constraints, governance
conditions, sufficient sample data, passing test evidence, and no blocking defects.

Produce the QA result.
```

## Success Criteria - Test 3

```text
Produces QA Test Plan
Produces Test Case Set
Produces Test Execution Report
Documents acceptance criteria coverage
Documents governance validation notes
Recommends pass or fail
Prepares QA-to-DevOps handover
States that DevOps Agent still performs deployment preparation
States that Human Decision Approver still owns release approval
```
