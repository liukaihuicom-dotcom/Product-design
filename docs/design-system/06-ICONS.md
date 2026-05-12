# 06-ICONS.md

This file extends `ICONS.md` for Design System v2.0.

## Runtime System

- Assets: `src/assets/icons/`
- Component pattern: `src/components/ui/Icon.html`
- CSS classes: `.icon`, `.icon--asset`, `.icon-*`
- Tokens: `--icon-size-*`, `--icon-color-*`

## Platform Notes

| Platform | Rule |
|---|---|
| Web | 16px table/action icons, 20px default, 24px section icons |
| App | 20px default, 24px nav/card icons, 32px feedback icons |

## Status Rule

Status icons must appear with status text and semantic color. Never rely on color alone.
