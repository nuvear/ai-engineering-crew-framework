# Commit Deliverables Policy

## Core Rules

```text
No agent deliverable is official until committed to GitHub.
All deliverables must be introduced through pull requests.
Every deliverable must link to a business goal, requirement, decision, or issue.
```

## Deliverables by Agent

```text
Enterprise Architect Agent:
Architecture plans, activation plans, review notes

Environment Engineering Agent:
Environment setup docs, tool inventory, access matrix, branching strategy, CI/CD plan, secrets strategy

Requirement Agent:
Requirement specification, acceptance criteria, scope boundary, requirement handover

Product Manager Agent:
Product plan, MVP scope, roadmap, feature priority matrix, success metrics

UX/UI Agent:
Personas, user journeys, wireframes, Figma links, sample data, UI handover

Governance Agent:
Governance review, risk classification, AI usage declaration, data classification, governance handovers

Builder Agent:
Build plans, implementation tasks, files changed summary, test evidence, pull request summary, Builder-to-Critic handover

Critic Agent:
Critic review reports, traceability review, architecture conformance review, governance conformance review, findings, Critic-to-Builder feedback, Critic-to-QA handover
```

## Pull Request Requirements

Every commit of agent deliverables must include:

- Linked GitHub issue
- Agent owner identified
- Deliverable type specified
- Acceptance criteria referenced
- Test evidence (traceability, completeness, or code tests as applicable)

## Traceability

Every deliverable must trace to at least one of: business goal, requirement ID, decision
record, or GitHub issue.
