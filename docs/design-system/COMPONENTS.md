# COMPONENTS.md

## 0. Icon

### Purpose

Used to render all product icons consistently.

### Rules

- Icon usage must follow `docs/design-system/ICONS.md`.
- Use `src/components/ui/Icon.html` patterns and `.icon-*` classes for all icon rendering in HTML prototypes.
- Do not inline random SVG icons inside pages.
- Functional icons should use `currentColor`.
- Brand icons may retain original colors.
- Important actions must include text labels.

### Sizes

| Size | Token |
|---|---|
| xs | `--icon-size-xs` |
| sm | `--icon-size-sm` |
| md | `--icon-size-md` |
| lg | `--icon-size-lg` |
| xl | `--icon-size-xl` |
| 2xl | `--icon-size-2xl` |
| 3xl | `--icon-size-3xl` |

## 1. Button

### Purpose

Used for user actions.

### Variants

| Variant | Usage |
|---|---|
| primary | Main action |
| secondary | Secondary action |
| ghost | Low-emphasis action |
| danger | Destructive or high-risk action |

### Sizes

| Size | Height |
|---|---:|
| sm | 32px |
| md | 40px |
| lg | 48px |

### Rules

- One primary button per main action area.
- Destructive actions must use `danger`.
- Disabled buttons must visibly reduce emphasis and block interaction.
- Loading buttons must keep width stable.
- Financial submission actions should use clear text: "Submit for Review", "Confirm Withdrawal", "Continue Verification".

### Token Mapping

| Property | Token |
|---|---|
| Height | `--button-height-md` |
| Radius | `--button-radius` |
| Primary background | `--color-brand-primary` |
| Danger background/text | `--color-danger` |

## 2. Card

### Purpose

Used to group related content.

### Variants

| Variant | Usage |
|---|---|
| default | Normal content group |
| elevated | Important summary card |
| interactive | Clickable card |
| warning | Risk/compliance notice |
| success | Success feedback |

### Rules

- Card must have consistent padding.
- Header and body must be visually separated.
- Avoid heavy shadows.
- Summary cards can use subtle shadow.
- Financial information must be aligned for scanning.

### Token Mapping

| Property | Token |
|---|---|
| Background | `--color-bg-surface` |
| Border | `--color-border-default` |
| Radius | `--card-radius` |
| Padding | `--card-padding` |
| Shadow | `--shadow-card` |

## 3. Input

### Purpose

Used for forms, filters, search, and financial input.

### States

- default
- focused
- disabled
- error
- success
- loading

### Rules

- Every input must have a label.
- Helper text should explain requirements.
- Error message must appear below the field.
- Financial amount input should display currency clearly.
- Do not hide validation until final submit if the error is obvious.

## 4. Select

### Purpose

Used for account, currency, status, reviewer, region, and filter choices.

### Rules

- The selected value must be readable at rest.
- Placeholder text must describe the expected choice.
- Disabled selects must include nearby reason text when the blocked state affects workflow.
- For currency/account choices, include enough metadata to prevent ambiguity.

## 5. StatusBadge

### Purpose

Used to show business status.

### Variants

| Variant | Usage |
|---|---|
| success | Approved, completed, successful |
| warning | Pending, reviewing, action required |
| danger | Failed, rejected, blocked |
| neutral | Draft, inactive, archived |
| info | Processing, submitted |

### Rules

- Status label must be concise.
- Badge color must match semantic meaning.
- Risk statuses must include explanation nearby.
- Do not rely on color alone; use text.

## 6. Alert

### Purpose

Used for risk, compliance, review, success, and system notices.

### Rules

- Alert text must say what happened and what the user can do next.
- Warning and danger alerts must be visible before final submission.
- Do not use alerts as decorative banners.

## 7. Table

### Purpose

Used for account lists, transaction records, review queues, partner lists.

### Rules

- Support empty state.
- Support loading state.
- Support error state.
- Important columns should appear first.
- Row actions should be placed at the right side.
- Risk/status column should be visually scannable.
- Financial numbers should be right-aligned.
- Long IDs should support copy action.

## 8. Modal

### Purpose

Used for confirmation, risk warnings, focused forms.

### Rules

- Do not overuse modals for normal navigation.
- High-risk actions require explicit confirmation.
- Modal must have clear title, description, primary action, secondary action.
- Destructive confirmation must use `danger`.

## 9. EmptyState

### Purpose

Used when there is no data.

### Rules

- Explain why the area is empty.
- Provide next action if available.
- Avoid decorative-only empty states.
- For compliance or review flows, explain whether user needs to act.

## 10. LoadingState

### Purpose

Used while data or actions are in progress.

### Rules

- Keep layout dimensions stable.
- Disable duplicate submission.
- For financial actions, describe what is being processed.

## 11. ErrorState

### Purpose

Used when something failed.

### Rules

- Explain what happened.
- Tell the user what they can do next.
- Provide retry action when possible.
- For financial operations, avoid vague error messages.
