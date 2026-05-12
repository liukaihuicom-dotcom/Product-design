---
name: production-ui-v2
description: Create production-grade Web/App HTML prototypes using Design System v2.0 platform rules, business components, API state mapping, and QA.
---

# Production UI v2 Skill

## Goal

Create platform-appropriate production UI HTML for Web, App, and H5 surfaces.

## Required Reading

Read these files before page work:

1. docs/design-system/00-OVERVIEW.md
2. docs/design-system/01-DESIGN.md
3. docs/design-system/02-TOKENS.md
4. docs/design-system/03-LAYOUT.md
5. docs/design-system/04-TYPOGRAPHY.md
6. docs/design-system/05-COMPONENTS.md
7. docs/design-system/06-ICONS.md
8. docs/design-system/07-FORM.md
9. docs/design-system/08-DATA_TABLE.md
10. docs/design-system/09-STATES.md
11. docs/design-system/10-PATTERNS.md
12. docs/design-system/11-BUSINESS_COMPONENTS.md
13. docs/design-system/12-API_STATE_MAP.md
14. docs/design-system/13-I18N.md
15. docs/design-system/14-ACCESSIBILITY.md
16. docs/design-system/15-MOTION.md
17. docs/design-system/17-UI_QA.md

## Platform Decision

Identify one target platform before generating:

- web-admin
- web-portal
- app-ios
- app-android
- h5-mobile

If not explicit, infer from `PAGE_BRIEF.md` and document the assumption.

## Process

1. Read `PAGE_BRIEF.md` if available.
2. Identify platform and page type.
3. Select platform tokens: `tokens.web.css` or `tokens.app.css`.
4. Select platform pattern: `src/patterns/web/` or `src/patterns/app/`.
5. Reuse base UI and business components.
6. Map UI state to `12-API_STATE_MAP.md`.
7. Add required states and abnormal copy.
8. Verify I18N, accessibility, responsive behavior, and UI QA.

## Output

- Web pages: `src/pages/web/[page-name]/production.html`
- App pages: `src/pages/app/[page-name]/production.html`
- For dual-platform tasks, output both and summarize separately.
