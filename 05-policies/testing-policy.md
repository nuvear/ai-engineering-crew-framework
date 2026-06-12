# Testing Policy

## Principle

Not all testing is code testing. The framework distinguishes between documentation
deliverable testing and future code deliverable testing.

## Documentation Deliverable Testing

For documentation deliverables, testing means:

```text
Traceability check
Completeness check
Contradiction check
Scope creep check
Human decision check
Approval readiness check
```

## Builder Code Deliverable Testing

For Builder-controlled code deliverables, testing means:

```text
Unit tests
Build check
Linting
Security check
Architecture conformance review
Governance condition review
Traceability review
```

## Critic Review Evidence

Critic Agent reviews Builder test evidence for sufficiency before QA handover. Critic
review may identify missing, weak, or insufficient Builder test evidence.

## QA Validation Evidence

QA Agent independently validates reviewed implementation work after Critic review. QA
validation includes test planning, test case definition, functional validation,
regression validation, edge case and negative path validation, acceptance criteria
coverage, defect evidence, governance validation notes, and QA pass/fail recommendation.

QA validation evidence contributes to Gate 6 release readiness, but QA Agent does not
approve final release.

## When Testing Applies

| Deliverable Type          | Testing Method                                         |
| ------------------------- | ------------------------------------------------------ |
| Business Intent           | Completeness, human decision check                     |
| Requirement Specification | Traceability, completeness, scope creep                |
| Product Plan              | Traceability to requirements, scope separation         |
| UX Wireframes             | Flow completeness, sample data, feature linkage        |
| UI Design                 | Wireframe conformance, brand consistency               |
| Architecture Blueprint    | Requirement coverage, NFR coverage, risk documentation |
| Governance Review         | Risk coverage, control evidence, approval readiness    |
| Builder Build Plan        | Traceability, testability, scope and governance checks |
| Critic Review             | Traceability, conformance, test evidence, QA readiness |
| QA Test Plan              | Acceptance criteria, risk, coverage, validation scope  |
| QA Execution Report       | Test results, defects, coverage, release readiness     |
| Code (Builder-controlled) | Unit tests, build, lint, security, traceability        |
