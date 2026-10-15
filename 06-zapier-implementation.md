# 06 — Zapier Implementation

## 1. Implementation Overview
The workflow was created in Zapier to schedule project deadline reminders using Google Sheets and Gmail.

## 2. Connected Applications
- Google Sheets
- Formatter by Zapier
- Delay by Zapier
- Gmail

## 3. Zap Configuration

### Step 1: Google Sheets
- Trigger event: New Spreadsheet Row
- Spreadsheet: Freelance Project Tracker
- Worksheet: الورقة1

The spreadsheet includes Freelancer Name, Project Name, Freelancer Email, and Deadline.

### Step 2: Formatter by Zapier
- Action: Date / Time — Add/Subtract Time
- Input: Deadline
- Expression: -24 hours
- Purpose: Calculate the reminder time.

### Step 3: Delay by Zapier
- Action: Delay Until
- Input: Output from Formatter by Zapier
- Purpose: Wait until the calculated reminder time.

### Step 4: Gmail
- Action: Send Email
- Recipient: Freelancer Email from Google Sheets
- Subject: Reminder: Project Deadline
- Purpose: Send an email reminder before the deadline.

## 4. Testing Results
The Formatter test succeeded, the Delay test succeeded, and the Gmail test email was received.

## 5. Publication Status
The Zap was published, and Zapier confirmed that the new version was on.

## 6. Remaining Verification
- Confirm that a newly added row triggers the live workflow.
- Confirm the local timezone and scheduled release time.
- Verify that the complete workflow sends the reminder at the intended time.

## 7. Current Limitation
The current implementation handles project deadline reminders. It does not yet implement the complete client request intake, AI classification, and human review process.
