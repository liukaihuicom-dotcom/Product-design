# 09-STATES.md

This file extends `STATES.md` for Design System v2.0.

## Required UI States

- default
- loading
- empty
- error
- disabled
- success
- failed
- reviewing
- pending
- blocked
- no_permission
- partial_loading

## Abnormal State Copy

Every blocked or failed state must include:

1. What happened.
2. Why it happened.
3. What the user can do next.
4. Whether funds, account, or access are affected.

## API Alignment

UI states must map to `12-API_STATE_MAP.md`. Do not invent visual states that conflict with backend status fields.
