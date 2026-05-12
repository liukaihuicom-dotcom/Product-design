# PAGE_BRIEF.md

## Page Name

Deposit Page

## Platforms

- web-portal
- app-ios
- app-android
- h5-mobile

## User Role

Trader

## Business Goal

User selects trading account, enters deposit amount, selects payment method, and submits deposit request.

## Key User Tasks

1. Select trading account.
2. Enter deposit amount.
3. Select payment method.
4. Review fee and processing time.
5. Submit deposit request.
6. View deposit status.

## Required Data

- trading_account_id
- account_type
- account_currency
- available_balance
- deposit_amount
- payment_method
- fee
- processing_time
- verification_status
- deposit_status

## API State Fields

- kyc_status
- liveness_required
- liveness_status
- deposit_status
- account_status

## Required UI States

- default
- loading
- empty account
- amount error
- payment method unavailable
- compliance verification required
- submitting
- successful
- failed
- pending verification

## Web Requirements

- Use form card + side compliance helper.
- Show deposit records link.
- Use desktop-friendly account selector.

## App Requirements

- Amount input should be visually prominent.
- Use bottom sheet for account and payment method selection.
- Use sticky bottom submit button.
- Use card list for recent deposit records.

## Primary CTA

Submit Deposit

## Secondary CTA

View Deposit Records
