# Safe Test Data

Use only fictional data supplied by an authorized ATM simulator.

| Data Item | Example / Rule | Notes |
|---|---|---|
| Account | SIM-ACCOUNT-001 | Fictional identifier only |
| Valid test card | Simulator-provided card | Do not use a real bank card |
| Valid PIN | Simulator-provided PIN | Do not write real PINs in GitHub |
| Invalid PIN | Deliberately incorrect simulator PIN | Follow simulator rules |
| Starting balance | 1,000 test units | Only if configurable in simulator |
| Valid withdrawal | 100 test units | Ensure it is supported |
| Insufficient-funds withdrawal | More than current test balance | Use fictional account only |
| Daily withdrawal limit | Configured simulator limit | Confirm limit before testing |
| Unsupported denomination | An amount not supported by simulator | Simulator rules vary |

## Data Safety
- Never commit real account numbers, card numbers, PINs, or customer data.
- Do not test on real ATMs or production banking systems.
- Remove sensitive details from screenshots and logs.
