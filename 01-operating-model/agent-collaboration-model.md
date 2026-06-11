# Agent Collaboration Model

## Principle

Agents do not operate as isolated chatbots. They collaborate through a shared workspace
with defined handover contracts and approval gates.

## Collaboration Channels

Agents collaborate through:

```text
GitHub Issues
GitHub Pull Requests
GitHub Project Board
Markdown documents
Decision logs
Figma links
Handover contracts
Approval gates
```

## How Collaboration Works

1. **Shared workspace** — All official artifacts live in GitHub (and Figma for design).
   Agents read previous agents' committed work before producing their own.
2. **Handover contracts** — Each agent has defined inputs and outputs documented in
   `06-agents/<agent>/handover-contracts.md`.
3. **Pull requests** — All deliverables are introduced through PRs with linked issues,
   acceptance criteria, and test evidence.
4. **Approval gates** — No agent proceeds to the next phase until the human approves at
   the relevant gate.
5. **Decision log** — Major decisions are recorded for future agents and humans to
   reference.
6. **Traceability** — Every deliverable links to a business goal, requirement, or
   decision.

## Anti-Patterns

| Anti-Pattern                     | Why It Fails                                            |
| -------------------------------- | ------------------------------------------------------- |
| Agent chat without GitHub commit | Output is lost; other agents cannot read it             |
| Skipping handover review         | Next agent works from incomplete or wrong inputs        |
| Bypassing approval gates         | Unapproved scope enters build                           |
| Parallel agents on same artifact | Contradictory outputs without merge conflict resolution |
| Builder before requirements      | Code built without approved scope                       |

## Agent Activation Sequence

Agents activate in a defined order (see README Agent Setup Order). The Enterprise
Architect Agent orchestrates activation. Environment Engineering Agent must complete
before Requirement Agent. Requirement approval must complete before Product Manager
Agent. And so on through the gates.
