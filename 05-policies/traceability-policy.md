# Traceability Policy

## Full Traceability Chain

```text
Business Goal -> Requirement -> Feature -> UX Flow -> Architecture Decision -> Governance Control -> Build Item -> Critic Finding -> QA Test Case -> Defect -> Release Evidence
```

## Current Coverage

For the current framework state, traceability must cover:

```text
Business Goal -> Requirement -> Feature -> UX Flow -> Architecture Handover -> Governance Control -> Build Item -> Critic Finding -> QA Test Case -> Defect
```

## Traceability Requirements

| Link                         | Requirement                                               |
| ---------------------------- | --------------------------------------------------------- |
| Business Goal -> Requirement | Every requirement ID references a business goal           |
| Requirement -> Feature       | Every feature ID references one or more requirement IDs   |
| Feature -> UX Flow           | Every user flow references product features               |
| UX Flow -> Architecture      | Architecture blueprint references approved UX/UI handover |
| Architecture -> Governance   | Governance review references approved architecture        |
| Governance -> Build Item     | Every build item references governance conditions         |
| Build Item -> Critic Finding | Critic findings reference affected build items and files  |
| Build Item -> QA Test Case   | QA test cases reference requirements and build evidence   |
| QA Test Case -> Defect       | Every defect references failed test cases or criteria     |
| Defect -> Release            | Release evidence references QA results and defect status  |

## Verification

Traceability checks are part of the testing policy for documentation deliverables.
Reviewers must verify links before approving at each gate.
