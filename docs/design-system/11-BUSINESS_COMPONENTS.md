# 11-BUSINESS_COMPONENTS.md

## Business Components Goal

Broker products require reusable business components beyond basic UI components.

## Component Priority

| Priority | Component | Scenario |
|---|---|---|
| P0 | AccountCard | Trading account display |
| P0 | AmountInput | Deposit / withdrawal / transfer |
| P0 | CurrencySelector | Multi-currency account |
| P0 | VerificationStatus | KYC / liveness / POA |
| P0 | RiskNotice | Compliance warning |
| P0 | StatusTimeline | Review and transaction history |
| P0 | TransactionItem | App transaction list |
| P1 | WalletSummary | Wallet overview |
| P1 | PaymentMethodCard | Deposit / withdrawal |
| P1 | PartnerSummaryCard | Partner portal |
| P1 | RebateMetricCard | IB rebate reports |
| P1 | ReviewDecisionPanel | Admin review center |
| P2 | PartnerTreeView | IB hierarchy |
| P2 | AccountGroupBadge | Account type / currency group |
| P2 | ComplianceChecklist | KYC completion status |

## AccountCard Required Data

| Field | Required |
|---|---:|
| Account number | Yes |
| Account type | Yes |
| Platform MT4/MT5 | Yes |
| Currency | Yes |
| Balance | Yes |
| Status | Yes |
| Primary action | Conditional |
| Copy action | Yes |

## AmountInput Rules

- Amount input must be visually prominent.
- Currency cannot be ambiguous.
- Error must explain the exact problem.
- Use large numeric typography for key amount input on App.

## RiskNotice Rules

- Use for compliance, risk, and blocked fund movement.
- Must include reason and next action.
- Do not hide important risk inside tooltip only.
- On App, place near the affected action.
