# Freelance Client Request Automation

## Project Overview
This project demonstrates a basic automation workflow that helps freelancers track project deadlines and receive email reminders.

## Problem
Freelancers may manage several projects at once and can forget important deadlines when tracking them manually.

## Solution
The workflow stores project information in Google Sheets, calculates a reminder time 24 hours before the deadline, waits until that time, and sends an email through Gmail.

## Tools Used
- Google Sheets
- Zapier
- Formatter by Zapier
- Delay by Zapier
- Gmail

## Workflow
1. A new project row is added to Google Sheets.
2. Formatter calculates the reminder time by subtracting 24 hours from the deadline.
3. Delay waits until the calculated time.
4. Gmail sends an email reminder to the freelancer.

## Spreadsheet Fields
- Freelancer Name
- Project Name
- Freelancer Email
- Deadline

## Testing
The Formatter and Delay steps were tested successfully. A Gmail test email was also received. The complete scheduled workflow still requires end-to-end verification, including timezone accuracy.

## AI Enhancement
AI-based client request classification and human review are proposed future improvements. They are not implemented in the current workflow.

## Documentation
- [Business Analysis](01-business-analysis.md)
- [Requirements](02-requirements.md)
- [Workflow Design](03-workflow-design.md)
- [AI Design](04-ai-design.md)
- [Testing](05-testing.md)
- [Zapier Implementation](06-zapier-implementation.md)

## Current Status
The basic deadline reminder workflow has been configured and published. Final verification of a live scheduled reminder is pending.
