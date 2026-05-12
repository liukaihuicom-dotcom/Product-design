# ICONS.md

## 1. Icon Library Role

Icons are part of the design system. They are not decorative files scattered through pages.

| Goal | Standard |
|---|---|
| Visual consistency | Use one icon family and one stroke style per product surface. |
| Semantic clarity | Icons must help users understand an action, status, object, or risk. |
| Reuse | Render icons through `src/components/ui/Icon.html` patterns and `.icon-*` classes. |
| Maintainability | Icons use category folders, kebab-case names, currentColor, and shared tokens. |
| Delivery | Designers, Codex, and frontend engineers can tell where icons live and how to use them. |

## 2. Directory Structure

```txt
src/assets/icons/
├── system/
├── outline/
├── filled/
├── status/
├── finance/
├── broker/
├── verification/
├── payment/
├── brand/
└── illustration/
```

## 3. Style Standard

| Item | Standard |
|---|---|
| Primary style | Outline |
| Stroke width | `var(--icon-stroke-width)` conceptually, exported SVG uses `1.75` |
| Stroke caps | Rounded |
| Stroke joins | Rounded |
| Default size | `--icon-size-md` / 20px |
| Default color | `--icon-color-default` |
| Mood | Professional, clear, restrained, financial SaaS |

## 4. Tokens

Icon tokens live in `src/styles/tokens.css`:

| Token | Purpose |
|---|---|
| `--icon-size-xs` | 14px, dense tables and tiny status labels |
| `--icon-size-sm` | 16px, compact buttons and badges |
| `--icon-size-md` | 20px, default actions and inputs |
| `--icon-size-lg` | 24px, navigation and card headers |
| `--icon-size-xl` | 32px, empty states and compact feedback |
| `--icon-size-2xl` | 48px, feedback pages |
| `--icon-size-3xl` | 64px, illustration-like empty states |
| `--icon-color-default` | normal functional icon |
| `--icon-color-muted` | weak / disabled icon |
| `--icon-color-primary` | current or primary action icon |
| `--icon-color-success` | success status icon |
| `--icon-color-warning` | warning / reviewing status icon |
| `--icon-color-danger` | failed / blocked status icon |
| `--icon-color-info` | info / processing status icon |
| `--icon-color-inverse` | icon on dark or brand background |

## 5. Naming

Use lowercase kebab-case:

```txt
wallet.svg
withdrawal.svg
account-trading.svg
verification-video.svg
status-success.svg
status-reviewing.svg
partner-tree.svg
```

Do not include colors, sizes, versions, or vague words in icon names.

## 6. Current Icon Set

### System

| File | Purpose |
|---|---|
| `system/search.svg` | Search inputs |
| `system/filter.svg` | Filters |
| `system/copy.svg` | Copy IDs and account numbers |
| `system/more.svg` | More actions |
| `system/close.svg` | Close modals and tags |
| `system/arrow-left.svg` | Back |
| `system/chevron-down.svg` | Dropdown |
| `system/chevron-up.svg` | Collapse |
| `system/chevron-right.svg` | Continue / detail |
| `system/calendar.svg` | Date selection |
| `system/download.svg` | Download |
| `system/upload.svg` | Upload |
| `system/edit.svg` | Edit |
| `system/trash.svg` | Delete |
| `system/settings.svg` | Settings |

### Status

| File | Semantic color |
|---|---|
| `status/status-success.svg` | `--icon-color-success` |
| `status/status-failed.svg` | `--icon-color-danger` |
| `status/status-warning.svg` | `--icon-color-warning` |
| `status/status-info.svg` | `--icon-color-info` |
| `status/status-reviewing.svg` | `--icon-color-warning` |
| `status/status-processing.svg` | `--icon-color-info` |
| `status/status-blocked.svg` | `--icon-color-danger` |
| `status/status-disabled.svg` | `--icon-color-muted` |

### Finance / Broker / Verification

| File | Purpose |
|---|---|
| `finance/wallet.svg` | Wallet overview |
| `finance/deposit.svg` | Deposit |
| `finance/withdrawal.svg` | Withdrawal |
| `finance/transfer.svg` | Transfer |
| `finance/balance.svg` | Balance |
| `finance/transaction.svg` | Transaction history |
| `finance/bank-account.svg` | Bank account |
| `finance/exchange-rate.svg` | Exchange rate |
| `finance/fee.svg` | Fee |
| `finance/report.svg` | Report |
| `broker/account-trading.svg` | Real trading account |
| `broker/account-demo.svg` | Demo account |
| `broker/partner.svg` | Partner |
| `broker/partner-tree.svg` | IB tree |
| `broker/rebate.svg` | Rebate |
| `broker/client.svg` | Client |
| `verification/verification-identity.svg` | KYC |
| `verification/verification-video.svg` | Liveness |
| `verification/verification-address.svg` | Proof of address |
| `verification/document-upload.svg` | Upload document |
| `verification/document-review.svg` | Document review |
| `verification/compliance.svg` | Compliance |
| `verification/risk.svg` | Risk |
| `verification/locked.svg` | Blocked |
| `verification/reviewer.svg` | Reviewer |

## 7. Usage Rules

- Before using icons, read this file.
- Use icons from `src/assets/icons/`.
- Render icons through `src/components/ui/Icon.html` patterns and `.icon-*` classes.
- Do not inline random SVG icons directly inside pages.
- Do not use random third-party icons without documenting the source.
- Do not mix outline, filled, duotone, and 3D icons on the same page without documented reason.
- Important actions must include text labels, not icon-only buttons.
- Status icons must match the status semantic color and include status text.
- Brand icons may keep original brand colors.
- Functional icons should use `currentColor` and design tokens.

## 8. HTML Prototype Usage

```html
<span class="icon icon-md icon-primary icon--asset icon-wallet" aria-hidden="true"></span>
```

For local HTML prototypes, each icon can also be referenced as an image when original brand color is required:

```html
<span class="icon icon-sm icon-default" aria-hidden="true">
  <img src="../../assets/icons/system/filter.svg" alt="">
</span>
```

Use `aria-hidden="true"` for decorative icons paired with text. Use `aria-label` only when the icon itself conveys unique meaning.

## 9. Acceptance Checklist

| Check | Pass Standard |
|---|---|
| Naming | Kebab-case and semantically clear |
| Size | Uses icon size tokens |
| Color | Uses currentColor or tokens |
| Style | No mixed visual systems on one page |
| Stroke | Unified outline weight |
| Semantics | Icon matches the business meaning |
| Accessibility | Important icons have label or paired text |
| Componentization | Rendered through icon wrapper / component |
| Maintainability | Stored in the correct category folder |
| Business fit | Professional enough for financial / Broker UI |
