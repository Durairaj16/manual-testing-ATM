# ATM Simulator Manual Test Plan

## 1. Purpose
Define the approach for testing common ATM functions in a dedicated simulator or authorized training environment.

## 2. Objectives
- Verify expected behaviour for valid and invalid inputs.
- Check transaction rules such as available balance and withdrawal limits.
- Confirm clear feedback when a transaction cannot proceed.
- Check that unsuccessful withdrawals do not incorrectly change the balance.
- Document results and reproducible defects.

## 3. Scope
### In scope
- Card acceptance/rejection
- PIN validation
- Balance enquiry
- Cash withdrawal
- Insufficient funds and transaction limits
- Supported denominations
- Mini statement
- Receipt generation
- Session timeout and termination

### Out of scope
- Real bank networks or real payment transactions
- Physical ATM hardware security testing
- Penetration testing
- Testing against production banking systems

## 4. Test Approach
Use manual black-box testing. Follow the steps in each test case, compare the observed result with the expected result, and record evidence where possible. Use positive, negative, and boundary-value tests.

## 5. Test Environment
- A dedicated ATM simulator or authorized training system
- Fictional test accounts and balances
- Browser or device supported by the simulator
- Test evidence stored without sensitive information

Features differ by simulator. Mark unsupported cases **Blocked** or **Not Applicable**, and explain why.

## 6. Entry Criteria
- Simulator is accessible.
- Fictional test data is available.
- Test scope and supported functions are understood.

## 7. Exit Criteria
- All applicable cases have an execution status.
- Failures have reproducible steps and evidence where possible.
- Summary metrics are updated.
- Known limitations are documented.

## 8. Severity Guidance
- **Critical:** major transaction integrity issue or broad service outage.
- **High:** important function fails with significant impact.
- **Medium:** function is impaired but a workaround may exist.
- **Low:** minor display or usability issue.

Assign severity based on observed impact, not the sample report.

## 9. Deliverables
- Test plan
- Test cases
- Test execution report
- Defect reports
- Test summary

## 10. Risks and Assumptions
- The project is documentation for simulator-based practice.
- Some test scenarios may not be supported by the selected simulator.
- No defect is confirmed until it is reproduced.
- Never use real banking credentials or real ATMs for practice.
