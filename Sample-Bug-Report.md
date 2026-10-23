# Sample Defect Report — Hypothetical

> This is a training example only. It is not a confirmed defect in any real ATM or simulator.

- **Defect ID:** ATM-BUG-SAMPLE-001
- **Title:** Withdrawal is accepted even when requested amount exceeds available balance
- **Module:** Cash Withdrawal
- **Severity:** High (proposed)
- **Priority:** High (proposed)
- **Status:** Not Verified

## Preconditions
A fictional test account exists with a known balance in an authorized simulator.

## Steps to Reproduce
1. Sign in using the simulator's fictional test account.
2. Note the available balance.
3. Request a withdrawal greater than that balance.
4. Observe the result and check the balance again.

## Expected Result
The transaction should be rejected and the balance should remain unchanged.

## Actual Result
Not observed yet. Fill this section only after execution.

## Evidence
Attach a simulator screenshot or log only if the issue is reproduced. Remove any sensitive data.

## Conclusion
Do not classify this scenario as an actual defect unless the behaviour is reproduced in the test environment.
