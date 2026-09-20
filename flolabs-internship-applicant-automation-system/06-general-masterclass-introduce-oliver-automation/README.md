# General Masterclass Introduce Oliver Automation

## Overview

An n8n-based automation workflow designed to process General Masterclass form submissions and manage the transition of applicants to the next communication stage.

The workflow detects completed masterclass submissions, validates applicant information, updates applicant tracking records, and sends the appropriate introduction email to continue the applicant journey.

---

## Problem

After applicants attend the orientation session, they are required to complete the General Masterclass form before moving to the next stage.

Manually reviewing submissions, checking applicant responses, updating statuses, and introducing applicants to the next team member creates additional operational work.

This workflow automates the process and ensures applicants are moved forward consistently after completing the required form.

---

## Workflow Purpose

The workflow manages the post-orientation masterclass stage:

1. Receive General Masterclass form submissions.
2. Extract applicant information.
3. Identify the applicant record.
4. Validate submitted responses.
5. Update applicant status.
6. Send the introduction email.
7. Record communication events.

---

## Workflow Architecture


General Masterclass Form
|
v
Receive Submission
|
v
Extract Applicant Data
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
Send Introduction Email
|
v
Track Communication Event


---

## Applicant Status Flow


Attended
|
v
Masterclass Completed
|
v
Second Meeting


---

## Main Features

- General Masterclass form processing.
- Applicant identification.
- Response validation.
- Applicant status updates.
- Automated introduction emails.
- Communication history tracking.
- Database synchronization.

---

## Data Management

The workflow uses the applicant tracking database to maintain:

- Applicant profile information.
- Current lifecycle stage.
- Form submission events.
- Communication history.
- Status transitions.

This allows the automation system to determine the correct next action based on applicant progress.

---

## Technologies Used

- n8n
- Fillout Forms
- Gmail API
- MySQL Applicant Tracking Database
- JavaScript Code Nodes

---

## Workflow Role in the System

This workflow represents the final automation stage in the internship applicant communication pipeline.

It completes the transition from orientation participation to the next applicant interaction stage.
