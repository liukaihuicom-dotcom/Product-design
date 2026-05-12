# Dual Platform Checklist

## Web

- Uses `data-platform="web"`.
- Loads `tokens.css`, `tokens.web.css`, theme CSS, globals, and components.
- Uses table patterns for dense records.
- Uses side helper panels for complex compliance explanation.
- Avoids mobile-only bottom sheet / sticky CTA unless the viewport requires it.

## App / H5

- Uses `data-platform="app"` or `data-platform="h5"`.
- Loads `tokens.css`, `tokens.app.css`, theme CSS, globals, and components.
- Uses card lists instead of dense tables.
- Uses sticky bottom CTA for primary form actions.
- Uses bottom sheet / selector patterns for complex choices.

## Shared

- Same business logic and API state mapping.
- Same token semantics.
- Same icon semantics.
- Same abnormal state copy requirements.
- Separate QA summaries.
