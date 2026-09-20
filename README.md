# FloLabs Automation Portfolio

A collection of AI-powered automation systems developed for FloLabs using workflow automation, API integrations, artificial intelligence, and database-driven solutions.

This repository showcases practical automation solutions designed to reduce repetitive operational tasks, improve internal processes, and create scalable workflows across different business functions.

---

# Overview

Modern organizations rely on multiple tools and platforms to manage communication, data, and operations.

The automation systems in this repository focus on connecting these systems together through reliable workflows that combine:

- Event-driven automation
- API integrations
- AI-powered data processing
- Database management
- Automated communication
- Error monitoring and reliability improvements

The goal is to transform manual operational processes into structured, scalable, and maintainable automation systems.

---

# Projects

## FloLabs Indeed Applicant CV Automation

An AI-powered recruitment automation workflow that processes incoming applicant emails from Indeed, validates email authenticity, extracts candidate information from CV documents, and automates HR follow-up communication.

### Key Capabilities

- Monitors applicant emails.
- Validates email authentication.
- Detects and processes CV attachments.
- Extracts candidate information using AI.
- Validates candidate email addresses.
- Prevents duplicate communication.
- Routes uncertain cases for manual review.
- Sends automated HR follow-up emails.

### Technologies

- n8n
- Gmail Integration
- OpenAI API
- JavaScript
- Workflow Automation

---

## FloLabs Internship Applicant Automation System

An end-to-end applicant lifecycle automation system designed to manage internship candidates from initial application submission through orientation, evaluation, and onboarding stages.

### Key Capabilities

- Application processing automation.
- Applicant communication workflows.
- Automated reminder sequences.
- Candidate status tracking.
- Form submission processing.
- Orientation attendance tracking.
- Masterclass follow-up automation.
- Database-driven applicant management.

### Technologies

- n8n
- Gmail API
- Fillout Forms
- Zoom API
- Google Sheets API
- MySQL Database
- OpenAI API

---

## FloLabs n8n Error Monitoring System

An automated monitoring workflow designed to improve automation reliability by detecting workflow failures, collecting error details, and providing structured failure notifications.

### Key Capabilities

- Captures failed workflow executions.
- Collects failed node information.
- Stores error details.
- Sends automated alerts.
- Improves troubleshooting and recovery speed.

### Technologies

- n8n
- Discord Webhooks
- Notion Database
- Workflow Automation

---

# Repository Structure


flolabs-automation-portfolio

├── flolabs-indeed-applicant-cv-automation
│ ├── README.md
│ ├── workflow-overview.png
│ └── workflow.json
│
├── flolabs-internship-applicant-automation-system
│ ├── README.md
│ ├── 01-hubspot-form-gmail-reply-automation
│ ├── 02-interested-response-gmail-automation
│ ├── 03-fillout-before-meeting-email-automation
│ ├── 04-meeting-recordings-saturday-meeting-automation
│ ├── 05-zoom-orientation-attendance-google-sheets
│ └── 06-general-masterclass-introduce-oliver-automation
│
└── flolabs-n8n-error-monitoring-system
├── README.md
└── workflow.json


---

# Technologies Used

| Technology | Purpose |
|---|---|
| n8n | Workflow automation engine |
| OpenAI API | AI-powered extraction and processing |
| Gmail API | Automated email communication |
| Fillout | Form processing |
| Zoom API | Meeting automation |
| Google Sheets API | Data tracking |
| MySQL | Applicant data management |
| JavaScript | Custom workflow logic |

---

# Security & Privacy

All workflows included in this repository have been sanitized before publication.

Sensitive information has been removed, including:

- API credentials
- Authentication tokens
- Private email addresses
- Internal identifiers
- Private documents and links

Only workflow architecture, automation logic, and technical implementation patterns are included.

---

# Documentation

Each project contains its own documentation covering:

- Workflow purpose
- Architecture overview
- Main features
- Technologies used
- Challenges solved
- Security considerations

---

# About FloLabs Automation Systems

This repository represents automation solutions built to connect business processes, improve operational efficiency, and enable scalable workflows through modern automation technologies.
