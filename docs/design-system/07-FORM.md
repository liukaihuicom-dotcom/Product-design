# 07-FORM.md

## Form Goal

Forms must reduce user errors and clearly explain compliance requirements.

## Form Structure

1. Page title.
2. Short explanation.
3. Step indicator if multi-step.
4. Field groups.
5. Compliance / risk notice.
6. Primary action.
7. Secondary action.
8. Feedback state.

## Field Rules

| Field | Rule |
|---|---|
| Label | Required |
| Placeholder | Helpful but not a replacement for label |
| Helper text | Use for rules and requirements |
| Error text | Show below field |
| Disabled field | Explain why disabled if important |
| Required mark | Use consistently |
| Optional field | Mark as optional when needed |

## Amount Input

| Rule | Description |
|---|---|
| Currency visible | Always show currency |
| Min/max visible | Show limits near input |
| Fee visible | Show fee before submit |
| Available balance visible | Required for withdrawal |
| Decimal rule | Match currency precision |
| Error timing | Show obvious errors before submit |

## Upload Field

| Rule | Description |
|---|---|
| File requirements | Show type, size, count |
| Preview | Show uploaded image / document |
| Upload progress | Required |
| Failed upload | Show reason and retry |
| Replace file | Must be supported |
| Delete file | Must require confirmation if submitted |

## Mobile Form Rules

- Use single-column layout.
- Use sticky bottom CTA.
- Avoid too many fields on one screen.
- Use bottom sheet for selectors.
- Use step-by-step flow for KYC and verification.
- Keep compliance explanation close to related fields.

## Web Form Rules

- Use form groups.
- Use side helper panel for complex compliance explanation.
- Long forms should use sections.
- Confirmation modals required for high-risk financial operations.
