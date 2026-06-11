# GitHub Workspace Setup

## Components

The GitHub workspace includes:

```text
Repository
Project Board
Issues
Labels
Pull Requests
Branch protection
CODEOWNERS
Decision logs
Templates
```

## Repository

Create a dedicated repository per software solution. The framework repository
(`ai-engineering-crew-framework`) is separate from project repositories.

## Project Board

Configure columns matching workflow statuses (see
[github-project-board.md](github-project-board.md)).

## Issues

Use issue templates for business intent, requirements, product features, decisions, and
risks.

## Labels

Apply recommended labels for agent ownership, status, gate tracking, and work type:

```text
agent: requirement
agent: product-manager
agent: enterprise-architect
agent: environment-engineering
agent: ux-ui
agent: governance
agent: builder
agent: critic
agent: qa
agent: devops
agent: documentation

status: draft
status: review
status: approved
status: blocked
status: rejected

gate: environment-readiness
gate: requirement-approval
gate: product-scope-approval
gate: ux-approval
gate: ui-approval
gate: architecture-approval
gate: release-approval

type: requirement
type: feature
type: decision
type: risk
type: defect
type: documentation
```

## Pull Requests

All deliverables enter through pull requests using the PR template.

Branch format:

```text
agent/<agent-name>/<work-item-id>-short-description
```

## Branch Protection

Protect `main` branch. Require pull request reviews before merge. No direct commits to
main.

## CODEOWNERS

Define ownership for framework and project directories. See `.github/CODEOWNERS`.

## Decision Logs

Store decision records in `docs/10-decision-log/` (project) or `10-decision-log/`
(framework).

## Templates

Issue templates, PR template, and markdown document templates ensure consistent artifact
structure.
