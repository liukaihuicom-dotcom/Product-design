# 05-COMPONENTS.md

This file extends `COMPONENTS.md` for Design System v2.0.

## Component Layers

| Layer | Path | Purpose |
|---|---|---|
| Base UI | `src/components/ui/` | Button, Card, Input, Select, Table, Modal, Icon, Alert |
| Business UI | `src/components/business/` | AccountCard, AmountInput, RiskNotice, VerificationStatus, Timeline |
| Page Patterns | `src/patterns/web/`, `src/patterns/app/` | Platform-specific layouts |

## Cross-Platform Component Rule

- Keep semantics shared across Web/App.
- Let platform token files adjust density, touch target, padding, and radius.
- Do not copy a dense Web table into App. Use mobile business components instead.

## Required Base Components

- Icon
- Button
- Input
- Select
- Card
- Alert
- StatusBadge
- Table
- Modal / Bottom sheet pattern
- EmptyState
- LoadingState
- ErrorState

## Component Acceptance

Each component must define purpose, variants, sizes, states, token usage, accessibility, and platform-specific behavior.
