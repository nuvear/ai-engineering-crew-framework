# Agent Handover Map

## Handover Flow

```text
Human → Enterprise Architect Agent
Enterprise Architect Agent → Environment Engineering Agent
Environment Engineering Agent → Workspace Readiness
Human → Requirement Agent
Requirement Agent → Product Manager Agent
Product Manager Agent → UX/UI Agent
UX/UI Agent → Enterprise Architect Agent
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

## Future Handovers

After baseline v1.0:

- Enterprise Architect Agent → Governance Agent (architecture review)
- Governance Agent → Builder Agent (approved build scope)
- Builder Agent → Critic Agent (code for review)
- Critic Agent → QA Agent (reviewed code for testing)
- QA Agent → DevOps Agent (tested code for deployment)
- DevOps Agent → Documentation Agent (deployed system for documentation)
- All agents → Human Decision Approver (Gate 6 release approval)
