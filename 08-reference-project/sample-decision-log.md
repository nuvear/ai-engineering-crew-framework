# Sample Decision Log — Inventory Management Reference Project

## DEC-REF-001: Single Warehouse Assumption

**Date:** 2026-01-15 **Decision:** MVP assumes single warehouse location. **Reason:**
Business operates from one location; multi-warehouse adds complexity without MVP value.
**Impact:** Simplified data model; multi-warehouse deferred to future release.

## DEC-REF-002: Email Alerts Deferred

**Date:** 2026-01-20 **Decision:** Email alert notifications deferred from MVP to v1.1.
**Reason:** In-app alerts sufficient for MVP; email integration adds setup complexity.
**Impact:** FR-019 marked as should-have for v1.1.

## DEC-REF-003: Web-Only Delivery

**Date:** 2026-02-01 **Decision:** MVP delivered as responsive web application, no
native mobile app. **Reason:** Warehouse staff have browser access on existing devices;
native app cost not justified for MVP. **Impact:** UX designed responsive; mobile-native
features out of scope.
