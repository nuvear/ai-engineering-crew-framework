# Governance Agent — Setup Guide

## Gemini Enterprise Setup

1. Open Gemini Enterprise Agent Designer
2. Create new single-step agent named Governance Agent
3. Paste system instruction from `system-instruction.md`
4. Connect governance policies from `05-policies/`:
   - `ai-usage-policy.md`
   - `data-governance-policy.md`
   - `auditability-policy.md`
   - `release-governance-policy.md`
   - `value-realization-policy.md`
5. Connect governance templates from `07-templates/`
6. Connect risk register and reference project samples

## Activation Prerequisites

- Gate 0 (Environment Readiness) must be approved
- Approved Requirement Specification must exist in GitHub
- Approved Product Plan must exist in GitHub
- Approved UX/UI handover must exist when user-facing or data-sensitive flows are
  involved
- Approved Architecture Blueprint must exist before final governance sign-off for build
  authorization

## Governance Workspace Location

Store project governance artifacts in:

```text
docs/06-governance/
```

Recommended files:

```text
GOVERNANCE-REVIEW-[project-name].md
RISK-REGISTER-[project-name].md
RISK-CLASSIFICATION-[project-name].md
AI-USAGE-DECLARATION-[project-name].md
DATA-CLASSIFICATION-[project-name].md
VALUE-TRACKING-[project-name].md
```

## First Activation Checklist

- [ ] Governance Agent configured in Gemini Enterprise
- [ ] Governance policies linked as knowledge documents
- [ ] GitHub labels include `agent: governance` and `gate: release-approval`
- [ ] Risk issue template available in `.github/ISSUE_TEMPLATE/risk.md`
- [ ] Human Decision Approver understands 4-level risk model
