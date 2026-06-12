# Agent Handover Map

## Handover Flow

```text
Human -> Enterprise Architect Agent
Enterprise Architect Agent -> Environment Engineering Agent
Environment Engineering Agent -> Workspace Readiness
Human -> Requirement Agent
Requirement Agent -> Product Manager Agent
Product Manager Agent -> UX/UI Agent
UX/UI Agent -> Enterprise Architect Agent
Enterprise Architect Agent -> Governance Agent
Governance Agent -> Human Decision Approver
Human Decision Approver -> Builder Agent
Builder Agent -> Critic Agent
Critic Agent -> QA Agent
QA Agent -> DevOps Agent (future)
```

## Handover Details

| From                          | To                            | Handover Artifact                                              |
| ----------------------------- | ----------------------------- | -------------------------------------------------------------- |
| Human                         | Enterprise Architect Agent    | Business Intent                                                |
| Enterprise Architect Agent    | Environment Engineering Agent | Activation plan, environment requirements                      |
| Environment Engineering Agent | Workspace                     | GitHub repo, Figma project, templates, Gate 0 checklist        |
| Human                         | Requirement Agent             | Approved business intent, environment readiness                |
| Requirement Agent             | Product Manager Agent         | Requirement Specification, Requirement-to-Product Handover     |
| Product Manager Agent         | UX/UI Agent                   | Product Plan, Product-to-UX Handover                           |
| UX/UI Agent                   | Enterprise Architect Agent    | UX/UI artifacts, Figma links, UX-to-Architecture Handover      |
| Enterprise Architect Agent    | Governance Agent              | Architecture Blueprint, architecture constraints               |
| Governance Agent              | Human Decision Approver       | Governance Review, Risk Classification, human decision package |
| Human Decision Approver       | Builder Agent                 | Governance acceptance, authorized build scope                  |
| Builder Agent                 | Critic Agent                  | Pull request, test evidence, Builder-to-Critic handover        |
| Critic Agent                  | QA Agent                      | Critic Review Report, Critic-to-QA handover                    |
| QA Agent                      | DevOps Agent (future)         | QA Test Report, QA-to-DevOps handover                          |

## Active Step 10 Handover

```text
UX/UI Agent -> Enterprise Architect Agent -> Governance Agent -> Human Decision Approver -> Builder Agent -> Critic Agent -> QA Agent -> DevOps Agent (future)
```

Builder Agent must not begin until Governance Agent completes risk classification and
the Human Decision Approver accepts governance conditions.

Critic Agent reviews Builder Agent outputs before QA handover. Critic Agent must not
implement fixes, merge pull requests, deploy code, or replace QA Agent.

QA Agent validates reviewed implementation work after Critic review and before future
DevOps handover. QA Agent must not implement fixes, merge pull requests, deploy code,
approve final release, or replace Critic Agent, DevOps Agent, Governance Agent, or Human
Decision Approver approval.

## Future Handovers

After QA Agent setup and Step 10 merge:

- QA Agent -> DevOps Agent (tested code for deployment)
- DevOps Agent -> Documentation Agent (deployed system for documentation)
- QA, DevOps, Documentation, and Governance -> Human Decision Approver (Gate 6 release
  approval)
