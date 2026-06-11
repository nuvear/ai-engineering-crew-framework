# UX/UI Plan — Inventory Management System

## Product Scope Used

MVP features F-001 through F-005 from the approved Product Plan.

## Personas

**Maria — Business Owner:** Needs dashboard visibility, alert response, and reports.
Uses the system 2–3 times daily.

**James — Warehouse Staff:** Needs fast stock movement recording and product lookup.
Uses the system continuously during shifts.

## User Journeys

1. **Daily Stock Check:** James logs in → views stock dashboard → records receipt →
   system updates quantities
2. **Low-Stock Response:** Maria sees alert on dashboard → reviews affected products →
   initiates reorder externally
3. **Weekly Report:** Maria generates inventory report → filters by date → exports for
   review

## Task Flows

- Add product → assign category/supplier → set reorder point → save
- Record movement → select product → enter quantity/type → confirm → audit logged
- View alerts → acknowledge → optionally adjust reorder point

## Information Architecture

```text
Dashboard
├── Stock Overview
├── Active Alerts
└── Recent Movements
Products
├── Product List
├── Product Detail
└── Categories
Movements
├── Record Movement
└── Movement History
Reports
├── Inventory Report
└── Movement Report
Settings
└── Users (admin only)
```

## Screen Inventory

| Screen           | Feature      | Priority |
| ---------------- | ------------ | -------- |
| Dashboard        | F-002, F-004 | Must     |
| Product List     | F-001        | Must     |
| Product Detail   | F-001        | Must     |
| Record Movement  | F-003        | Must     |
| Movement History | F-003        | Must     |
| Alert Panel      | F-004        | Must     |
| Inventory Report | F-005        | Must     |

## Wireframe Summary

Low-fidelity wireframes created in Figma pages 04 (Wireframes) and 05 (Clickable
Prototype). All screens populated with sample data.

## Sample Data

```text
100 products
10 categories
20 suppliers
500 stock transactions
20 low-stock alerts
10 users across different roles
```

## User Acceptance Scenarios

1. James records a stock receipt of 50 units for Product SKU-0042 and sees updated
   quantity on dashboard
2. Maria views active alerts and acknowledges alert for Product SKU-0015 below reorder
   point
3. Maria generates inventory report filtered to last 7 days

## Figma Link

Figma project: Inventory Management System — pages 00–09 per standard structure.

## UX Approval Checklist

- [x] Personas exist
- [x] User journey exists
- [x] Task flows exist
- [x] Information architecture exists
- [x] Wireframes exist with sample data
- [x] User acceptance scenarios exist
- [x] Figma prototype link exists

## UX-to-Architecture Handover

Five primary screen groups map to five feature modules. Dashboard aggregates data from
inventory and alert services. Movement form requires real-time stock validation. RBAC
hides Settings from warehouse staff.
