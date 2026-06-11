# Approval Policy

## Approval Matrix

```text
Deliverable | Prepared By | Reviewed By | Approved By
```

| Deliverable                 | Prepared By                              | Reviewed By                                                  | Approved By       |
| --------------------------- | ---------------------------------------- | ------------------------------------------------------------ | ----------------- |
| Business Intent             | Human                                    | Enterprise Architect Agent                                   | Human             |
| Environment Setup           | Environment Engineering Agent            | Enterprise Architect Agent                                   | Human             |
| Requirement Specification   | Requirement Agent                        | Product Manager Agent + Enterprise Architect Agent           | Human             |
| Product Plan                | Product Manager Agent                    | Requirement Agent + Enterprise Architect Agent               | Human             |
| UX Wireframes               | UX/UI Agent                              | Product Manager Agent + Enterprise Architect Agent           | Human             |
| UI Design                   | UX/UI Agent                              | Enterprise Architect Agent                                   | Human             |
| Architecture Blueprint      | Enterprise Architect Agent               | Governance Agent                                             | Human             |
| Governance Review           | Governance Agent                         | Enterprise Architect Agent                                   | Human             |
| Build Plan                  | Builder Agent                            | Enterprise Architect Agent + Governance Agent                | Human             |
| Implementation Pull Request | Builder Agent                            | Critic Agent + Enterprise Architect Agent + Governance Agent | Human             |
| Critic Review               | Critic Agent                             | Enterprise Architect Agent + Governance Agent                | Human if required |
| Release                     | QA + DevOps + Documentation + Governance | Enterprise Architect Agent                                   | Human             |

## Approval Recording

All approvals must be recorded in GitHub via PR review, issue status change, or decision
log entry.

## Rejection Process

If the Human Decision Approver rejects a deliverable:

1. Document rejection reason in PR comment or issue
2. Return to preparing agent for revision
3. Re-submit via new or updated pull request
4. Do not proceed to next gate until approved

## Builder Approval Constraints

Builder Agent must not approve or merge its own pull request. Builder Agent may prepare
implementation work only when required approvals, governance risk classification, and
Human Decision Approver governance acceptance exist.

## Critic Approval Constraints

Critic Agent must not implement fixes, approve final merge, deploy code, or replace QA
Agent. Critic Agent may recommend QA readiness only after independent review findings do
not block QA handover. Level 4 findings require Human Decision Approver visibility.
