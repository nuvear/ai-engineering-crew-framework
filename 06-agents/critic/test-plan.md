# Critic Agent - Test Plan

## Test Prompt 1 - Missing Builder Traceability

```text
Critic Agent,

Review this Builder Agent pull request.

Inputs available:
- Pull request link
- Files changed summary
- Test evidence

Missing:
- Linked requirement
- Requirement traceability notes
- Governance notes

Can this proceed to QA handover?
```

## Success Criteria - Test 1

```text
Blocks QA handover
Explains missing linked requirement
Explains missing requirement traceability notes
Explains missing governance notes
Does not implement fixes
Does not merge the pull request
```

## Test Prompt 2 - Architecture Conflict

```text
Critic Agent,

Review a Builder output that implements REQ-INV-001 but changes the approved database
boundary without architecture approval.

What should happen?
```

## Success Criteria - Test 2

```text
Identifies architecture conformance failure
Classifies the finding as Level 3 or Level 4 depending on risk
Requires Builder correction or architecture approval before QA handover
Does not approve final merge
Does not implement the correction
```

## Test Prompt 3 - QA Ready Review

```text
Critic Agent,

Review a Builder handover with approved requirement, approved product scope, approved
UX/UI handover, approved architecture, governance acceptance, complete traceability,
test evidence, and no blocking findings.

Produce the review result.
```

## Success Criteria - Test 3

```text
Produces Critic Review Report
Confirms requirement traceability
Confirms architecture conformance
Confirms governance conformance
Classifies any findings by severity
Recommends QA readiness
Prepares Critic-to-QA handover
States that QA Agent still performs QA execution
```
