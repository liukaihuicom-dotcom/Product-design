# STATES.md

## 1. Global UI States

| State | Meaning | Required UI |
|---|---|---|
| default | Normal state | Main content + primary action |
| loading | Data or action in progress | Skeleton / spinner + disabled action |
| empty | No data | Empty explanation + next action |
| error | Failed to load or submit | Error reason + retry / support action |
| disabled | Action unavailable | Disabled control + reason |
| success | Action completed | Success message + next step |
| failed | Business process failed | Reason + resubmission / contact action |
| reviewing | Waiting for manual review | Status explanation + estimated next step |
| pending | Submitted but not completed | Timeline / progress indicator |
| blocked | User cannot continue | Clear reason + required action |

## 2. Broker / Compliance States

| Business State | Scenario | UI Treatment |
|---|---|---|
| KYC not submitted | User has not submitted identity info | Guide to start verification |
| KYC reviewing | Documents submitted, under review | Show review status and what happens next |
| KYC failed | Review rejected | Show failed reasons and resubmit action |
| KYC approved | Review passed | Show next required step if any |
| Liveness required | User triggered video verification | Explain why required and start action |
| Liveness reviewing | Video submitted | Show reviewing state and disable duplicate submission |
| Liveness failed | Video review failed | Show reason and retry action |
| Deposit pending verification | User transferred money but verification incomplete | Show fund status clearly; do not imply balance is credited |
| Withdrawal blocked | Compliance not complete | Explain requirement and guide verification |
| Account blocked | Risk control / compliance block | Show safe explanation and support path |

## 3. Required Copy Pattern

Every abnormal state should include:

1. What happened.
2. Why it happened.
3. What the user can do next.
4. Whether money/account/action is affected.

Example:

Title: Video verification required

Subtitle: Your deposit has been received but cannot be credited to your trading account until video verification is completed.

Primary Action: Start Video Verification

Secondary Action: View Deposit Details
