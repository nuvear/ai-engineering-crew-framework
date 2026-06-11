# Branching Policy

## Core Rules

```text
main is protected.
No direct commits to main.
All changes go through pull requests.
Feature branches use the following format:

agent/<agent-name>/<work-item-id>-short-description
```

## Branch Naming Examples

```text
agent/requirement/REQ-001-inventory-requirements
agent/product-manager/PROD-001-mvp-scope
agent/ux-ui/UX-001-inventory-wireframes
agent/environment/ENV-001-repository-setup
```

## Branch Lifecycle

1. Create branch from latest `main`
2. Agent produces deliverables on the branch
3. Open pull request with linked issue and acceptance criteria
4. Human reviews and approves at relevant gate
5. Merge to `main` after approval checklist passes

## Protection Rules

- `main` branch requires pull request before merge
- Direct pushes to `main` are prohibited
- Branch should be deleted after merge
