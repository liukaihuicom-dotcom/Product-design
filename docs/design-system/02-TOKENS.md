# 02-TOKENS.md

## Token Architecture

| Layer | Description |
|---|---|
| L1 Base Tokens | Raw values: color, spacing, radius, typography. |
| L2 Semantic Tokens | Purpose-based values: bg-page, text-primary, border-default. |
| L3 Component Tokens | Component-specific values: button-height-md, card-padding. |
| L4 Platform Tokens | Web/App-specific remapping. |
| L5 Theme Tokens | Light/Dark/Brand theme remapping. |

## Token Modes

| Mode | Values |
|---|---|
| Platform | web / app / h5 |
| Theme | light / dark |
| Density | compact / comfortable / spacious |
| Brand | default / broker-a / broker-b |
| Radius | sharp / default / rounded |

## Platform Spacing

| Token | Web | App |
|---|---:|---:|
| `--page-padding` | 32px | 16px |
| `--section-gap` | 24px | 20px |
| `--card-padding` | 20px | 16px |
| `--field-gap` | 12px | 12px |
| `--list-item-gap` | 12px | 8px |
| `--bottom-action-padding` | 24px | 16px |

## Platform Component Size

| Component | Web | App |
|---|---:|---:|
| Button md | 40px | 44px |
| Button lg | 48px | 52px |
| Input md | 40px | 48px |
| List item | 48px | 56px |
| Touch target | 40px | 44px minimum |

## Runtime Files

- `src/styles/tokens.css`: base and semantic tokens.
- `src/styles/tokens.web.css`: web platform overrides.
- `src/styles/tokens.app.css`: app / mobile platform overrides.
- `src/styles/themes.light.css`: light theme mapping.
- `src/styles/themes.dark.css`: dark theme mapping.

## Compatibility

The existing `TOKENS.md` remains available for v1 workflows. New v2 pages should use the numbered token docs plus the runtime platform token files.
