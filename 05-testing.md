# 05 — Testing

## 1. Testing Objective
The purpose of testing is to verify that the workflow calculates reminder times, waits until the scheduled time, and sends email reminders.

## 2. Test Cases

| Test | Expected Result | Status |
|---|---|---|
| Google Sheets trigger setup | Detect a new spreadsheet row | Configured; full live trigger needs verification |
| Formatter test | Calculate a time 24 hours before the deadline | Test successful |
| Delay test | Accept the calculated reminder time | Test successful |
| Gmail test | Send a reminder email to the configured recipient | Test email received |
| End-to-end scheduled reminder | Send the reminder at the correct time | Pending verification |
| Timezone verification | Send the reminder at the intended local time | Pending verification |

## 3. Email Test
A Gmail test email was sent to the configured recipient. The test confirmed that the email action can send a message.

## 4. Known Limitations
- A successful Gmail test does not prove that the full scheduled workflow has completed.
- The live trigger must be verified using a newly added spreadsheet row.
- The timezone must be checked because the Delay test output was displayed in UTC.
- The actual scheduled reminder has not yet been confirmed.

## 5. Conclusion
The main Zap steps have been configured and tested individually. Full end-to-end verification remains necessary to confirm that a reminder is sent at the intended local time.
