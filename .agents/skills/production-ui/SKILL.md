---
name: production-ui-upgrade
description: Upgrade low-fidelity product prototype HTML into production-grade UI HTML using the project design system.
---

# Production UI Upgrade Skill

## Goal

Convert product-flow HTML into production-grade UI design HTML.

## Required Files

Before making changes, read:

- docs/design-system/DESIGN.md
- docs/design-system/TOKENS.md
- docs/design-system/COMPONENTS.md
- docs/design-system/ICONS.md
- docs/design-system/PATTERNS.md
- docs/design-system/STATES.md
- docs/design-system/UI_QA.md

## Process

1. Audit the current page.
2. Identify page type:
   - dashboard
   - list
   - detail
   - form
   - review center
   - wallet / funds page
   - onboarding / KYC page
   - account management page
3. Check whether business logic is complete.
4. Improve information hierarchy.
5. Replace ad-hoc styles with tokens.
6. Replace random icons with documented icon assets.
7. Replace repeated UI with reusable components.
8. Add missing states.
9. Improve responsive behavior.
10. Run UI QA checklist.
11. Summarize what changed.

## Rules

- Do not change business logic unless requested.
- Do not invent random visual styles.
- Do not use generic AI-looking UI.
- Do not create one-off components when a reusable component is appropriate.
- Use financial SaaS design principles: clear, stable, professional, trustworthy.

## Output

- Production-grade responsive HTML.
- Reusable UI components.
- Token-driven CSS.
- Complete business states.
- QA summary.
