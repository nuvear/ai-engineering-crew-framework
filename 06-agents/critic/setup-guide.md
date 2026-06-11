# Critic Agent - Setup Guide

## Agent Setup

1. Create a new single-step agent named Critic Agent.
2. Paste system instruction from `system-instruction.md`.
3. Connect review policies from `05-policies/`:
   - `critic-review-policy.md`
   - `review-separation-policy.md`
   - `pull-request-policy.md`
   - `code-change-control-policy.md`
   - `definition-of-done.md`
4. Connect Critic templates from `07-templates/`.
5. Connect Builder Agent handover requirements from `06-agents/builder/`.

## Activation Prerequisites

- Builder Agent PR summary exists
- Build Plan exists
- Implementation task breakdown exists
- Files Changed Summary exists
- Requirement Traceability Notes exist
- Test Evidence exists
- Risk / Governance Notes exist
- Builder-to-Critic handover exists
- Required approvals and governance acceptance are linked

## Critic Workspace Location

Store project review artifacts in:

```text
docs/08-review/
```

Recommended files:

```text
CRITIC-REVIEW-[work-item-id].md
CODE-REVIEW-CHECKLIST-[work-item-id].md
ARCHITECTURE-CONFORMANCE-REVIEW-[work-item-id].md
CRITIC-TO-BUILDER-FEEDBACK-[work-item-id].md
CRITIC-TO-QA-HANDOVER-[work-item-id].md
```

## First Activation Checklist

- [ ] Critic Agent configured
- [ ] Critic policies linked as knowledge documents
- [ ] Critic templates linked as output templates
- [ ] Builder-to-Critic handover available
- [ ] Critic Agent understands it cannot implement fixes
- [ ] Critic Agent understands it cannot approve or merge pull requests
- [ ] Critic Agent understands it does not replace QA Agent
