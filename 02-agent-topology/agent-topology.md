# Agent Topology

## Original Concept

```text
Human Decision Approver
        ↓
Enterprise Architect Agent
        ↓
Requirement / PM / Governance / UX / Builder / Critic / QA / DevOps / Documentation
```

In the original concept, specialist agents reported directly to the Enterprise Architect
Agent without an explicit workspace layer.

## Revised Concept

```text
Human Decision Approver
        ↓
Enterprise Architect Agent
        ↓
Environment Engineering Agent
        ↓
Collaboration Workspace
        ↓
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

## Current Baseline Agents

| Agent                         | Layer         |
| ----------------------------- | ------------- |
| Enterprise Architect Agent    | Orchestration |
| Environment Engineering Agent | Workspace     |
| Requirement Agent             | Planning      |
| Product Manager Agent         | Planning      |
| UX/UI Agent                   | Design        |

## Future Agents

Governance, Builder, Critic, QA, DevOps, and Documentation agents are defined in the
roadmap but not fully specified in v1.0.
