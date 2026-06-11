# Pull Request Policy

## Requirement

Every pull request must include:

```text
Linked issue
Agent owner
Deliverable type
Files changed
Acceptance criteria
Test evidence
Risk notes
Human decision required
Approval checklist
```

## PR Template

Use `.github/PULL_REQUEST_TEMPLATE.md` for all pull requests.

## Review Process

1. Agent owner completes deliverable on feature branch
2. Agent owner opens PR with all required sections filled
3. Reviewing agent(s) verify completeness and traceability
4. Human Decision Approver approves if gate criteria are met
5. PR merges to `main`

## Implementation PR Review Discipline

Implementation pull requests prepared by Builder Agent require independent Critic Agent
review before QA handover. Critic Agent reviews traceability, scope conformance,
architecture conformance, governance conformance, code quality, test evidence, risk
notes, and QA readiness.

Critic Agent must not implement fixes, approve final merge, or merge the pull request it
reviews.

## Documentation PRs

For documentation-only deliverables, test evidence includes traceability check,
completeness check, contradiction check, scope creep check, and approval readiness
check.
