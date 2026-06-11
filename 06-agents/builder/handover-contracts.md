# Builder Agent - Handover Contracts

## Purpose

This document defines what the Builder Agent receives, produces, and hands off after
governed implementation work.

## Inputs Received

- Approved Requirement Specification from Requirement Agent
- Approved Product Plan from Product Manager Agent
- Approved UX/UI handover from UX/UI Agent when user experience is affected
- Approved Architecture Blueprint from Enterprise Architect Agent
- Governance risk classification from Governance Agent
- Accepted governance conditions from Human Decision Approver
- Linked GitHub issue or approved work item
- Testing expectations

## Outputs Produced

- Build Plan
- Implementation Task Breakdown
- Code changes within approved scope
- Files Changed Summary
- Requirement Traceability Notes
- Test Evidence
- Risk / Governance Notes
- Known Limitations
- Pull Request Summary
- Builder-to-Critic Handover

## Handover Obligations

### Governance-to-Builder Handover

Builder Agent must receive:

- Authorized build scope boundaries
- Required controls during implementation
- Prohibited data and AI usage boundaries
- Evidence that must be captured during build
- Explicit statement that build is authorized
- Human Decision Approver acceptance of governance conditions

### Builder-to-Critic Handover

Builder Agent must provide the future Critic Agent with:

- Pull request link
- Requirement IDs implemented
- Product scope boundaries followed
- Architecture constraints followed
- Governance controls followed
- Files changed summary
- Test evidence
- Known limitations and residual concerns
- Areas requiring focused review

## Stop Conditions

Builder Agent must stop and escalate if:

- Any required approval is missing
- Governance acceptance is missing
- Work expands approved scope
- Work conflicts with approved architecture
- Sensitive data handling is unclear or unapproved
- Test expectations are unclear

## GitHub Commit Requirements

No Builder deliverable is official until committed to GitHub via pull request. Builder
Agent must not approve or merge its own pull request.
