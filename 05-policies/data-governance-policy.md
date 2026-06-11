# Data Governance Policy

## Purpose

Help the Human Decision Approver understand what data the solution uses, how sensitive
it is, and what handling rules apply before build and release.

## Scope

Applies to all business data, user data, operational data, sample data, test data, and
AI training or prompt context data used in the project.

## Data Classification Levels

| Level | Name         | Description                   | Examples                                    |
| ----- | ------------ | ----------------------------- | ------------------------------------------- |
| D1    | Public       | Safe for general sharing      | Marketing copy, public docs                 |
| D2    | Internal     | Business use only             | Internal process notes, drafts              |
| D3    | Confidential | Restricted business data      | Customer lists, pricing, inventory levels   |
| D4    | Restricted   | Highly sensitive or regulated | PII, financial records, health, credentials |

## Handling Rules

| Classification  | Storage                     | Access       | AI Usage                              | Sharing                          |
| --------------- | --------------------------- | ------------ | ------------------------------------- | -------------------------------- |
| D1 Public       | GitHub allowed              | Project team | Allowed with review                   | Allowed                          |
| D2 Internal     | GitHub with access control  | Project team | Allowed with declaration              | Internal only                    |
| D3 Confidential | Controlled repositories     | Need-to-know | Restricted, declared                  | Approval required                |
| D4 Restricted   | Approved secure stores only | Named owners | Prohibited unless explicitly approved | Human Decision Approver approval |

## Sensitive Data Rules

```text
Do not commit secrets, credentials, or live production data to GitHub.
Use sample or anonymized data in UX review whenever possible.
Document any exception in the decision log.
Classify data before Builder Agent begins implementation.
```

## Required Artifacts

- Data Classification document using `07-templates/data-classification-template.md`
- Data fields mapped to requirement IDs
- Retention and deletion notes for sensitive categories
- Human approval record for D3 and D4 data use

## Governance Agent Responsibilities

The Governance Agent must:

1. Identify data types used by the solution
2. Assign classification levels
3. Define handling and retention expectations
4. Flag data that blocks build or release until controlled
5. Prepare plain-language summaries for the Human Decision Approver

## Human Decision Approver Decisions

The human must approve:

- Use of D3 Confidential data in AI-assisted workflows
- Any use of D4 Restricted data
- Exceptions to storage or retention rules
- Customer or employee data in non-production test flows

## Link to Risk Classification

| Data Classification | Typical Project Risk Impact |
| ------------------- | --------------------------- |
| D1-D2 only          | Level 1-2                   |
| D3 present          | Level 3 likely              |
| D4 present          | Level 4 likely              |
