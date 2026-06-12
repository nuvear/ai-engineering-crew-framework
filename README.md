# AI Engineering Crew Framework

## Human Decision Approver + AI Engineering Crew Operating Model

## Purpose

The AI Engineering Crew Framework is a structured operating model that enables a
business-oriented Human Decision Approver to direct an AI-native engineering crew to
design, build, review, deploy, and govern software solutions - without becoming a
programmer.

GitHub is the official source of truth for project memory, decisions, and deliverables.
Figma is the official design workspace for UX/UI work.

## Who This Framework Is For

This framework is designed for:

- **Business leaders and product owners** who own intent, value, priority, risk, and
  final approval
- **Business-led vibe coders** who want engineering discipline packaged into an
  AI-native crew
- **Enterprise teams** adopting AI agents for structured software delivery
- **Organizations** that require traceability, approval gates, and governance from day
  one

The human acts as Business Sponsor, Product Owner, Decision Approver, Value Owner, and
Final Accountability Holder. The agents supply structure, discipline, technical
reasoning, implementation support, review, testing, deployment preparation,
documentation, and governance support.

## Core Operating Philosophy

```text
Human owns intent, value, priority, risk, and final approval.
Agents own structured execution.
Engineering discipline must not be removed.
Engineering discipline must be packaged into an AI-native operating model.
```

Critical principles:

```text
If it is not in GitHub, it does not officially exist.
If it is not linked to a requirement, it should not be built.
If it is not approved, it should not be merged.
If it is not tested, it should not be released.
```

## Current Framework Scope

The current framework documents:

1. Human Decision Approver role
2. AI Engineering Crew philosophy
3. Enterprise Architect Agent
4. Environment Engineering Agent
5. GitHub collaboration workspace
6. Figma design workspace
7. Requirement Agent
8. Product Manager Agent
9. UX/UI Agent
10. Approval gates (Gates 0-6)
11. GitHub branching policy
12. Pull request policy
13. Commit deliverables policy
14. Testing policy
15. Decision log policy
16. Handover contracts between agents
17. Setup, test, and proceed workflow
18. Governance Agent and enterprise risk management framework
19. Builder Agent operating model
20. Critic Agent independent review operating model
21. QA Agent independent validation operating model

Framework Baseline v1.0 documents agent setup through **Step 6 (UX/UI Agent)**.

**Step 7 (Governance Agent)** defines the governance and enterprise risk management
framework required before Builder Agent begins. Builder Agent remains blocked until
Governance Agent risk classification and Human Decision Approver acceptance are
complete.

**Step 8 (Builder Agent)** defines Builder Agent setup as a governed implementation
support operating model only. It does not authorize application implementation without
approved requirements, architecture, governance acceptance, testing expectations, and
pull request review.

**Step 9 (Critic Agent)** defines Critic Agent setup as an independent review operating
model only. It reviews Builder Agent outputs before QA handover, but it does not
implement fixes, replace QA Agent, approve final release, merge pull requests, or
replace Human Decision Approver approval.

**Step 10 (QA Agent)** defines QA Agent setup as an independent validation operating
model only. It validates reviewed Builder output after Critic review and before future
DevOps preparation, but it does not replace Critic Agent, DevOps Agent, Governance
Agent, or Human Decision Approver approval.

## Agent Setup Order

```text
Step 1: Enterprise Architect Agent
Step 2: GitHub Collaboration Workspace
Step 3: Environment Engineering Agent
Step 4: Requirement Agent
Step 5: Product Manager Agent
Step 6: UX/UI Agent
Step 7: Governance Agent
Step 8: Builder Agent
Step 9: Critic Agent
Step 10: QA Agent
Step 11: DevOps Agent
Step 12: Documentation Agent
```

The repository documents Steps 1-10. Step 10 adds QA Agent setup as independent
validation after Critic review.

Builder Agent must not begin implementation unless Governance Agent has completed risk
classification and the Human Decision Approver has accepted the required governance
conditions.

Critic Agent must not implement fixes, approve final merge, deploy code, or replace QA
Agent.

QA Agent must not implement fixes, merge pull requests, deploy code, approve final
release, or replace Human Decision Approver approval.

## Repository Structure

