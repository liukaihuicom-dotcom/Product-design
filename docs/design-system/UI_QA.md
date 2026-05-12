# UI_QA.md

## 1. Production UI Checklist

| Check Item | Pass Standard |
|---|---|
| Visual consistency | Uses tokens, not random visual values |
| Component consistency | Uses components from `src/components/ui/` |
| Icon consistency | Uses `docs/design-system/ICONS.md`, `src/assets/icons/`, and `.icon-*` classes |
| Hierarchy | User can identify current status and next action within 3 seconds |
| CTA clarity | Main action is obvious; secondary actions are lower emphasis |
| State coverage | Required states are included |
| Responsive | Mobile and desktop layouts are usable |
| Financial clarity | Amounts, currencies, accounts, and statuses are readable |
| Compliance clarity | Risk and review requirements are clearly explained |
| Accessibility | Color is not the only indicator; contrast is readable |
| Maintainability | Repeated UI has been componentized |

## 2. Common Failure Signs

The UI is not production-grade if:

- It looks like a generic dashboard template.
- It uses random gradients or heavy shadows.
- Every card has the same visual weight.
- There are too many primary buttons.
- Empty / loading / error states are missing.
- Icons are random, mixed-style, or embedded directly in pages without the icon system.
- Financial values are not aligned.
- Risk messages are hidden or vague.
- The mobile layout is just a squeezed desktop layout.
- Components are copied repeatedly instead of reused.

## 3. Final Review Prompt

Before finishing, Codex must answer:

1. Which design-system files were used?
2. Which components were reused?
3. Which components were newly created?
4. Which icon assets were used?
5. Which business states were covered?
6. Which UI QA issues were found and fixed?
7. What still needs manual design review?
