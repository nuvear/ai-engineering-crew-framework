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
| Code (Builder-controlled) | Unit tests, build, lint, security, traceability        |
