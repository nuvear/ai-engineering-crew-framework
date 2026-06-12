# End-to-End Workflow

## Current Workflow

This documents the workflow through QA Agent setup as an independent validation
operating model. It does not authorize application implementation or release without the
required approvals, governance acceptance, Builder discipline, Critic review, QA
validation, pull request controls, and Human Decision Approver release approval.

```text
1. Human creates Business Intent.
2. Enterprise Architect Agent reviews intent and activates Environment Engineering Agent.
3. Environment Engineering Agent prepares GitHub, Figma, templates, project board, and environment standards.
4. Requirement Agent creates Requirement Specification.
5. Human approves requirements.
6. Product Manager Agent creates Product Plan and MVP Scope.
7. Human approves product scope.
8. UX/UI Agent creates wireframes and sample data.
9. Human approves UX.
10. UX/UI Agent applies brand guidance and creates UI.
11. Human approves UI.
12. Enterprise Architect Agent uses approved requirements, product plan, and UX/UI handover to prepare architecture.
13. Human approves architecture.
14. Governance Agent classifies risk and defines required controls.
15. Human accepts, conditionally accepts, or rejects governance conditions.
16. Builder Agent prepares governed build plans and implementation tasks only for approved, traceable work.
17. Critic Agent independently reviews Builder Agent outputs before QA handover.
18. QA Agent validates reviewed implementation work before future DevOps preparation.
```

## Step-by-Step Detail

### Step 1: Business Intent

The Human Decision Approver creates a Business Intent document using the
[business intent template](../07-templates/business-intent-template.md) and opens a
GitHub issue.

### Step 2: Enterprise Architect Review

The Enterprise Architect Agent reviews intent, identifies risks, recommends agent
activation sequence, and activates the Environment Engineering Agent.

### Step 3: Environment Setup

The Environment Engineering Agent prepares the full collaboration workspace and produces
the Gate 0 Environment Readiness checklist. Human approves Gate 0.

### Step 4-5: Requirements

The Requirement Agent creates a Requirement Specification with IDs, acceptance criteria,
and scope boundaries. Human approves Gate 1.

### Step 6-7: Product Planning

The Product Manager Agent creates Product Plan, MVP scope, feature priority matrix, and
success metrics. Human approves Gate 2.

### Step 8-9: UX Design

The UX/UI Agent (Mode 1: Experience Design) creates personas, journeys, wireframes,
sample data, and acceptance scenarios in Figma and GitHub. Human approves Gate 3.

### Step 10-11: UI Design

The UX/UI Agent (Mode 2: Visual Design) applies brand guidance and creates high-fidelity
UI, components, and developer handoff. Human approves Gate 4.

### Step 12: Architecture Preparation

The Enterprise Architect Agent synthesizes approved requirements, product plan, and
UX/UI handover into an architecture blueprint. Human approves Gate 5.

### Step 13-15: Governance Review

The Governance Agent classifies risk, defines required controls, and prepares the Human
Decision Approver governance package. Builder Agent must not begin implementation until
the Human Decision Approver accepts the required governance conditions.

### Step 16: Builder Preparation

The Builder Agent verifies approvals, prepares a Build Plan, breaks approved work into
implementation tasks, documents traceability, and prepares pull request and
Builder-to-Critic handover materials. Builder Agent must not approve, merge, or deploy
its own work.

### Step 17: Critic Review

The Critic Agent independently reviews Builder Agent outputs for requirement
traceability, product scope conformance, UX/UI handover conformance when applicable,
architecture conformance, governance conformance, code quality, maintainability,
security concerns, reliability concerns, test evidence sufficiency, pull request
readiness, known limitations, and unresolved risks.

Critic Agent may send required corrections back to Builder Agent or prepare a
Critic-to-QA handover when findings do not block QA readiness. Critic Agent must not
implement fixes, approve final merge, deploy code, or replace QA Agent.

### Step 18: QA Validation

The QA Agent validates reviewed implementation work after Critic Agent review. QA
validates approved requirement acceptance criteria, product scope conformance, UX/UI
acceptance scenarios when applicable, architecture constraints relevant to behavior,
governance conditions, functional correctness, regression risk, edge cases, negative
paths, test coverage sufficiency, defect evidence, release validation readiness, and
QA-to-DevOps handover readiness.

QA Agent may send defects back to Builder Agent when correction is required or prepare a
QA-to-DevOps handover when QA findings do not block release preparation. QA Agent must
not implement fixes, merge pull requests, deploy code, approve final release, or replace
Critic Agent, DevOps Agent, Governance Agent, or Human Decision Approver approval.

## Future Workflow Extensions

Future workflow extensions add DevOps deployment, documentation, and Gate 6 release
approval.
