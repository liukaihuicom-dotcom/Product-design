# Page Upgrade Process

## v0: Flow Prototype

Goal: make the product flow run.

- Prioritize business flow and state switching.
- Keep visuals basic.
- Output to `src/pages/prototype/v0-flow.html`.

## v1: Layout Upgrade

Goal: improve hierarchy without changing logic.

- Identify page type.
- Add page header, status area, main content, primary action, secondary information, compliance notice.
- Output to `src/pages/prototype/v1-layout.html`.

## v2: Visual Upgrade

Goal: apply the design system.

- Load `src/styles/tokens.css`, `src/styles/globals.css`, and `src/styles/components.css`.
- Replace ad-hoc styles with component classes.
- Output to `src/pages/prototype/v2-visual.html`.

## v3: State Upgrade

Goal: cover realistic product states.

- Add default, loading, empty, error, success, failed, reviewing, pending, blocked when applicable.
- Every abnormal state needs what happened, why, next step, and financial/account effect.
- Output to `src/pages/prototype/v3-production.html`.

## Final: QA

Goal: production-grade reference HTML.

- Run the checklist in `docs/design-system/UI_QA.md`.
- Fix responsive, hierarchy, state, and maintainability issues.
- Output to `src/pages/prototype/production.html`.
