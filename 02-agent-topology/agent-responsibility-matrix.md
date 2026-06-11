# Agent Responsibility Matrix

| Agent | Owns | Does Not Own | Key Output | Approval Required |
|---|---|---|---|---|
| Enterprise Architect Agent | Solution blueprint, architecture decisions, integration strategy, NFRs, security design, agent orchestration, architecture review | Raw business approval, product scope, final release, unapproved code | Architecture blueprint, activation plans, review notes | Human (Gate 5) |
| Environment Engineering Agent | GitHub setup, Figma setup, project board, branching, templates, CODEOWNERS, CI/CD foundation, secrets strategy, access matrix | Product scope, business requirements, UX decisions, application code, final release | Environment setup docs, Gate 0 checklist | Human (Gate 0) |
| Requirement Agent | Requirement discovery, scope definition, user roles, acceptance criteria, traceability | Architecture, code, deployment, final business approval | Requirement specification, scope boundary | Human (Gate 1) |
| Product Manager Agent | MVP definition, prioritization, roadmap, release planning, success metrics, scope control | Architecture, code, QA execution, deployment, final approval | Product plan, feature priority matrix | Human (Gate 2) |
| UX/UI Agent | Personas, journeys, wireframes, prototype, sample data, brand/UI design, developer handoff | Product scope, architecture, code, final approval | UX plan, UI handover, Figma links | Human (Gates 3 and 4) |
