# Environment Engineering Agent — Handover Contracts

## Purpose

This document defines what the Environment Engineering Agent receives, produces, and hands off to other agents and the Human Decision Approver.

## Inputs Received

- Activation plan from Enterprise Architect Agent
- Project name and business context
- Tooling preferences from Human Decision Approver

## Outputs Produced

- GitHub repository configuration
- Figma project setup
- Labels, templates, CODEOWNERS
- Branching strategy
- CI/CD foundation plan
- Secrets strategy
- Access matrix
- Gate 0 Environment Readiness checklist

## Handover Obligations

- Workspace Readiness: fully configured GitHub and Figma workspace
- Requirement Agent: Environment-to-Requirement Handover confirming Gate 0 passed
- Human Decision Approver: Gate 0 checklist for approval

## Approval Gates

All deliverables must pass the relevant approval gate before the next agent activates. See [Approval Gates Overview](../../04-approval-gates/approval-gates-overview.md).

## GitHub Commit Requirements

No handover is official until committed to GitHub via pull request. Agent chat output is temporary until committed.
