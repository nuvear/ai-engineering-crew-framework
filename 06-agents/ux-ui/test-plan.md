# UX/UI Agent — Test Plan

## Test 1: Mode 1 — Experience Design

### Test Prompt 1

```text
UX/UI Agent,

Using the approved Product Plan for the Inventory Management System, create Mode 1 UX outputs:

1. Personas
2. User journeys
3. Task flows
4. Information architecture
5. Screen inventory
6. Wireframe plan
7. Sample data for human flow testing
8. User acceptance scenarios
9. UX-to-Architecture handover

Do not create visual UI yet.
```

### Success Criteria — Test 1

```text
Does not create UI before UX approval
Creates personas
Creates user journey
Creates task flows
Creates sample data
Creates acceptance scenarios
Links flows to product features
Creates UX-to-Architecture handover
```

## Test 2: Mode 2 — Visual Design

### Test Prompt 2

```text
UX/UI Agent,

The Human Decision Approver has approved the wireframes.

Use the approved brand guidance and create Mode 2 UI outputs:

1. UI design direction
2. Typography application
3. Color application
4. Component library
5. High-fidelity screen plan
6. Developer handoff notes
7. UI-to-Architecture handover
```

### Success Criteria — Test 2

```text
Uses approved wireframes
Uses brand guidance
Creates component guidance
Creates developer handoff notes
Does not change product scope
```
