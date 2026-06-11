# GitHub Project Board

## Purpose

The GitHub Project Board tracks work items through the full AI Engineering Crew workflow
from intake to release.

## Status Columns

```text
Intake
Environment Setup
Requirement Drafting
Requirement Review
Product Planning
Scope Approval
UX Design
UX Approval
UI Design
UI Approval
Architecture Review
Architecture Approval
Ready for Build
Build in Progress
Critic Review
QA Testing
Deployment Readiness
Release Approval
Released
Blocked
```

## Status Flow

1. **Intake** - Business intent received
2. **Environment Setup** - Environment Engineering Agent preparing workspace
3. **Requirement Drafting** - Requirement Agent creating specification
4. **Requirement Review** - Human reviewing requirements (Gate 1)
5. **Product Planning** - Product Manager Agent creating product plan
6. **Scope Approval** - Human reviewing product scope (Gate 2)
7. **UX Design** - UX/UI Agent Mode 1 (Experience Design)
8. **UX Approval** - Human reviewing wireframes (Gate 3)
9. **UI Design** - UX/UI Agent Mode 2 (Visual Design)
10. **UI Approval** - Human reviewing UI (Gate 4)
11. **Architecture Review** - Enterprise Architect preparing blueprint
12. **Architecture Approval** - Human reviewing architecture (Gate 5)
13. **Ready for Build** - All pre-build gates passed
14. **Build in Progress** - Builder Agent
15. **Critic Review** - Critic Agent (future)
16. **QA Testing** - QA Agent (future)
17. **Deployment Readiness** - DevOps Agent (future)
18. **Release Approval** - Human final approval (Gate 6)
19. **Released** - Solution live
20. **Blocked** - Work paused pending decision or dependency

## Usage

Move issues through columns as work progresses. Link issues to pull requests and
markdown deliverables. Use labels for agent ownership and gate tracking.
