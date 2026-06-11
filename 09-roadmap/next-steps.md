# Next Steps

## Current Work

The current framework work is Step 8 - Builder Agent Setup.

Step 8 adds the Builder Agent operating model and defines:

```text
Build planning
Implementation task breakdown
Approved-scope code change control
Requirement-to-code traceability
Test evidence expectations
Pull request discipline
Builder-to-Critic handover
```

## Step 8 Prerequisites

Before beginning Builder Agent setup:

- [ ] Framework Baseline v1.0 is committed and reviewed
- [ ] Governance Agent v1.1 is merged
- [ ] Reference project walkthrough is complete through Gate 5
- [ ] Governance risk acceptance rules are documented
- [ ] Human Decision Approver has reviewed governance controls

## Step 8 Completion Criteria

- [ ] Builder Agent folder in `06-agents/builder/` is complete
- [ ] Builder implementation policy is documented
- [ ] Code change control policy is documented
- [ ] Build plan and implementation task templates are complete
- [ ] Builder-to-Critic handover is defined
- [ ] Builder Agent cannot approve or merge its own pull request
- [ ] Builder Agent remains blocked unless governance acceptance is recorded

## Next Phase

After Step 8 is approved and merged, the next framework phase is Step 9 - Critic Agent.
