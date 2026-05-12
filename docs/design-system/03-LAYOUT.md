# 03-LAYOUT.md

## Layout Goal

Define Web/App layout rules so Codex does not use the same layout for all platforms.

## Web Admin

| Area | Rule |
|---|---|
| Sidebar | 240px default width |
| Topbar | 64px height |
| Page padding | 32px |
| Content max width | No strict max for admin tables |
| Main grid | 12 columns |
| Card gap | 24px |
| Table layout | Preferred for data-heavy pages |

## Web Portal

| Area | Rule |
|---|---|
| Header | 64px / 72px |
| Page max width | 1200px |
| Page padding | 32px desktop, 20px tablet |
| Content grid | 12 columns |
| Form max width | 640px |
| Detail page max width | 960px |

## App Layout

| Area | Rule |
|---|---|
| Safe area | Respect top and bottom safe area |
| Page padding | 16px |
| Header height | 56px |
| Bottom tab | 56px - 64px |
| Sticky bottom action | Required for primary form actions |
| Cards | Full width, 16px radius |
| Lists | Card list or grouped list, avoid dense tables |

## Responsive Breakpoints

| Breakpoint | Width | Usage |
|---|---:|---|
| mobile | 375px | App / H5 |
| tablet | 768px | Tablet / narrow web |
| desktop | 1200px | Standard web |
| wide | 1440px | Large admin display |

## Web vs App Decision

| Scenario | Web Pattern | App Pattern |
|---|---|---|
| Record list | Table | Card list |
| Filter | Horizontal filter bar | Bottom sheet |
| Form action | Header / footer action | Sticky bottom CTA |
| Detail page | Two-column layout | Single-column stacked |
| Modal | Center modal | Bottom sheet |
| Navigation | Sidebar / top nav | Bottom tab / app header |
| Batch action | Toolbar | Multi-select bottom action |
