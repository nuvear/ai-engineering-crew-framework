# DEC-008 - QA Agent As Independent Validation Before Release

## Status

Accepted

## Date

2026-06-12

## Context

After Critic Agent setup, the framework needs an independent validation function before
future DevOps and release preparation. Critic Agent reviews Builder outputs, but QA
Agent must validate behavior against approved requirements, acceptance criteria,
governance conditions, and release-readiness expectations.

The framework must preserve separation between implementation, review, QA validation,
deployment preparation, release approval, and human decision rights.

## Options Considered

1. **Critic Agent performs QA validation** - Rejected: weak separation between review
   and validation
2. **QA Agent as independent validation before DevOps** - Selected
3. **Wait for DevOps Agent to validate release readiness** - Rejected: DevOps should
   receive QA evidence, not unvalidated implementation output

## Decision

Define QA Agent as an independent validation agent after Critic Agent and before future
DevOps Agent.

QA Agent validates approved requirement acceptance criteria, product scope conformance,
UX/UI acceptance scenarios when applicable, architecture constraints relevant to test
behavior, governance conditions, functional correctness, regression risk, edge cases,
negative paths, test coverage sufficiency, defect evidence, release validation
readiness, and QA-to-DevOps handover readiness.

QA Agent must not implement fixes, merge pull requests, deploy code, approve final
release, replace Critic Agent, replace DevOps Agent, replace Governance Agent, or
replace Human Decision Approver approval.

## Consequences

- Reviewed Builder output receives independent QA validation before DevOps handover.
- Defect severity is standardized from Level 1 through Level 4.
- Blocking defects return to Builder Agent for correction.
- QA evidence becomes part of Gate 6 release-readiness evidence.
- DevOps Agent remains a future deployment preparation role.
- Human Decision Approver approval remains the final release authority.
