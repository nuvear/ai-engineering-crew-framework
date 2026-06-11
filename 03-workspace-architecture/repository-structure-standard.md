# Repository Structure Standard

## Standard Software Project Repository

Every software solution built under the AI Engineering Crew Framework should follow this
repository structure:

```text
project-name/
|
|-- docs/
|   |-- 00-environment/
|   |-- 01-business-intent/
|   |-- 02-requirements/
|   |-- 03-product-management/
|   |-- 04-ux-ui/
|   |-- 05-architecture/
|   |-- 06-governance/
|   |-- 07-build/
|   |-- 08-review/
|   |-- 09-qa/
|   |-- 10-devops/
|   |-- 11-documentation/
|   `-- 12-decision-log/
|
|-- src/
|-- tests/
|-- .github/
`-- README.md
```

## Directory Purposes

| Directory                     | Contents                                                             |
| ----------------------------- | -------------------------------------------------------------------- |
| `docs/00-environment/`        | Environment setup, tool inventory, access matrix, branching strategy |
| `docs/01-business-intent/`    | Business intent documents                                            |
| `docs/02-requirements/`       | Requirement specifications                                           |
| `docs/03-product-management/` | Product plans, MVP scope, roadmaps                                   |
| `docs/04-ux-ui/`              | Personas, journeys, wireframes, Figma links, UI handover             |
| `docs/05-architecture/`       | Architecture blueprints                                              |
| `docs/06-governance/`         | Risk registers, compliance docs                                      |
| `docs/07-build/`              | Build plans, implementation tasks, Builder handovers                 |
| `docs/08-review/`             | Critic reviews, findings, QA readiness handovers                     |
| `docs/09-qa/`                 | Test plans, test reports (future)                                    |
| `docs/10-devops/`             | Deployment configs, CI/CD (future)                                   |
| `docs/11-documentation/`      | User guides, API docs (future)                                       |
| `docs/12-decision-log/`       | Decision records                                                     |
| `src/`                        | Application source code (future, after build phase)                  |
| `tests/`                      | Test code (future)                                                   |
| `.github/`                    | Issue templates, PR template, CODEOWNERS, workflows                  |
