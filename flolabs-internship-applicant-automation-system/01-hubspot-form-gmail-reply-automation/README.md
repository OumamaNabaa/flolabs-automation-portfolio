# HubSpot Form Gmail Reply Automation

## Overview

An n8n-based automation workflow designed to process new internship application notifications received from HubSpot Forms and automate the first communication stage with applicants.

The workflow uses Gmail as the communication layer and n8n as the automation engine to receive application notifications, extract applicant information, send the first email reply, and manage automated follow-up reminders.

---

## Problem

The existing CRM workflow could trigger automatic emails after an applicant submitted an application form, but it could not send the first email as a reply within the original email conversation thread.

This workflow solves this limitation by using Gmail and n8n to process incoming application notifications and maintain structured communication with applicants.

---

## Workflow Purpose

The workflow is responsible for the first stage of the applicant lifecycle:

1. Receiving application notification emails.
2. Validating that the email is from the internship application form.
3. Extracting applicant information.
4. Sending the first email communication.
5. Saving applicant information into the applicant tracking database.
6. Managing reminder communication when applicants do not respond.

---

## Workflow Architecture


HubSpot Application Form
|
v
Gmail Notification Email
|
v
n8n Gmail Trigger
|
v
Validate Application Email
|
v
Extract Applicant Information
|
v
Send First Email Reply
|
v
Store Applicant Data
|
v
Schedule Reminder Follow-ups


---

## Main Components

### Gmail Integration

The workflow receives application notification emails through Gmail and sends applicant communication emails while preserving the email conversation thread.

---

### Applicant Data Processing

The workflow extracts important applicant information including:

- First Name
- Last Name
- Email Address
- Phone Number
- Country
- Location
- LinkedIn Profile
- Education Information
- CV Information

---

### Applicant Tracking Database

Applicant information and communication events are stored in the MySQL applicant tracking database.

The database is used to maintain:

- Applicant profile information
- Current applicant status
- Email communication history
- Reminder stages
- Status change events

---

## Reminder System

The workflow includes automated follow-up stages for applicants who do not respond.

The reminder system tracks applicant progress and sends the appropriate communication based on the current applicant state.

---

## Technologies Used

- n8n
- Gmail
- MySQL
- HubSpot Forms
- JavaScript Code Nodes

---

## Workflow Role in the System

This workflow represents the entry point of the FloLabs Internship Applicant Automation System.

It starts the applicant journey and prepares applicant data for the following automation stages.
