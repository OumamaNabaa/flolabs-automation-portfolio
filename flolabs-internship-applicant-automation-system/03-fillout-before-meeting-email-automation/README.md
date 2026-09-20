# Fillout Before Meeting Email Automation

## Overview

An n8n-based automation workflow that processes applicant submissions from the Fillout "Websites & Presentations" form and manages the communication stage before the orientation meeting.

The workflow automatically detects completed forms, updates applicant records, sends the appropriate follow-up emails, and manages reminder sequences until the applicant progresses to the next stage.

---

## Problem

After an applicant confirms interest and receives the required preparation form, the team needs to monitor whether they complete the required information before the orientation meeting.

Manually checking submissions, sending reminders, and updating applicant statuses creates unnecessary operational overhead.

This workflow automates the entire "Before Meeting" communication stage while keeping applicant information synchronized with the tracking database.

---

## Workflow Purpose

The workflow handles applicants in the **Before Meeting** stage:

1. Receive Fillout form submissions.
2. Parse applicant responses.
3. Identify the applicant record.
4. Update applicant status in the database.
5. Send the Before Meeting confirmation email.
6. Monitor incomplete responses.
7. Send automated reminders when required.
8. Track all status changes and communication events.

---

## Workflow Architecture


Fillout Form Submission
|
v
Gmail Trigger
|
v
Detect Websites & Presentations Form
|
v
Parse Applicant Responses
|
v
Find Applicant in Database
|
v
Update Applicant Status
|
v
Send Before Meeting Email
|
v
Reminder Sequence
|
+----------------+
| |
v v
Reminder 1 Reminder 2
| |
+----------------+
|
v
Final Reminder
|
v
No Answer


---

## Main Features

- Fillout form submission processing.
- Applicant information extraction.
- Database status management.
- Thread-based Gmail replies.
- Automated reminder sequence.
- Applicant event tracking.
- Duplicate communication prevention.
- Structured applicant journey management.

---

## Applicant Status Flow


Before Meeting
|
v
Reminder Before Meeting 1
|
v
Reminder Before Meeting 2
|
v
No Answer


Each status transition is recorded to maintain a complete applicant communication history.

---

## Data Management

The workflow uses the applicant database to store and manage:

- Applicant information.
- Current status.
- Status update timestamps.
- Email thread information.
- Communication events.

This allows the automation system to determine the correct next action based on the applicant's current stage.

---

## Technologies Used

- n8n
- Gmail API
- Fillout Forms
- MySQL Database
- OpenAI API
- JavaScript Code Nodes

---

## Automation Schedule

The workflow contains scheduled checks to identify applicants who require follow-up based on their current status and the elapsed time since the previous communication.

---

## Security

Sensitive information has been removed from this repository.

Credentials, authentication tokens, private emails, and internal identifiers are replaced with placeholders.

Only the workflow architecture and automation logic are included.
