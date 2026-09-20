# Meeting Recordings Saturday Meeting Automation

## Overview

An n8n-based automation workflow designed to process applicant submissions from the Fillout "Meeting Recordings" form and manage the transition from the Before Meeting stage to the Saturday Orientation Meeting stage.

The workflow validates submitted meeting recording responses, updates applicant progress, sends the Saturday meeting invitation email, and maintains communication tracking throughout the process.

---

## Problem

After applicants complete the initial preparation form, they are required to provide meeting recording responses before joining the orientation session.

Manually reviewing submissions, updating applicant status, and sending meeting invitations can create delays and inconsistent communication.

This workflow automates the transition process and ensures applicants move to the correct stage after completing the required information.

---

## Workflow Purpose

The workflow manages the applicant stage before the Saturday orientation meeting:

1. Receive Meeting Recordings form submissions.
2. Identify the applicant record.
3. Validate submitted responses.
4. Update applicant lifecycle status.
5. Send Saturday meeting invitation email.
6. Record communication events.
7. Track applicant progress.

---

## Workflow Architecture


Fillout Meeting Recordings Form
|
v
Receive Submission
|
v
Extract Applicant Information
|
v
Find Applicant Record
|
v
Validate Responses
|
v
Update Applicant Status
|
v
Send Saturday Meeting Invitation
|
v
Record Communication Event


---

## Applicant Status Flow


Before Meeting
|
v
Meeting Recordings Submitted
|
v
Saturday Meeting
|
v
Orientation Session


---

## Main Features

- Fillout form processing.
- Applicant identification.
- Response validation.
- Applicant status updates.
- Automated Saturday meeting invitation.
- Gmail thread-based communication.
- Database event tracking.

---

## Data Management

The workflow uses the applicant tracking database to maintain:

- Applicant information.
- Current lifecycle stage.
- Communication history.
- Form submission events.
- Status transitions.

This allows the automation system to continue the applicant journey based on completed requirements.

---

## Technologies Used

- n8n
- Fillout Forms
- Gmail API
- MySQL Applicant Tracking Database
- JavaScript Code Nodes

---

## Security

Sensitive information has been removed from this repository.

Credentials, authentication details, private links, and internal identifiers are replaced with placeholders.

Only workflow architecture and automation logic are included.
