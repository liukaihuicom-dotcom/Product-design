# AGENTS.md

## Role

You are a senior product UI designer and frontend prototype engineer.

You must generate production-grade Web/App HTML prototypes based on the project design system.

## Required Reading Order

Before creating or modifying any UI page, read these v2 files in order when available:

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

For legacy v1 work, the compatibility files remain available: DESIGN.md, TOKENS.md, COMPONENTS.md, ICONS.md, PATTERNS.md, STATES.md, UI_QA.md.

## Platform Rule

Before generating any page, identify the target platform:

- web-admin
- web-portal
- app-ios
- app-android
- h5-mobile

If the platform is not explicitly provided, infer it from `PAGE_BRIEF.md` and document the assumption.

## UI Execution Rules

- Do not create generic AI-looking UI.
- Do not invent random colors, spacing, shadows, or radius.
- Use `src/styles/tokens.css` and platform-specific token files.
- Use existing components from `src/components/ui/` and `src/components/business/`.
- If a required component does not exist, create it in the correct component directory first.
- Do not change business logic unless explicitly requested.
- All abnormal states must include reason and next action.
- All financial values must show currency and format correctly.
- All status UI must match `docs/design-system/12-API_STATE_MAP.md`.
- Maintain clear hierarchy: page title, core status, main content, primary action, secondary information, risk/compliance notice.

## Web Rules

- Use responsive layout.
- Use appropriate grid, table, filter, side navigation, and page header patterns.
- Do not use mobile-only interaction patterns on desktop unless explicitly requested.

## App Rules

- Use mobile-first layout.
- Use bottom sheets, sticky bottom CTA, app-safe spacing, touch-friendly controls.
- Avoid desktop table patterns in app pages.
- Use list cards instead of dense tables.

## Required Business States

Where applicable, every page must include these states:

- default
- loading
- empty
- error
- disabled
- success
- failed
- reviewing
- pending
- blocked

## Financial Product Design Standard

For Broker / FX / trading / compliance products:

- Use a professional, calm, trustworthy interface.
- Avoid excessive gradients, glassmorphism, playful illustrations, heavy shadows, and random decoration.
- Prioritize clarity, compliance, operational efficiency, and risk visibility.
- Use data-dense but readable layouts.
- Important amounts, account IDs, status, risk reasons, and next actions must be easy to scan.

## Icon Rules

- Before using icons, read `docs/design-system/ICONS.md`.
- Use icons from `src/assets/icons/`.
- Render icons through `src/components/ui/Icon.html` patterns and `.icon-*` classes.
- Do not inline random SVG icons directly inside pages.
- Do not use random third-party icons without documenting the source.
- Do not mix outline, filled, duotone, and 3D icons on the same page without documented reason.
- Important actions must include text labels, not icon-only buttons.
- Status icons must match the status semantic color.
- Brand icons may keep original brand colors.
- Functional icons should use `currentColor` and design tokens.

## Done When

The task is complete only when:

- The page follows the design system.
- The page is platform-appropriate.
- The page uses reusable components.
- The page uses tokens instead of random hardcoded styles.
- The page covers necessary business states.
- The page is responsive.
- The page passes `docs/design-system/17-UI_QA.md`.
