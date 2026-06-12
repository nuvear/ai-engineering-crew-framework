# Next Steps

## Current Work

The current completed framework work is Step 10 - QA Agent Setup.

Step 10 adds the QA Agent operating model and defines:

```text
Independent validation of reviewed implementation work
QA test planning
Test case definition
Functional and regression validation
Edge case and negative path validation
UX acceptance validation when applicable
Governance validation checks
Defect identification and evidence capture
Test execution reporting
QA pass/fail recommendation
QA-to-DevOps handover
```

## Step 10 Prerequisites

Before beginning QA Agent setup:

- [ ] Framework Baseline v1.0 is committed and reviewed
- [ ] Governance Agent v1.1 is merged
- [ ] Builder Agent v1.2 is merged
- [ ] Critic Agent v1.3 is merged
- [ ] Critic-to-QA handover is documented
- [ ] Test evidence rules are documented
- [ ] Defect management rules are documented

## Step 10 Completion Criteria

- [ ] QA Agent folder in `06-agents/qa/` is complete
- [ ] QA validation policy is documented
- [ ] Test evidence policy is documented
- [ ] Defect management policy is documented
- [ ] QA templates are complete
- [ ] Defect severity model is defined
- [ ] Critic-to-QA handover is defined
- [ ] QA-to-DevOps handover is defined
- [ ] QA Agent cannot implement fixes
- [ ] QA Agent cannot merge pull requests
- [ ] QA Agent cannot deploy code
- [ ] QA Agent cannot approve final release
- [ ] QA Agent does not replace Critic, DevOps, Governance, or Human Decision Approver
      approval

## Next Phase

After Step 10 is approved and merged, the next framework phase is Step 11 - DevOps
Agent.
