# FloLabs Indeed Applicant CV Automation

## Overview

An AI-powered n8n automation workflow that processes incoming applicant emails from Indeed, validates email authenticity, extracts candidate information from CV attachments, and automates HR follow-up communication.

The workflow reduces manual CV screening effort by combining Gmail monitoring, document processing, AI extraction, and automated candidate communication.

---

## Problem

FloLabs receives applicant emails from Indeed containing candidate CV attachments.

Manually reviewing every application, extracting candidate information, validating emails, and sending follow-up communication creates repetitive HR workload.

This workflow automates the initial applicant processing stage while maintaining validation checks and human review paths for uncertain cases.

---

## Workflow Architecture


Gmail Applicant Email
|
v
Email Authentication Verification
|
v
CV Attachment Detection
|
v
CV File Extraction
|
v
Document Text Parsing
|
v
AI Candidate Information Extraction
|
v
Email Validation
|
+----------------+
| |
v v
Valid Candidate Manual Review
|
v
Automated HR Follow-up Email


---

## Main Features

- Monitors company Gmail inbox for new Indeed applications.
- Verifies email authentication headers.
- Confirms emails are signed by Indeed.
- Detects CV attachments.
- Supports PDF, DOC, and DOCX files.
- Prioritizes CV-related attachments.
- Extracts candidate information using AI.
- Extracts:
  - Candidate email address.
  - Candidate first name.
- Validates candidate email before sending.
- Prevents duplicate outreach.
- Creates manual review paths when validation fails.
- Sends automated HR follow-up communication.

---

## CV Processing Logic

The workflow follows a validation-first approach:

1. Identify supported CV attachments.
2. Extract CV text.
3. Detect candidate information.
4. Validate extracted email.
5. Check duplicate contact history.
6. Send follow-up email only when confidence requirements are met.

The workflow avoids guessing candidate information when confidence is low.

---

## Technologies Used

- n8n
- Gmail API
- OpenAI API
- Document Processing
- JavaScript
- Workflow Automation

---

## Challenges Solved

- Processing unstructured CV documents.
- Extracting reliable candidate information.
- Validating applicant identity data.
- Reducing manual HR screening workload.
- Creating automated but controlled communication flows.
- Handling failed cases through human review.

---

## Security

Sensitive information has been removed from this repository.

Credentials, authentication details, internal emails, and private identifiers are replaced with placeholders.

Only workflow architecture and automation logic are included.
