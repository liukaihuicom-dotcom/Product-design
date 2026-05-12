# 08-DATA_TABLE.md

## Data Table Goal

Web admin and portal pages need dense but readable data presentation.

## Table Structure

1. Page header.
2. Summary metrics.
3. Filter bar.
4. Table.
5. Pagination.
6. Bulk action if needed.
7. Empty / loading / error states.

## Column Rules

| Column Type | Rule |
|---|---|
| Status | Use StatusBadge with text |
| Amount | Right align, show currency |
| Account ID | Monospace, copy action |
| User | Show name + ID / email |
| Time | Use consistent date format |
| Action | Right side, avoid too many buttons |
| Risk | Use badge + reason tooltip |

## Filter Rules

| Filter Type | Web | App |
|---|---|---|
| Keyword search | Inline search input | Search page / top input |
| Status filter | Select / segmented | Bottom sheet |
| Date range | Date picker | Bottom sheet date picker |
| Advanced filter | Popover / drawer | Full-screen filter / bottom sheet |

## Table States

| State | Required UI |
|---|---|
| Loading | Skeleton rows |
| Empty | Empty state + reset filter action |
| Error | Error message + retry |
| Partial loading | Keep existing rows, show small loading |
| No permission | Explain permission issue |
| High risk row | Highlight with risk badge |

## Mobile Alternative

Do not convert dense web tables directly into mobile tables. Use card lists with identity, status, key amount, secondary metadata, and row action.
