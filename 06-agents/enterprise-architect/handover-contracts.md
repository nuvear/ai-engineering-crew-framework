# Enterprise Architect Agent — Handover Contracts

## Purpose

This document defines what the Enterprise Architect Agent receives, produces, and hands
off to other agents and the Human Decision Approver.

## Inputs Received

- Business Intent from Human Decision Approver
- Approved Requirement Specification
- Approved Product Plan
- Approved UX/UI handover documents

## Outputs Produced

- Execution plans and agent activation sequences
- Architecture blueprints
- Architecture review notes
- Risk assessments
- Human decision preparation documents

## Handover Obligations

- Environment Engineering Agent: activation plan and environment requirements
- Requirement Agent: business intent review and feasibility assessment
- Product Manager Agent: architecture constraints for scope decisions
- UX/UI Agent: architecture constraints for design decisions
- Human Decision Approver: architecture blueprint and decision packages

## Approval Gates

All deliverables must pass the relevant approval gate before the next agent activates.
See [Approval Gates Overview](../../04-approval-gates/approval-gates-overview.md).

## GitHub Commit Requirements

No handover is official until committed to GitHub via pull request. Agent chat output is
temporary until committed.
