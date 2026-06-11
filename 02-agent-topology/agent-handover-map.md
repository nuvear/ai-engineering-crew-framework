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
Human Decision Approver -> Builder Agent (future, after governance acceptance)
```

## Handover Details

| From | To | Handover Artifact |
|---|---|---|
| Human | Enterprise Architect Agent | Business Intent |
| Enterprise Architect Agent | Environment Engineering Agent | Activation plan, environment requirements |
| Environment Engineering Agent | Workspace | GitHub repo, Figma project, templates, Gate 0 checklist |
| Human | Requirement Agent | Approved business intent, environment readiness |
| Requirement Agent | Product Manager Agent | Requirement Specification, Requirement-to-Product Handover |
| Product Manager Agent | UX/UI Agent | Product Plan, Product-to-UX Handover |
| UX/UI Agent | Enterprise Architect Agent | UX/UI artifacts, Figma links, UX-to-Architecture Handover |
| Enterprise Architect Agent | Governance Agent | Architecture Blueprint, architecture constraints |
| Governance Agent | Human Decision Approver | Governance Review, Risk Classification, human decision package |
| Human Decision Approver | Builder Agent (future) | Governance acceptance, authorized build scope |

## Active Step 7 Handover

```text
UX/UI Agent -> Enterprise Architect Agent -> Governance Agent -> Human Decision Approver -> Builder Agent (future)
```

Builder Agent must not begin until Governance Agent completes risk classification and the Human Decision Approver accepts governance conditions.

## Future Handovers

After Governance Agent approval and Step 7 merge:

- Builder Agent -> Critic Agent (code for review)
- Critic Agent -> QA Agent (reviewed code for testing)
- QA Agent -> DevOps Agent (tested code for deployment)
- DevOps Agent -> Documentation Agent (deployed system for documentation)
- QA, DevOps, Documentation, and Governance -> Human Decision Approver (Gate 6 release approval)
