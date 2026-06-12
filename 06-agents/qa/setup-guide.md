# QA Agent - Setup Guide

## Agent Setup

1. Create a new single-step agent named QA Agent.
2. Paste system instruction from `system-instruction.md`.
3. Connect QA policies from `05-policies/`:
   - `qa-validation-policy.md`
   - `test-evidence-policy.md`
   - `defect-management-policy.md`
   - `testing-policy.md`
   - `review-separation-policy.md`
4. Connect QA templates from `07-templates/`.
5. Connect Critic Agent handover requirements from `06-agents/critic/`.

## Activation Prerequisites

- Critic-to-QA handover exists
- Critic review is complete
- No unresolved Level 3 or Level 4 Critic findings block QA
- Approved requirements and acceptance criteria exist
- Product scope approval exists
- UX/UI acceptance scenarios exist when user experience is affected
- Architecture constraints relevant to validation are linked
- Governance conditions relevant to validation are linked
- Test environment and sample data are sufficient

## QA Workspace Location

Store project QA artifacts in:

```text
docs/09-qa/
```

Recommended files:

```text
QA-TEST-PLAN-[work-item-id].md
TEST-CASE-[work-item-id].md
DEFECT-REPORT-[work-item-id].md
QA-EXECUTION-REPORT-[work-item-id].md
QA-TO-DEVOPS-HANDOVER-[work-item-id].md
```

## First Activation Checklist

- [ ] QA Agent configured
- [ ] QA policies linked as knowledge documents
- [ ] QA templates linked as output templates
- [ ] Critic-to-QA handover available
- [ ] QA Agent understands it cannot implement fixes
- [ ] QA Agent understands it cannot merge pull requests
- [ ] QA Agent understands it cannot deploy code
- [ ] QA Agent understands it cannot approve final release
- [ ] QA Agent understands it does not replace Critic, DevOps, Governance, or Human
      Decision Approver approval
