# ATS Job Tracker

An automated Applicant Tracking System (ATS) job tracker built using **n8n** to streamline internship and job searching. The workflow detects the ATS used by a company's careers page, extracts current job openings, matches them against user-defined preferred roles, and updates a Google Sheet automatically.

---

## Overview

Searching hundreds of company career pages manually is repetitive and time-consuming. This project automates that process by integrating Google Sheets, n8n workflows, and ATS-specific APIs.

The system currently supports:

- Workday-based career portals
- Role-based job filtering
- Automatic Google Sheets updates
- Modular workflow design for adding new ATS platforms

---

## Project Architecture

```
ATS Job Tracker
│
├── Phase 1
│   ├── Reads company details from Google Sheets
│   ├── Detects ATS platform
│   └── Routes execution to the correct workflow
│
├── Workday Module
│   ├── Calls Workday APIs
│   ├── Extracts job information
│   └── Returns structured job data
│
└── Phase 2
    ├── Matches jobs with preferred roles
    ├── Aggregates matching openings
    ├── Updates Google Sheets
    └── Stores job availability
```

---

## Features

- Automated ATS detection
- Workday integration
- API-based job extraction (no HTML scraping for supported portals)
- Preferred role matching
- Google Sheets integration
- Modular workflow architecture
- Easy extension for additional ATS providers

---

## Repository Structure

```
ATS-Job-Tracker
│
├── workflows
│   ├── ATS Job Tracker - Phase 1.json
│   ├── ATS Job Tracker - Phase 2.json
│   └── ATS Job Tracker - Workday.json
│
├── screenshots
│
├── docs
│
└── README.md
```

---

### Phase 1

![Phase 1](screenshots/Phase%201%20workflow.png)

### Phase 2

![Phase 2](screenshots/Phase%202%20workflow.png)

### Workday Module

![Workday](screenshots/Workday%20workflow.png)

### Google Sheet

![Google Sheet](screenshots/Google%20Sheet.png)

## Technologies Used

- n8n
- Google Sheets
- HTTP Request APIs
- JavaScript
- Git
- GitHub

---

## Current Status

Implemented:

- ATS detection
- Workday workflow
- API integration
- Job extraction
- Preferred role matching
- Google Sheets update workflow

---

## Future Scope

- Greenhouse ATS
- Lever ATS
- Oracle ATS
- SuccessFactors ATS
- SmartRecruiters
- Additional company integrations

---

## Author

**Dhruvi Singh**

Electronics and Communication Engineering

Interested in Communication Systems, Automation, and Cybersecurity.
