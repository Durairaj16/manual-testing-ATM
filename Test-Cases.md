# ATM Simulator Test Cases

**Application:** ATM simulator / authorized training environment  
**Test status at project creation:** Not Run

| ID | Scenario | Preconditions / Test Data | Steps | Expected Result | Priority |
|---|---|---|---|---|---|
| ATM-001 | Open simulator | Simulator URL/app available | Launch simulator | Start screen appears | High |
| ATM-002 | Accept valid test card | Supported fictional card | Insert/select test card | Card is accepted | High |
| ATM-003 | Reject unsupported card | Unsupported test card, if simulator supports it | Insert/select unsupported card | Clear rejection message appears | Medium |
| ATM-004 | Authenticate with valid PIN | Valid fictional card and PIN | Enter valid PIN | Main menu opens | High |
| ATM-005 | Reject incorrect PIN | Valid card, incorrect fictional PIN | Enter incorrect PIN | Access is denied with a suitable message | High |
| ATM-006 | Handle blank PIN | Simulator allows submitting blank input | Leave PIN blank and submit | Validation appears; access is denied | Medium |
| ATM-007 | Handle PIN length boundary | Use shorter/longer PIN input if supported | Enter PIN with invalid length | Input is rejected or validation appears | Medium |
| ATM-008 | View balance | Authenticated fictional account | Select Balance Enquiry | Correct test balance is shown | High |
| ATM-009 | Withdraw valid amount | Balance sufficient; amount allowed | Select withdrawal and enter amount | Transaction succeeds and balance is updated correctly | High |
| ATM-010 | Withdraw zero amount | Simulator accepts amount entry | Enter 0 | Transaction is rejected with validation | Medium |
| ATM-011 | Withdraw negative amount | Simulator accepts signed input | Enter a negative amount | Transaction is rejected | High |
| ATM-012 | Withdraw above available balance | Request exceeds fictional account balance | Submit withdrawal | Transaction is rejected; balance remains unchanged | High |
| ATM-013 | Withdraw at daily limit | Test data supports limit boundary | Request amount exactly at configured limit | Result follows configured policy | Medium |
| ATM-014 | Withdraw above daily limit | Request exceeds configured limit | Submit withdrawal | Transaction is rejected with suitable message | High |
| ATM-015 | Unsupported denomination | Enter amount not supported by simulator | Submit withdrawal | Validation or rejection appears | Medium |
| ATM-016 | Empty withdrawal amount | Leave amount blank | Submit withdrawal | Required-field validation appears | Medium |
| ATM-017 | Balance after withdrawal | Successful withdrawal completed | Check balance again | Balance reflects the withdrawal accurately | High |
| ATM-018 | Failed withdrawal does not debit | Insufficient-funds scenario | Attempt withdrawal, then check balance | Balance remains unchanged | High |
| ATM-019 | View mini statement | Authenticated account with test transactions | Select Mini Statement | Recent test transactions are displayed accurately | Medium |
| ATM-020 | Request receipt | Receipt feature supported | Complete a test transaction and request receipt | Receipt is generated or a clear message appears | Low |
| ATM-021 | Decline receipt | Receipt choice is available | Choose no receipt | Transaction completes without a receipt | Low |
| ATM-022 | Cancel transaction | Transaction screen is open | Select Cancel | Transaction is cancelled and user returns safely | Medium |
| ATM-023 | Session timeout | Simulator supports timeout | Leave session idle for configured duration | Session expires and protected functions require authentication | High |
| ATM-024 | End session | Authenticated session active | Select Exit/Finish | Session terminates and card is ejected/virtual card returned if supported | High |
| ATM-025 | Access protected menu after logout | Session has ended | Attempt to return to account menu | Protected account details are not accessible without authentication | High |

## Execution Instructions
1. Run each applicable case in the simulator.
2. Record the actual result and status in `Test-Execution-Report.csv`.
3. Use **Pass** only when actual behaviour matches the expected result.
4. Use **Fail** only when a reproducible mismatch occurs.
5. Use **Blocked** when the environment prevents execution.
6. Use **Not Applicable** only when the feature is not supported, with a reason.

Do not mark cases as passed based only on the expected result written here.
