# Production UI HTML Design System

This workspace implements the v1 design-system plan and the v2 Web/App upgrade plan from `production-design-system-v2-web-app-codex.md`.

Visual direction: Wise-inspired financial UI. The system uses bright green primary actions, forest-green text, green-tinted neutral surfaces, rounded controls, and clear money/status hierarchy without using Wise logos or protected brand assets.

## What Is Included

- `AGENTS.md`: execution rules and required reading order for Codex.
- `docs/design-system/`: v1 compatibility docs plus v2 numbered docs for Web/App work.
- `src/styles/tokens.css`: CSS variable source of truth.
- `src/styles/tokens.web.css` / `tokens.app.css`: platform token overrides.
- `src/styles/themes.light.css` / `themes.dark.css`: theme overrides.
- `src/styles/globals.css`: base layout and typography helpers.
- `src/styles/components.css`: reusable component class library for runnable HTML.
- `src/components/ui/`: P0 component snippets and usage examples.
- `src/components/business/`: Broker business component snippets.
- `src/assets/icons/`: token-friendly SVG icon assets organized by category.
- `src/patterns/web/` and `src/patterns/app/`: platform-specific page skeletons.
- `.agents/skills/production-ui/`: repeatable workflow for upgrading prototypes.
- `.agents/skills/production-ui-v2/`: Web/App workflow for platform-specific production UI.
- `src/pages/prototype/`: v0 to final prototype upgrade example.

## Preview

Open the final reference page directly:

```txt
src/pages/prototype/production.html
```

Or run a static server from the project root:

```bash
python3 -m http.server 4173
```

Then visit:

```txt
http://127.0.0.1:4173/src/pages/prototype/production.html
```

## Workflow

1. Build or place the functional prototype at `src/pages/prototype/v0-flow.html`.
2. Use `docs/design-system/PATTERNS.md` to create `v1-layout.html`.
3. Apply `src/styles/tokens.css`, `globals.css`, and `components.css` to create `v2-visual.html`.
4. Use `docs/design-system/STATES.md` to create `v3-production.html`.
5. Use `docs/design-system/UI_QA.md` to create `production.html`.

## V2 Workflow

1. Create or read `PAGE_BRIEF.md`.
2. Identify platform: `web-admin`, `web-portal`, `app-ios`, `app-android`, or `h5-mobile`.
3. Read numbered docs from `00-OVERVIEW.md` through `17-UI_QA.md`.
4. Load platform tokens: `tokens.web.css` for Web, `tokens.app.css` for App/H5.
5. Reuse `src/components/ui/` and `src/components/business/`.
6. Output Web pages under `src/pages/web/` and App pages under `src/pages/app/`.

## Current Example

Because this workspace did not contain an existing product prototype or `PRODUCT.md`, the included example uses a Broker compliance review queue. It covers:

- default review queue
- loading
- empty
- error
- disabled
- success
- failed
- reviewing
- pending
- blocked

The example is intentionally finance-oriented: statuses, risk reasons, amount alignment, blocked funds language, and reviewer actions are all visible in the first production reference.

## Icons

Icon guidelines live in `docs/design-system/ICONS.md`. Assets are stored under `src/assets/icons/` and rendered in HTML prototypes with `.icon`, `.icon--asset`, and semantic classes such as `icon-risk`, `icon-status-blocked`, or `icon-download`.
