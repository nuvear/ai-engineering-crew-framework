# Decision Log Policy

## Requirement

Every major decision must be recorded in the decision log.

## File Format

```text
DEC-[number]-[short-title].md
```

## Required Fields

Each decision must include:

```text
Decision ID
Decision title
Date
Decision owner
Prepared by
Reviewed by
Context
Options considered
Decision
Reason
Impact
Follow-up action
```

## When to Record a Decision

- Framework design choices (see `10-decision-log/` for examples)
- Architecture approach selection
- Scope trade-off acceptance
- Technology selection
- Risk acceptance
- Process changes

## Location

- Framework decisions: `10-decision-log/` in the framework repository
- Project decisions: `docs/10-decision-log/` in project repositories
