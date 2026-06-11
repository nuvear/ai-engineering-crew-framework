# AI Engineering Crew Operating Model

## Overview

The AI Engineering Crew Operating Model defines how a Human Decision Approver works with a structured set of AI agents to deliver software solutions with full traceability, governance, and business alignment.

## Operating Flow

```text
Human Decision Approver
        ↓
Enterprise Architect Agent
        ↓
Environment Engineering Agent
        ↓
GitHub + Figma Collaboration Workspace
        ↓
Requirement Agent
        ↓
Product Manager Agent
        ↓
UX/UI Agent
        ↓
Enterprise Architect Agent
        ↓
Future: Governance, Builder, Critic, QA, DevOps, Documentation
```

## Phase Descriptions

### Phase 1: Intent and Orchestration

The Human Decision Approver articulates business intent. The Enterprise Architect Agent reviews intent, assesses feasibility, identifies risks, and recommends which agents to activate and in what order.

### Phase 2: Environment Readiness

The Environment Engineering Agent prepares GitHub repository, Project Board, labels, issue templates, PR template, CODEOWNERS, branching strategy, Figma project, and development environment standards. Gate 0 must pass before requirements work begins.

### Phase 3: Requirements

The Requirement Agent converts business intent into structured, traceable requirements with IDs, acceptance criteria, and scope boundaries. Gate 1 requires human approval.

### Phase 4: Product Planning

The Product Manager Agent converts approved requirements into MVP scope, feature priorities, release plan, and success metrics. Gate 2 requires human approval.

### Phase 5: Experience and Interface Design

The UX/UI Agent operates in two modes: Experience Design (wireframes, flows, sample data) then Visual Design (brand, components, high-fidelity UI). Gates 3 and 4 require human approval between modes.

### Phase 6: Architecture

The Enterprise Architect Agent uses approved requirements, product plan, and UX/UI handover to prepare the architecture blueprint. Gate 5 requires human approval.

### Future Phases

Governance review, build, critic review, QA testing, deployment, documentation, and release (Gate 6) will be added in subsequent framework versions.

## Collaboration Workspace

The workspace (GitHub + Figma) is central, not optional. All agents read from and write to the workspace. Agent chat output is temporary until committed.

## Human Accountability

The Human Decision Approver retains final accountability at every gate. Agents prepare decisions; the human approves them.
