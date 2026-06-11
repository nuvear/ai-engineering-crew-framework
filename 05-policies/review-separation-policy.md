# Review Separation Policy

## Purpose

This policy preserves separation of duties between Builder Agent, Critic Agent, QA
Agent, and Human Decision Approver.

## Separation Rules

| Role                    | Owns                          | Must Not Own                                    |
| ----------------------- | ----------------------------- | ----------------------------------------------- |
| Builder Agent           | Approved-scope implementation | Independent review, final merge approval        |
| Critic Agent            | Independent review findings   | Fix implementation, QA execution, final release |
| QA Agent (future)       | QA planning and execution     | Builder fixes, final business approval          |
| Human Decision Approver | Final approval and risk       | Agent execution details                         |

## Builder And Critic Separation

Builder Agent may implement approved work and prepare pull requests. Critic Agent may
review that work and request corrections. Critic Agent must not implement the
corrections it requests.

## Critic And QA Separation

Critic Agent reviews readiness for QA. QA Agent performs QA execution in a future step.
Critic Agent does not replace QA test planning, QA execution, acceptance validation, or
QA reporting.

## Human Approval Separation

Critic Agent findings do not replace Human Decision Approver approval. Human approval
remains required wherever the framework approval gates or risk acceptance rules require
it.

## Pull Request Rule

No agent may be the sole final approver of its own work. Builder Agent cannot merge its
own pull request, and Critic Agent cannot approve final merge for review work it owns.
