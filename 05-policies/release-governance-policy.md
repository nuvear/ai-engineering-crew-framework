# Release Governance Policy

## Purpose

Connect governance controls to Gate 6 (Release Approval) so release decisions are based on evidence, not assumption.

## Scope

Applies to all releases, production deployments, and externally visible go-live events.

## Gate 6 Connection

Release governance uses [Gate 6 — Release Approval](../04-approval-gates/gate-6-release-approval.md).

Governance Agent supports Gate 6 by defining what evidence must exist before the Human Decision Approver approves release.

## Pre-Release Governance Checklist

- [ ] All Level 3 and Level 4 risks reviewed and accepted or mitigated
- [ ] AI Usage Declaration current and approved
- [ ] Data classification current and approved
- [ ] Audit evidence package complete
- [ ] QA evidence available (future baseline)
- [ ] Deployment readiness documented (future baseline)
- [ ] Documentation complete (future baseline)
- [ ] Rollback plan documented
- [ ] Value realization metrics defined

## Release Decision Options

| Decision | Meaning |
|---|---|
| Approve release | All required evidence present; human approves go-live |
| Approve with conditions | Release allowed after documented conditions are met |
| Reject release | Release blocked; return to responsible agent |
| Defer release | Pause until dependencies or decisions are resolved |

## Residual Risk at Release

Any unresolved risk at release must be:

1. Documented in the risk register
2. Assigned an accepted risk owner
3. Accepted explicitly by the Human Decision Approver
4. Linked to Gate 6 approval record

## Governance-to-Release Handover Contents

```text
Final risk summary
Compliance status
AI usage status
Data handling status
Required release evidence checklist
Open human decisions
Recommended release decision
```

## Builder and Release Boundary

Builder Agent output alone is not sufficient for release. Release requires Gate 6 approval supported by governance, testing, deployment readiness, and documentation evidence as defined for the project risk level.

## Post-Release Governance

After release, governance artifacts must include:

- Release approval record
- Release notes link
- Value realization review schedule
- Post-release risk review date
