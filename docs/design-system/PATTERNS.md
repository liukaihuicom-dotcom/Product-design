# PATTERNS.md

## 1. Dashboard Page Pattern

Use for:

- Partner dashboard
- Broker admin dashboard
- User home page
- Wallet overview

Structure:

1. Page header.
2. Key metrics.
3. Important alert / risk notice.
4. Primary operation cards.
5. Recent records.
6. Secondary modules.

Rules:

- Metrics should be easy to compare.
- Do not overload the first screen.
- Risk or action-required messages must appear above secondary content.

## 2. Detail Page Pattern

Use for:

- Trading account detail
- Deposit detail
- Withdrawal detail
- KYC user detail
- Partner detail

Structure:

1. Page header with status.
2. Key summary card.
3. Detail sections.
4. Timeline / history.
5. Action area.
6. Risk / compliance notes.

Rules:

- Status must be visible at the top.
- Primary action must match the current status.
- History should be chronological.

## 3. Form Page Pattern

Use for:

- KYC form
- Deposit form
- Withdrawal form
- Address proof upload
- Bank account binding

Structure:

1. Step / progress indicator.
2. Form title and subtitle.
3. Input groups.
4. Upload / proof area if needed.
5. Risk / requirement explanation.
6. Sticky bottom action on mobile.

Rules:

- Required fields must be clear.
- Compliance reason should be explained in friendly language.
- Mobile forms should avoid too many fields on one screen.

## 4. Review Queue Pattern

Use for:

- KYC review
- Liveness review
- Deposit review
- Withdrawal review
- POA review

Structure:

1. Queue summary.
2. Filters.
3. Table / list.
4. Risk badge.
5. SLA / priority.
6. Batch or row actions.

Rules:

- Reviewer must quickly identify priority.
- Status and risk must be visually scannable.
- Avoid splitting review queues only by document type unless business requires it.

## 5. Wallet / Funds Pattern

Use for:

- Wallet overview
- Deposit
- Withdrawal
- Transfer
- Transaction record

Structure:

1. Balance summary.
2. Main action area.
3. Account / currency selector.
4. Transaction form.
5. Compliance notice.
6. Transaction history.

Rules:

- Amount input must be prominent.
- Currency must never be ambiguous.
- Pending compliance requirements must be shown before final submit.
- If fund movement is blocked, explain the exact reason and next step.
