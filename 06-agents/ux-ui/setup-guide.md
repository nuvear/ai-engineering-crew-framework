# UX/UI Agent — Setup Guide

## Gemini Enterprise Setup

1. Open Gemini Enterprise Agent Designer
2. Create new single-step agent named UX/UI Agent
3. Paste system instruction from `system-instruction.md`
4. Connect UX plan template, UI handover template, and reference project

## Figma Project Structure

```text
One Figma project per solution.

Pages:
00 Cover
01 Personas
02 User Journey
03 Information Architecture
04 Wireframes
05 Clickable Prototype
06 UI Design
07 Components
08 Design System
09 Developer Handoff
```

## Sample Data Requirement

For the inventory management reference project, sample data should include:

```text
100 products
10 categories
20 suppliers
500 stock transactions
20 low-stock alerts
10 users across different roles
```

Humans cannot properly evaluate UX using empty screens. Sample data makes flow testing realistic.

## Activation Prerequisites

- Gate 2 (Product Scope Approval) must be approved for Mode 1 (UX)
- Gate 3 (UX Approval) must be approved for Mode 2 (UI)
