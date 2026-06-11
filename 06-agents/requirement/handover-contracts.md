# Requirement Agent — Handover Contracts

## Purpose

This document defines what the Requirement Agent receives, produces, and hands off to
other agents and the Human Decision Approver.

## Inputs Received

- Business Intent from Human Decision Approver
- Environment readiness confirmation (Gate 0 passed)
- Open questions from Enterprise Architect review

## Outputs Produced

- Requirement Specification document
- GitHub issue list for requirements
- Acceptance criteria table
- Scope boundary and out-of-scope list
- Open human questions list

## Handover Obligations

- Product Manager Agent: Requirement Specification and Requirement-to-Product Handover
- Enterprise Architect Agent: Requirement-to-Architecture Handover
- Human Decision Approver: Requirement Specification for Gate 1 approval

## Approval Gates

All deliverables must pass the relevant approval gate before the next agent activates.
See [Approval Gates Overview](../../04-approval-gates/approval-gates-overview.md).

## GitHub Commit Requirements

No handover is official until committed to GitHub via pull request. Agent chat output is
temporary until committed.
