# 15-MOTION.md

## Motion Goal

Motion should communicate state changes, not decorate.

## Recommended Motion

| Scenario | Motion |
|---|---|
| Button loading | Spinner, preserve width |
| Page loading | Skeleton |
| Bottom sheet | Slide up |
| Modal | Fade + scale |
| Status change | Subtle fade |
| Success feedback | Brief icon transition |
| Error | No shake by default; use clear message |

## Duration

| Type | Duration |
|---|---:|
| Fast | 120ms |
| Normal | 180ms |
| Slow | 240ms |
| Page transition | 240ms |

## Rules

- Do not use bouncy motion in financial workflows.
- Avoid playful animation for compliance states.
- Loading state must not hide important context.
- Respect reduced motion where possible.
