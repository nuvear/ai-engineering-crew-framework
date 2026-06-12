# Agent Topology

## Original Concept

```text
Human Decision Approver
        v
Enterprise Architect Agent
        v
Requirement / PM / Governance / UX / Builder / Critic / QA / DevOps / Documentation
```

In the original concept, specialist agents reported directly to the Enterprise Architect
Agent without an explicit workspace layer.

## Revised Concept

```text
Human Decision Approver
        v
Enterprise Architect Agent
        v
Environment Engineering Agent
        v
Collaboration Workspace
        v
Specialist Agents
```

## Why the Revision

The workspace is the source of truth. Agents must read and write to it. Without the
Environment Engineering Agent and collaboration workspace established early:

- Agents repeat questions
- Agents contradict each other
- Decisions are forgotten
- Scope expands uncontrolled
- Builder may build unapproved features

The revised topology inserts Environment Engineering Agent and the Collaboration
Workspace (GitHub + Figma) before specialist planning and design agents activate.

## Current Framework Agents

| Agent                         | Layer                  |
| ----------------------------- | ---------------------- |
| Enterprise Architect Agent    | Orchestration          |
| Environment Engineering Agent | Workspace              |
| Requirement Agent             | Planning               |
| Product Manager Agent         | Planning               |
| UX/UI Agent                   | Design                 |
| Governance Agent              | Governance             |
| Builder Agent                 | Implementation Support |
| Critic Agent                  | Independent Review     |
| QA Agent                      | Independent Validation |

## Future Agents

DevOps and Documentation agents remain future steps. QA Agent validates reviewed Builder
output before future DevOps handover.
