# 12-API_STATE_MAP.md

## API State Map Goal

UI state must be driven by backend status fields, not arbitrary visual assumptions.

## KYC State Mapping

| API Field | Value | UI State | UI Treatment |
|---|---|---|---|
| `kyc_status` | `not_started` | Not started | Guide user to start |
| `kyc_status` | `submitted` | Submitted | Show pending review |
| `kyc_status` | `reviewing` | Reviewing | Show reviewing status |
| `kyc_status` | `approved` | Approved | Show success and next step |
| `kyc_status` | `rejected` | Failed | Show reasons and resubmit |
| `kyc_status` | `expired` | Expired | Ask user to update documents |

## Liveness State Mapping

| API Field | Value | UI State | UI Treatment |
|---|---|---|---|
| `liveness_required` | `true` | Required | Show verification CTA |
| `liveness_status` | `not_started` | Not started | Start video verification |
| `liveness_status` | `submitted` | Submitted | Show submitted state |
| `liveness_status` | `reviewing` | Reviewing | Disable duplicate submit |
| `liveness_status` | `approved` | Approved | Unlock related action |
| `liveness_status` | `rejected` | Failed | Show reason and retry |

## Deposit State Mapping

| API Field | Value | UI State | UI Treatment |
|---|---|---|---|
| `deposit_status` | `draft` | Draft | User can continue |
| `deposit_status` | `submitted` | Submitted | Show processing |
| `deposit_status` | `processing` | Processing | Show timeline |
| `deposit_status` | `pending_verification` | Pending verification | Show verification required |
| `deposit_status` | `successful` | Successful | Show credited amount |
| `deposit_status` | `failed` | Failed | Show failed reason |
| `deposit_status` | `cancelled` | Cancelled | Show cancelled status |

## Withdrawal State Mapping

| API Field | Value | UI State | UI Treatment |
|---|---|---|---|
| `withdraw_status` | `draft` | Draft | User can edit |
| `withdraw_status` | `submitted` | Submitted | Show pending review |
| `withdraw_status` | `reviewing` | Reviewing | Show review timeline |
| `withdraw_status` | `blocked` | Blocked | Show compliance reason |
| `withdraw_status` | `approved` | Approved | Show processing payout |
| `withdraw_status` | `successful` | Successful | Show completed |
| `withdraw_status` | `rejected` | Failed | Show reason and next action |

## Account State Mapping

| API Field | Value | UI State | UI Treatment |
|---|---|---|---|
| `account_status` | `active` | Active | Normal operations |
| `account_status` | `pending_demo` | Demo required | Guide demo trade |
| `account_status` | `pending_review` | Pending review | Show review status |
| `account_status` | `restricted` | Restricted | Explain limitations |
| `account_status` | `suspended` | Suspended | Show support path |
| `account_status` | `archived` | Archived | Read-only state |
