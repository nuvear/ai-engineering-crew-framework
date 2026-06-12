# Agent Hierarchy

## Hierarchy Levels

```text
Level 1: Human Decision Approver
Level 2: Enterprise Architect Agent
Level 3: Environment Engineering Agent
Level 4: Planning and Design Agents
Level 5: Governance Agent
Level 6: Build and Review Agents
Level 7: Validation Agent
Level 8: Deployment and Knowledge Agents
```

## Level 1: Human Decision Approver

Final accountability holder. Approves business decisions at every gate.

## Level 2: Enterprise Architect Agent

Chief orchestrator. Owns solution blueprint, architecture decisions, agent coordination,
and architecture review.

## Level 3: Environment Engineering Agent

Digital construction site manager. Prepares GitHub, Figma, project board, templates,
branching strategy, CI/CD foundation, and environment standards.

## Level 4: Planning and Design Agents (Baseline v1.0)

```text
Enterprise Architect Agent
Environment Engineering Agent
Requirement Agent
Product Manager Agent
UX/UI Agent
```

### Requirement Agent

Converts business intent into structured requirements.

### Product Manager Agent

Converts approved requirements into product plan and MVP scope.

### UX/UI Agent

Designs user experience and interface in two phases (UX then UI).

## Level 5: Governance Agent (Step 7)

Defines risk classification, governance controls, AI usage review, data governance
review, release evidence expectations, and the human risk acceptance package.

## Level 6: Build and Review Agents (Steps 8-9)

Builder Agent converts approved, governed work into build plans, implementation tasks,
testable code changes, pull request summaries, and Builder-to-Critic handovers. It
cannot approve or merge its own work.

Critic Agent independently reviews Builder outputs for traceability, architecture
conformance, governance conformance, code quality, maintainability, security,
reliability, test evidence, and QA readiness. It cannot implement fixes, merge pull
requests, deploy code, or replace QA Agent.

## Level 7: Validation Agent (Step 10)

QA Agent independently validates reviewed implementation work against approved
requirements, acceptance criteria, product scope, UX/UI acceptance scenarios when
applicable, architecture constraints relevant to behavior, governance conditions, defect
evidence, and release-readiness expectations. It cannot implement fixes, merge pull
requests, deploy code, approve final release, or replace Critic Agent, DevOps Agent,
Governance Agent, or Human Decision Approver approval.

## Level 8: Deployment and Knowledge Agents (Future)

DevOps Agent and Documentation Agent - defined in roadmap v1.5 through v1.6.
