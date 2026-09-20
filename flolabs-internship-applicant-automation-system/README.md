# FloLabs Internship Applicant Automation System

## Overview

An n8n-based automation system designed to automate and manage the complete internship applicant communication journey at FloLabs.

The system handles the applicant lifecycle from the initial application submission, automated email communication, form processing, orientation attendance tracking, and masterclass follow-up.

The automation was built to reduce manual HR operations, maintain structured applicant tracking, and ensure consistent communication throughout the recruitment process.

---

## Problem

The existing CRM workflow had limitations in maintaining email threads and providing the required flexibility for applicant lifecycle tracking.

The CRM could automatically send emails after an application submission, but it could not send the first communication as a reply to the original application notification email thread.

To overcome these limitations, n8n was implemented as an automation layer using Gmail for communication handling, MySQL for applicant lifecycle management, and external form integrations.

The system operates independently from CRM limitations by maintaining applicant states, communication history, and follow-up processes through a dedicated automation infrastructure.

---

## System Architecture


Application Submission
|
v
HubSpot Form Notification Email
|
v
Gmail Processing Layer
|
v
n8n Automation Engine
|
+----------------------+
| |
v v
Email Communication MySQL Database
| |
v v
Applicant Replies Applicant Tracking
Reminders Status Management
Templates Event History


---

## Applicant Lifecycle Flow


Application Submitted
|
v
First Email + Automated Reminders
|
v
Applicant Response Processing
|
v
Websites & Presentations Form
|
v
Before Meeting Communication
|
v
Meeting Recordings Form
|
v
Orientation Session
|
v
Attendance Tracking
|
v
General Masterclass Form
|
v
Introduce Oliver Follow-up


---

# Workflows Included

## 01. Application Form First Email Automation

Processes new applicant submissions, extracts applicant information, sends the first communication email, and manages automated reminders.

---

## 02. Interested Response Automation

Handles applicants who confirm their interest and sends the next communication stage with follow-up reminders.

---

## 03. Websites & Presentations Form Automation

Processes submitted applicant forms and triggers the Before Meeting communication stage.

---

## 04. Meeting Recordings Form Automation

Handles meeting recording submissions and sends orientation meeting invitations.

---

## 05. Orientation Attendance Automation

Processes Zoom orientation attendance data and updates attendance tracking records.

---

## 06. General Masterclass Automation

Processes masterclass form submissions and triggers the next applicant communication stage.

---

# Applicant Tracking Database

A dedicated MySQL database is used as the core applicant tracking layer for managing the applicant lifecycle and supporting automation decisions.

The database maintains structured information about applicants and their interactions throughout the recruitment process.

## Data Tracked

- Applicant profile information
- Current applicant status
- Communication stages
- Email history
- Reminder stages
- Status change events
- Workflow execution history
- Applicant journey progress

The database allows n8n workflows to determine the correct next action based on the applicant's current state and previous interactions.

---

# Key Features

- Automated applicant email communication
- Email thread management
- Applicant information extraction
- Custom applicant lifecycle tracking
- Automated reminder scheduling
- Form submission processing
- Orientation attendance tracking
- Communication history management
- Recruitment pipeline automation
- Event-based applicant status updates

---

# Technologies Used

- n8n
- Gmail API
- MySQL Applicant Tracking Database
- Google Sheets
- Zoom
- Fillout Forms
- JavaScript Code Nodes

---

# Purpose

This system creates a scalable automation framework for managing internship applicants while reducing repetitive HR tasks and improving communication consistency.

By combining n8n automation workflows with a dedicated applicant tracking database, the system provides more flexibility and control over the complete recruitment lifecycle.