```text
ai-engineering-crew-framework/
|-- README.md
|-- 00-vision/                    Framework charter and philosophy
|-- 01-operating-model/           Human + crew operating model
|-- 02-agent-topology/            Agent hierarchy and handovers
|-- 03-workspace-architecture/    GitHub + Figma workspace design
|-- 04-approval-gates/            Gates 0-6 approval checkpoints
|-- 05-policies/                  Branching, PR, testing, traceability
|-- 06-agents/                    Agent definitions (9 agents through Step 10)
|-- 07-templates/                 Reusable document templates
|-- 08-reference-project/         Inventory management reference flow
|-- 09-roadmap/                   Version roadmap and next steps
|-- 10-decision-log/              Recorded framework decisions
`-- .github/                      PR template, CODEOWNERS, issue templates
```

## Approval Gates

| Gate | Name                   | Prepared By                                                                                                                                   |
| ---- | ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| 0    | Environment Readiness  | Environment Engineering Agent                                                                                                                 |
| 1    | Requirement Approval   | Requirement Agent                                                                                                                             |
| 2    | Product Scope Approval | Product Manager Agent                                                                                                                         |
| 3    | UX Approval            | UX/UI Agent (Experience Design Mode)                                                                                                          |
| 4    | UI Approval            | UX/UI Agent (Visual Design Mode)                                                                                                              |
| 5    | Architecture Approval  | Enterprise Architect Agent                                                                                                                    |
| 6    | Release Approval       | Governance Agent for governance evidence; QA Agent for validation evidence; DevOps and Documentation as future release execution contributors |

See [04-approval-gates/](04-approval-gates/approval-gates-overview.md) for full gate
documentation.

## How to Use This Repository

1. **Read the vision** - Start with
   [00-vision/framework-charter.md](00-vision/framework-charter.md)
2. **Understand the operating model** - Review
   [01-operating-model/](01-operating-model/)
3. **Set up agents in order** - Follow Steps 1-10 in [06-agents/](06-agents/)
4. **Configure workspace** - Use
   [03-workspace-architecture/](03-workspace-architecture/)
5. **Apply templates** - Use [07-templates/](07-templates/) for all deliverables
6. **Walk the reference project** - Study [08-reference-project/](08-reference-project/)
   inventory management example
7. **Respect approval gates** - No phase proceeds without human approval
8. **Commit everything to GitHub** - Use the
   [branch naming format](#branch-naming-format) below

## Branch Naming Format

Use this branch format for all agent deliverables:

```text
agent/<agent-name>/<work-item-id>-short-description
```

Examples:

```text
agent/requirement/REQ-001-inventory-requirements
agent/product-manager/PROD-001-mvp-scope
agent/ux-ui/UX-001-inventory-wireframes
agent/environment-engineering/ENV-001-repository-setup
agent/governance/GOV-001-risk-classification
agent/builder/BUILD-001-approved-scope
agent/critic/CRITIC-001-independent-review
agent/qa/QA-001-validation-evidence
```

See [05-policies/branching-policy.md](05-policies/branching-policy.md) for full
branching rules.

## Version Roadmap

| Version | Focus                       |
| ------- | --------------------------- |
| v1.0    | Framework Baseline (merged) |
| v1.1    | Governance Agent            |
| v1.2    | Builder Agent (defined)     |
| v1.3    | Critic Agent (defined)      |
| v1.4    | QA Agent (defined)          |
| v1.5    | DevOps Agent                |
| v1.6    | Documentation Agent         |
| v1.7    | Multi-Agent Workflow        |
| v2.0    | Production Platform         |

See [09-roadmap/framework-roadmap.md](09-roadmap/framework-roadmap.md) for details.

## Current Step

Current completed step: **Step 10 - QA Agent Setup**

Next step: **Step 11 - DevOps Agent Setup**

Builder Agent setup is complete only as an operating model. Actual implementation work
still requires approved requirements, approved product scope, approved UX/UI handover
when applicable, approved architecture, completed governance risk classification, Human
Decision Approver acceptance of required governance conditions, testing expectations,
and pull request review.

Builder Agent must not begin implementation unless Governance Agent has completed risk
classification and the Human Decision Approver has accepted the required governance
conditions.

Critic Agent setup is complete only as an operating model. Critic Agent reviews Builder
output before QA validation, but it does not replace QA Agent, implement fixes, approve
final release, merge pull requests, or replace Human Decision Approver approval.

QA Agent setup is complete only as an operating model. DevOps Agent is not yet
implemented. QA Agent validates after Critic review, but it does not replace Critic
Agent, DevOps Agent, Governance Agent, or Human Decision Approver approval. QA Agent
cannot implement fixes, merge pull requests, deploy code, or approve final release.

---

Repository:
[nuvear/ai-engineering-crew-framework](https://github.com/nuvear/ai-engineering-crew-framework.git)
