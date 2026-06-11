# Product Plan — Inventory Management System

File path: docs/03-product-management/PRODUCT-PLAN-inventory-management.md

## 1. Product Objective

Deliver an MVP inventory management system that enables a small business to track
products, stock, movements, alerts, and basic reports.

## 2. Input Requirements Used

| Requirement ID     | Requirement Summary         |
| ------------------ | --------------------------- |
| FR-001 to FR-005   | Product catalog management  |
| FR-006 to FR-010   | Stock quantity tracking     |
| FR-011 to FR-015   | Stock movement recording    |
| FR-016 to FR-020   | Low-stock alert system      |
| FR-021 to FR-025   | Reporting                   |
| NFR-001 to NFR-005 | Non-functional requirements |

## 3. MVP Scope

MVP includes product catalog, stock tracking, stock movements, low-stock alerts, and
basic reports/dashboard. Excludes barcode scanning, multi-warehouse, PO management, and
accounting integration.

## 4. Must-Have Features

| Feature ID | Feature          | Linked Requirement IDs   | Business Value           | User Value                  |
| ---------- | ---------------- | ------------------------ | ------------------------ | --------------------------- |
| F-001      | Product Catalog  | FR-001 to FR-005         | Central product registry | Find and manage products    |
| F-002      | Stock Dashboard  | FR-006, FR-009, FR-025   | Inventory visibility     | See stock at a glance       |
| F-003      | Stock Movements  | FR-011 to FR-015         | Accurate inventory       | Record receipts and sales   |
| F-004      | Low-Stock Alerts | FR-016 to FR-018, FR-020 | Prevent stockouts        | Timely reorder notification |
| F-005      | Basic Reports    | FR-021, FR-022, FR-024   | Operational insight      | Export and review data      |

## 5. Should-Have Features

| Feature ID | Feature       | Linked Requirement IDs | Business Value         | User Value                  |
| ---------- | ------------- | ---------------------- | ---------------------- | --------------------------- |
| F-006      | Email Alerts  | FR-019                 | Proactive notification | Alerts without login        |
| F-007      | CSV Export    | FR-023                 | Data portability       | Share reports externally    |
| F-008      | Stock Filters | FR-010                 | Faster lookup          | Filter by category/supplier |

## 6. Could-Have Features

| Feature ID | Feature          | Linked Requirement IDs | Business Value    | User Value           |
| ---------- | ---------------- | ---------------------- | ----------------- | -------------------- |
| F-009      | Barcode Scanning | Out of scope           | Faster data entry | Scan instead of type |

## 7. Deferred / Out-of-Scope Features

| Feature                | Reason Deferred                   |
| ---------------------- | --------------------------------- |
| Multi-warehouse        | Complexity exceeds MVP need       |
| Purchase orders        | Separate module for v2            |
| Accounting integration | Requires partner evaluation       |
| Mobile native app      | Web-responsive sufficient for MVP |

## 8. Feature Priority Matrix

| Feature ID | Priority | Complexity | Business Value | MVP Decision  |
| ---------- | -------- | ---------- | -------------- | ------------- |
| F-001      | Must     | Medium     | High           | Include       |
| F-002      | Must     | Medium     | High           | Include       |
| F-003      | Must     | High       | High           | Include       |
| F-004      | Must     | Medium     | High           | Include       |
| F-005      | Must     | Low        | High           | Include       |
| F-006      | Should   | Low        | Medium         | Defer to v1.1 |
| F-007      | Should   | Low        | Medium         | Defer to v1.1 |

## 9. Release Plan

| Release    | Features            | Goal                       | Human Approval Needed |
| ---------- | ------------------- | -------------------------- | --------------------- |
| MVP (v1.0) | F-001 to F-005      | Core inventory management  | Yes — Gate 2          |
| v1.1       | F-006, F-007, F-008 | Enhanced alerts and export | Yes                   |

## 10. User Value Mapping

| User Role       | Value Delivered                       |
| --------------- | ------------------------------------- |
| Business Owner  | Dashboard, alerts, reports            |
| Warehouse Staff | Fast movement recording, stock lookup |

## 11. Success Metrics

| Metric                  | Target              | Measurement Method                |
| ----------------------- | ------------------- | --------------------------------- |
| Product registration    | 100% within 30 days | Count active products vs total    |
| Stockout reduction      | 50% decrease        | Compare alerts acted vs stockouts |
| Movement recording time | Under 30 seconds    | Timed user test                   |

## 12. Product Trade-Offs

- Email alerts deferred to v1.1 to reduce MVP complexity
- Single warehouse assumed to simplify data model
- Web-only delivery avoids mobile app development cost

## 13. Human Scope Decisions Required

- Confirm MVP scope excludes multi-warehouse (approved)
- Confirm email alerts deferred to v1.1 (approved)

## 14. GitHub Feature Issue List

- Issue F-001: Product Catalog
- Issue F-002: Stock Dashboard
- Issue F-003: Stock Movements
- Issue F-004: Low-Stock Alerts
- Issue F-005: Basic Reports

## 15. Product-to-UX Handover

MVP features F-001 through F-005 require UX design for: product list/detail, stock
dashboard, movement form, alert panel, and report views. Sample data: 100 products, 10
categories, 20 suppliers, 500 transactions, 20 alerts, 10 users.

## 16. Product-to-Architecture Handover

Five feature modules map to catalog, inventory, movements, alerts, and reporting
services. RBAC with business owner and warehouse staff roles. Single-warehouse data
model.
