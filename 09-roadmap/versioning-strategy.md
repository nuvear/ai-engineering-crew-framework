# Versioning Strategy

## Framework Versioning

The AI Engineering Crew Framework uses semantic versioning for framework releases:

- **Major (x.0):** Fundamental operating model changes (e.g., v2.0 Production Platform)
- **Minor (1.x):** New agent additions or significant policy updates (e.g., v1.1
  Governance Agent)
- **Patch (1.0.x):** Documentation corrections, template updates, minor policy
  clarifications

## Current Version

**Framework Baseline v1.0** — Documents the framework through Step 6 (UX/UI Agent).

## Version Alignment with Agent Setup

| Framework Version | Agent Setup Step | Agent Added                                                                        |
| ----------------- | ---------------- | ---------------------------------------------------------------------------------- |
| v1.0              | Steps 1–6        | Enterprise Architect, Environment Engineering, Requirement, Product Manager, UX/UI |
| v1.1              | Step 7           | Governance Agent                                                                   |
| v1.2              | Step 8           | Builder Agent                                                                      |
| v1.3              | Step 9           | Critic Agent                                                                       |
| v1.4              | Step 10          | QA Agent                                                                           |
| v1.5              | Step 11          | DevOps Agent                                                                       |
| v1.6              | Step 12          | Documentation Agent                                                                |

## Project Versioning

Software projects built under the framework follow their own versioning independent of
the framework version. Project release plans are defined by the Product Manager Agent.

## Decision Log Versioning

Framework decisions are numbered sequentially (DEC-001, DEC-002, ...). Project decisions
use the same format within the project repository's decision log.

## Branch and Tag Strategy

- Framework development uses feature branches: `feature/framework-baseline-v1`,
  `feature/governance-agent-v1.1`, etc.
- Released framework versions are tagged: `v1.0.0`, `v1.1.0`, etc.
- Project repositories tag releases independently after Gate 6 approval.
