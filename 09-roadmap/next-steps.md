# Next Steps

## Current Work

The current completed framework work is Step 9 - Critic Agent Setup.

Step 9 adds the Critic Agent operating model and defines:

```text
Independent review of Builder Agent outputs
Requirement-to-code traceability review
Architecture conformance review
Governance conformance review
Code quality and maintainability critique
Security, privacy, compliance, and reliability concern identification
Test evidence review
Finding severity classification
Critic-to-Builder feedback
Critic-to-QA handover
```

## Step 9 Prerequisites

Before beginning Critic Agent setup:

- [ ] Framework Baseline v1.0 is committed and reviewed
- [ ] Governance Agent v1.1 is merged
- [ ] Builder Agent v1.2 is merged
- [ ] Builder-to-Critic handover is documented
- [ ] Pull request review discipline is documented
- [ ] Review separation rules are documented

## Step 9 Completion Criteria

- [ ] Critic Agent folder in `06-agents/critic/` is complete
- [ ] Critic review policy is documented
- [ ] Review separation policy is documented
- [ ] Critic review templates are complete
- [ ] Finding severity model is defined
- [ ] Critic-to-Builder feedback is defined
- [ ] Critic-to-QA handover is defined
- [ ] Critic Agent cannot implement fixes
- [ ] Critic Agent cannot approve or merge pull requests
- [ ] Critic Agent does not replace QA Agent

## Next Phase

After Step 9 is approved and merged, the next framework phase is Step 10 - QA Agent.
