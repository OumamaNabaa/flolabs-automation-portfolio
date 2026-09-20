# Interested Response Gmail Automation

## Overview

An n8n-based automation workflow designed to process applicant responses after the initial internship application email and manage the next stage of the applicant communication journey.

The workflow identifies applicants who respond with interest or non-interest, updates their status in the applicant tracking database, sends the appropriate communication, and maintains structured follow-up tracking.

---

## Problem

After applicants receive the first communication email, responses need to be processed according to their decision.

Manually reviewing every response and updating applicant status can create delays and inconsistent tracking.

This workflow automates response handling and connects applicant communication with the internal applicant tracking system.

---

## Workflow Purpose

The workflow handles the interested applicant stage:

1. Monitor incoming applicant email responses.
2. Identify applicant intent.
3. Process interested or non-interested responses.
4. Update applicant status.
5. Send the appropriate connected email response.
6. Record communication events.

---

## Workflow Architecture


Applicant Email Response
|
v
Gmail Trigger
|
v
Analyze Response
|
v
Identify Applicant Status
|
+----------------+
| |
v v
Interested Not Interested
| |
v v
Connected Email Status Update
|
v
Database Update
|
v
Event Tracking


---

## Applicant Tracking

The workflow updates the applicant tracking database with:

- Applicant status
- Communication stage
- Email events
- Follow-up history

This allows the automation system to determine the correct next action based on the applicant's current state.

---

## Main Features

- Applicant response detection
- Interest status processing
- Automated connected email sending
- Applicant status updates
- Communication history tracking
- Reminder workflow support

---

## Technologies Used

- n8n
- Gmail API
- MySQL Applicant Tracking Database
- JavaScript Code Nodes

---

## Workflow Role in the System

This workflow represents the second stage of the applicant journey after the initial application email.

It moves interested applicants forward while keeping communication history and applicant status synchronized.
