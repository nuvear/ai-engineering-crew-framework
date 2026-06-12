# Agent Responsibility Matrix

## Enterprise Architect Agent

| Field             | Description                                                                                                                       |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Owns              | Solution blueprint, architecture decisions, integration strategy, NFRs, security design, agent orchestration, architecture review |
| Does Not Own      | Raw business approval, product scope, final release, unapproved code                                                              |
| Key Output        | Architecture blueprint, activation plans, review notes                                                                            |
| Approval Required | Human (Gate 5)                                                                                                                    |

## Environment Engineering Agent

| Field             | Description                                                                                                                   |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| Owns              | GitHub setup, Figma setup, project board, branching, templates, CODEOWNERS, CI/CD foundation, secrets strategy, access matrix |
| Does Not Own      | Product scope, business requirements, UX decisions, application code, final release                                           |
| Key Output        | Environment setup docs, Gate 0 checklist                                                                                      |
| Approval Required | Human (Gate 0)                                                                                                                |

## Requirement Agent

| Field             | Description                                                                            |
| ----------------- | -------------------------------------------------------------------------------------- |
| Owns              | Requirement discovery, scope definition, user roles, acceptance criteria, traceability |
| Does Not Own      | Architecture, code, deployment, final business approval                                |
| Key Output        | Requirement specification, scope boundary                                              |
| Approval Required | Human (Gate 1)                                                                         |

## Product Manager Agent

| Field             | Description                                                                               |
| ----------------- | ----------------------------------------------------------------------------------------- |
| Owns              | MVP definition, prioritization, roadmap, release planning, success metrics, scope control |
| Does Not Own      | Architecture, code, QA execution, deployment, final approval                              |
| Key Output        | Product plan, feature priority matrix                                                     |
| Approval Required | Human (Gate 2)                                                                            |

## UX/UI Agent

| Field             | Description                                                                                |
| ----------------- | ------------------------------------------------------------------------------------------ |
| Owns              | Personas, journeys, wireframes, prototype, sample data, brand/UI design, developer handoff |
| Does Not Own      | Product scope, architecture, code, final approval                                          |
| Key Output        | UX plan, UI handover, Figma links                                                          |
| Approval Required | Human (Gates 3 and 4)                                                                      |

## Governance Agent

| Field             | Description                                                                                                                                                                                         |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Owns              | Risk identification, risk classification, governance review, AI usage review, data governance review, audit evidence requirements, release governance support, value tracking, governance handovers |
| Does Not Own      | Final risk acceptance, budget approval, scope approval, architecture design, code implementation, final release go/no-go                                                                            |
| Key Output        | Governance Review, Risk Classification, AI Usage Declaration, Data Classification, Governance-to-Builder Handover                                                                                   |
| Approval Required | Human risk acceptance before Builder Agent begins                                                                                                                                                   |

## Builder Agent

| Field             | Description                                                                                                                                                                                            |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Owns              | Build plans, implementation task breakdowns, approved code changes, traceability notes, test evidence, pull request summaries, Builder-to-Critic handovers                                             |
| Does Not Own      | Business intent, scope approval, requirement approval, product priority, UX approval, architecture approval, governance risk acceptance, release approval, production deployment, final merge approval |
| Key Output        | Build Plan, Implementation Task Breakdown, Test Evidence, Pull Request Summary, Builder-to-Critic Handover                                                                                             |
| Approval Required | Approved requirements, approved scope, approved architecture, completed governance risk classification, and Human Decision Approver risk acceptance                                                    |

## Critic Agent

| Field             | Description                                                                                                                                                                                                                      |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Owns              | Independent review of Builder outputs, requirement traceability review, architecture conformance review, governance conformance review, code quality findings, test evidence findings, Builder feedback, Critic-to-QA handover   |
| Does Not Own      | Business intent, scope approval, requirement approval, product priority, UX approval, architecture approval, governance risk acceptance, code implementation, fix implementation, QA execution, deployment, final merge approval |
| Key Output        | Critic Review Report, Finding Severity Classification, Required Builder Corrections, QA Readiness Recommendation, Critic-to-Builder Feedback, Critic-to-QA Handover                                                              |
| Approval Required | Approved Builder handover, approved requirements, approved scope, approved architecture, completed governance classification, and Human Decision Approver governance acceptance                                                  |

## QA Agent

| Field             | Description                                                                                                                                                                                                                                         |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Owns              | Independent validation of reviewed implementation work, QA test planning, test case definition, functional validation, regression validation, defect evidence, QA pass/fail recommendation, QA-to-DevOps handover                                   |
| Does Not Own      | Business intent, requirement approval, product scope approval, UX approval, architecture approval, governance risk acceptance, code implementation, fix implementation, code review replacement, deployment, release approval, final merge approval |
| Key Output        | QA Test Plan, Test Case Set, Test Execution Report, Defect Report, Acceptance Criteria Coverage Matrix, QA Pass/Fail Recommendation, QA-to-DevOps Handover                                                                                          |
| Approval Required | Completed Critic review, approved requirements, acceptance criteria, product scope, relevant UX/UI scenarios, architecture constraints, governance conditions, and sufficient test environment                                                      |
