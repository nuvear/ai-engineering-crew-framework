# Value Realization Policy

## Purpose

Ensure the Human Decision Approver can measure whether the solution delivers intended
business value, not just technical completion.

## Principle

Value must be defined before build, tracked after release, and reviewed in business
terms the human understands.

## Value Definition Requirements

Every approved Product Plan should define:

```text
Business outcome expected
User or operational value
Success metrics
Measurement method
Review frequency
Owner for value review
```

## Value Tracking Structure

Governance Agent prepares a value tracking section containing:

| Metric | Business Goal | Baseline | Target | Data Source | Review Frequency | Owner |
| ------ | ------------- | -------- | ------ | ----------- | ---------------- | ----- |

## Example Metrics

| Metric Type    | Example                                |
| -------------- | -------------------------------------- |
| Efficiency     | Time to complete inventory count       |
| Quality        | Reduction in stock-out incidents       |
| Adoption       | Active users per role                  |
| Financial      | Cost avoided or revenue protected      |
| Risk reduction | Number of manual reconciliation errors |

## Governance Review Points

| Checkpoint                   | Value Question                           |
| ---------------------------- | ---------------------------------------- |
| After requirement approval   | Is the business problem worth solving?   |
| After product scope approval | Is MVP scope sufficient to prove value?  |
| Before build authorization   | Are success metrics measurable?          |
| Before release               | Is value evidence plan ready?            |
| After release                | Did the solution deliver expected value? |

## Human Decision Approver Role

The human owns whether value targets are acceptable, whether partial value justifies
release, and whether continued investment is warranted.

## Link to Release Governance

Gate 6 release approval should confirm that value realization tracking is defined and
owned, even if full value results are measured post-release.

## Evidence Requirements

```text
Value metrics documented in docs/06-governance/ or docs/03-product-management/
Linked to requirement IDs and business goals
Review schedule recorded in GitHub
Post-release review issue or milestone created
```

## Anti-Patterns

```text
Declaring success without defined metrics
Measuring only technical activity (commits, story count) instead of business value
Releasing without a plan to evaluate outcomes
Changing value targets after release without decision log entry
```
