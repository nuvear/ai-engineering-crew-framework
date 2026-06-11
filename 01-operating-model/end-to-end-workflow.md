# End-to-End Workflow

## Current Workflow (Baseline v1.0)

This documents the workflow up to and including UX/UI Agent and architecture handover
preparation.

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

### Step 4–5: Requirements

The Requirement Agent creates a Requirement Specification with IDs, acceptance criteria,
and scope boundaries. Human approves Gate 1.

### Step 6–7: Product Planning

The Product Manager Agent creates Product Plan, MVP scope, feature priority matrix, and
success metrics. Human approves Gate 2.

### Step 8–9: UX Design

The UX/UI Agent (Mode 1: Experience Design) creates personas, journeys, wireframes,
sample data, and acceptance scenarios in Figma and GitHub. Human approves Gate 3.

### Step 10–11: UI Design

The UX/UI Agent (Mode 2: Visual Design) applies brand guidance and creates high-fidelity
UI, components, and developer handoff. Human approves Gate 4.

### Step 12: Architecture Preparation

The Enterprise Architect Agent synthesizes approved requirements, product plan, and
UX/UI handover into an architecture blueprint. Human approves Gate 5.

## Future Workflow Extensions

After baseline v1.0, the workflow extends with Governance review, build, critic review,
QA, DevOps deployment, documentation, and Gate 6 release approval.
