# 16-VERSIONING.md

## Versioning Goal

Design system changes must be controlled so existing pages do not break unexpectedly.

## Version Format

Use semantic versioning: MAJOR.MINOR.PATCH.

| Type | Example | Meaning |
|---|---|---|
| PATCH | 2.0.1 | Bug fix, copy update, minor token correction |
| MINOR | 2.1.0 | New component, new pattern, backward compatible |
| MAJOR | 3.0.0 | Breaking token / component / layout change |

## Change Categories

| Category | Example | Required Action |
|---|---|---|
| Token added | Add new color token | Document only |
| Token changed | Change primary color | Visual regression review |
| Token removed | Remove old spacing token | Migration required |
| Component added | Add AccountCard | Document usage |
| Component changed | Change Button height | Check impacted pages |
| Component deprecated | Replace old Alert | Provide migration path |

## Deprecation Rule

Deprecated components must remain available for at least one release cycle.

## Changelog Template

```md
# CHANGELOG

## v2.0.0

### Added
- Web/App platform token modes
- Layout system
- Business components
- API state mapping

### Changed
- Component usage rules
- Form validation rules

### Deprecated
- None

### Migration
- Replace random page-level icon SVG with Icon component.
```
