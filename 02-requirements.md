# 02 — Requirements

## 1. Project Overview
The Freelance Client Request Automation project aims to help freelancers organize project information and receive email reminders before project deadlines.

## 2. Functional Requirements
- The user can store project details in Google Sheets.
- The spreadsheet records the freelancer name, project name, email address, and deadline.
- Zapier detects new rows added to the spreadsheet.
- Formatter by Zapier calculates a reminder time 24 hours before the deadline.
- Delay by Zapier waits until the calculated reminder time.
- Gmail sends an email reminder to the freelancer.

## 3. Input Data
The workflow uses the following fields:
- Freelancer Name
- Project Name
- Freelancer Email
- Deadline

## 4. Output
The expected output is an email reminder sent to the freelancer 24 hours before the project deadline.

## 5. Non-Functional Requirements
- The workflow should be simple to understand and maintain.
- Project information should be organized clearly.
- The reminder should be sent at the intended time.
- Email addresses and deadlines should be entered correctly.

## 6. Tools and Technologies
- Google Sheets
- Zapier
- Formatter by Zapier
- Delay by Zapier
- Gmail

## 7. Assumptions
- The user has access to Google Sheets, Zapier, and Gmail.
- Each project has a valid email address and deadline.
- The Zap is turned on and the connected accounts are working.

## 8. Constraints
- The current workflow is triggered by new spreadsheet rows.
- Existing rows may need to be added again or otherwise processed to trigger the workflow.
- Timezone settings must be checked to ensure reminders are sent at the correct local time.
- The workflow currently focuses on deadline reminders rather than full client request processing.
