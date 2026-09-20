# Zoom Orientation Attendance to Google Sheets Automation

## Overview

An n8n-based automation workflow designed to process Zoom Orientation Meeting attendance data, classify attendee participation, update attendance records, and maintain orientation tracking information in Google Sheets.

The workflow automatically analyzes meeting participants, determines attendance type, sends the appropriate follow-up communication, and records attendance information for future applicant tracking.

---

## Problem

After each orientation session, the team needs to review Zoom attendance, determine how long each applicant stayed, categorize their participation, send the correct follow-up email, and update tracking sheets.

Manually completing these steps after every session is time-consuming and can lead to inconsistent tracking.

This workflow automates attendance processing and standardizes post-orientation communication.

---

## Workflow Purpose

The workflow handles the post-orientation attendance process:

1. Receive Zoom meeting completion events.
2. Validate the meeting type.
3. Retrieve participant attendance data.
4. Normalize participant records.
5. Calculate attendance duration.
6. Compare attendance against session duration.
7. Classify attendance cases.
8. Update Google Sheets tracking.
9. Send the appropriate follow-up email.

---

## Workflow Architecture


Zoom Meeting Ended
|
v
Webhook Trigger
|
v
Validate Meeting Event
|
v
Retrieve Participants
|
v
Normalize Attendance Data
|
v
Classify Attendance Case
|
+-------------------+
| |
v v
Full Attendance Partial Attendance
| |
v v
Masterclass Email Recording + Q&A Email

    |
    v

Brief Attendance
|
v
Follow-up Email

    |
    v

Google Sheets Update


---

## Attendance Classification

The workflow categorizes participants into three groups:

### Full Session

Participants who attended the complete orientation session.

Action:
- Send orientation follow-up with Masterclass information.
- Record attendance in Google Sheets.

---

### Missed Q&A / Partial Attendance

Participants who attended most of the session but missed part of the meeting.

Action:
- Send the orientation recording link.
- Provide next steps.
- Record attendance details.

---

### Briefly Attended

Participants who attended for a short duration.

Action:
- Send a follow-up message.
- Offer additional support or another opportunity to attend.
- Record attendance details.

---

## Main Features

- Zoom webhook integration.
- Automatic participant retrieval.
- Attendance duration calculation.
- Attendance classification.
- Automated follow-up emails.
- Google Sheets attendance tracking.
- Duplicate participant handling.
- Communication history tracking.

---

## Technologies Used

- n8n
- Zoom API
- Gmail API
- Google Sheets API
- JavaScript Code Nodes

---

## Data Management

The workflow tracks:

- Applicant name.
- Attendance duration.
- Attendance category.
- Comments.
- Follow-up status.
- Communication history.

This allows the applicant journey to remain synchronized after orientation sessions.

---

## Security

Sensitive information has been removed from this repository.

Credentials, authentication details, private links, account identifiers, and internal email addresses have been replaced with placeholders.

Only workflow architecture and automation logic are included.
