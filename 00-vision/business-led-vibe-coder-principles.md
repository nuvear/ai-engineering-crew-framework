# Business-Led Vibe Coder Principles

## Who Is the Business-Led Vibe Coder?

A business-led vibe coder is a strong business leader — sponsor, product owner, or entrepreneur — who directs software creation through intent, decisions, and approval rather than through writing code. They "vibe" with the direction of the product while the AI engineering crew handles structured execution.

## Guiding Principles

```text
The human is not expected to read every line of code.
The human approves business decisions, risks, scope, UX, budget, and release readiness.
Agents translate business intent into technical work.
The system must protect the human from accidental technical chaos.
```

## What the Human Does

- Articulates business intent and goals
- Answers open questions about scope, users, and constraints
- Reviews and approves requirements, product scope, UX wireframes, UI design, and architecture (in business terms)
- Accepts or rejects risks at approval gates
- Makes go / no-go decisions for release
- Holds final accountability for value delivered

## What the Human Does Not Do

- Write application code
- Configure CI/CD pipelines manually (Environment Engineering Agent handles foundation)
- Review every pull request at the line level (Critic and QA agents handle this in future phases)
- Make architecture decisions without agent-prepared business-friendly summaries

## How the Framework Protects the Human

1. **Approval gates** — No phase proceeds without explicit human approval
2. **GitHub as source of truth** — Decisions and deliverables are never lost in chat history
3. **Traceability** — Every feature links back to a requirement and business goal
4. **Two-phase UX/UI** — Wireframes are approved before visual polish hides broken workflows
5. **Environment first** — Workspace, templates, and standards exist before build begins
6. **Decision log** — Major decisions are recorded with context, options, and rationale

## Success Looks Like

The business leader directs the crew with confidence, approves meaningful business decisions at each gate, and receives a traceable, governable software solution — without becoming a programmer.
