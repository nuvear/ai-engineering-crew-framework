# Inventory Management System — Reference Flow

## Purpose

This reference project demonstrates the complete AI Engineering Crew workflow from business intent through architecture handover using an inventory management system. No application code is included — this is documentation only.

## Business Intent

A small business needs to track products, stock quantities, stock movements, low-stock alerts, and generate simple reports. Users include a business owner and warehouse staff.

See [sample-business-intent.md](sample-business-intent.md).

## Requirement Agent Output

The Requirement Agent produces a Requirement Specification covering:

- Product catalog management (FR-001 through FR-005)
- Stock quantity tracking (FR-006 through FR-010)
- Stock movement recording (FR-011 through FR-015)
- Low-stock alert system (FR-016 through FR-020)
- Reporting (FR-021 through FR-025)

See [sample-requirement-specification.md](sample-requirement-specification.md).

## Product Manager Agent Output

The Product Manager Agent defines MVP scope with must-have features for catalog, stock tracking, movements, alerts, and basic reports. Should-have and could-have features are deferred.

See [sample-product-plan.md](sample-product-plan.md).

## UX/UI Agent Output

Mode 1 (UX): Personas for business owner and warehouse staff, user journeys for stock intake and low-stock response, wireframes with sample data (100 products, 10 categories, 20 suppliers, 500 transactions).

Mode 2 (UI): Brand-applied high-fidelity screens after UX approval.

See [sample-ux-ui-plan.md](sample-ux-ui-plan.md).

## Architecture Handover

The Enterprise Architect Agent uses approved requirements, product plan, and UX/UI handover to prepare architecture covering data model, security, and integration considerations.

## Approval Gates

| Gate | Status in Reference | Key Artifact |
|---|---|---|
| 0 — Environment Readiness | Passed | GitHub + Figma workspace ready |
| 1 — Requirement Approval | Passed | REQ-SPEC-inventory-management.md |
| 2 — Product Scope Approval | Passed | PRODUCT-PLAN-inventory-management.md |
| 3 — UX Approval | Passed | Wireframes with sample data |
| 4 — UI Approval | Passed | High-fidelity UI screens |
| 5 — Architecture Approval | Pending | Architecture blueprint in preparation |
| 6 — Release Approval | Future | After build phase |

## Decision Log Examples

See [sample-decision-log.md](sample-decision-log.md) for decisions made during the reference project walkthrough.
