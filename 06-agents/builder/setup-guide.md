# Builder Agent — Setup Guide

## Agent Setup

1. Create a new single-step agent named Builder Agent.
2. Paste system instruction from `system-instruction.md`.
3. Connect implementation policies from `05-policies/`:
   - `builder-implementation-policy.md`
   - `code-change-control-policy.md`
   - `testing-policy.md`
   - `traceability-policy.md`
   - `pull-request-policy.md`
4. Connect Builder templates from `07-templates/`.
5. Connect Governance Agent handover requirements from `06-agents/governance/`.

## Activation Prerequisites

- Gate 1 Requirement Approval exists
- Gate 2 Product Scope Approval exists
- Gate 3 and Gate 4 UX/UI approvals exist when user experience is affected
- Gate 5 Architecture Approval exists
- Governance Agent risk classification exists
- Human Decision Approver has accepted required governance conditions
- Linked GitHub issue or approved work item exists
- Test expectations are documented

## Builder Workspace Location

Store project build artifacts in:

```text
docs/07-build/
```

Recommended files:

```text
BUILD-PLAN-[work-item-id].md
IMPLEMENTATION-TASK-[work-item-id].md
BUILDER-PR-SUMMARY-[work-item-id].md
BUILDER-TO-CRITIC-HANDOVER-[work-item-id].md
```

## First Activation Checklist

- [ ] Builder Agent configured
- [ ] Builder policies linked as knowledge documents
- [ ] Builder templates linked as output templates
- [ ] Governance-to-Builder handover available
- [ ] Human Decision Approver risk acceptance available
- [ ] Pull request template includes implementation evidence
- [ ] Builder Agent understands it cannot approve or merge its own pull request
