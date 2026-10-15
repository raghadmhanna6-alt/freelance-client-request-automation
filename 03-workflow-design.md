# 03 — Workflow Design

## 1. Workflow Overview
The workflow uses Google Sheets and Zapier to schedule and send email reminders before project deadlines.

## 2. Workflow Steps

### Step 1: Trigger — Google Sheets
**Event:** New Spreadsheet Row

Zapier detects a new row added to the project tracker.

### Step 2: Calculate Reminder Time — Formatter by Zapier
**Event:** Date / Time — Add/Subtract Time

Formatter receives the project deadline and subtracts 24 hours to calculate the reminder time.

### Step 3: Wait — Delay by Zapier
**Event:** Delay Until

Zapier waits until the reminder time calculated by Formatter.

### Step 4: Send Email — Gmail
**Event:** Send Email

Gmail sends a reminder email to the freelancer using the email address from the spreadsheet.

## 3. Input and Output

**Input:** Freelancer name, project name, email address, and project deadline.

**Output:** An email reminder scheduled for 24 hours before the deadline.

## 4. Workflow Sequence

Google Sheets → Formatter by Zapier → Delay by Zapier → Gmail

## 5. Error Prevention
- Verify that required spreadsheet fields are completed.
- Check that the deadline uses a valid date and time format.
- Confirm that the Formatter output is connected to the Delay step.
- Verify the recipient email address.
- Test the workflow and confirm the timezone before relying on scheduled reminders.

## 6. Current Scope
This workflow handles deadline reminders for newly added spreadsheet rows. It does not yet include automated client request classification or human approval steps.
