# Data Listing

## Overview

The Data Listing module displays all user information, uploaded medical reports, AI analysis results, and health summaries in a structured format. It helps users and administrators easily view, search, and manage stored data within the AI-Based Medical Report Analyzer system.

---

## Objective

* Display stored data in an organized manner.
* Provide quick access to medical reports and analysis results.
* Support searching and filtering of records.
* Improve data management and user experience.

---

## User Data Listing

Displays all registered users.

| Field Name        | Description                     |
| ----------------- | ------------------------------- |
| User ID           | Unique identifier for each user |
| Name              | User's full name                |
| Email             | Registered email address        |
| Registration Date | Account creation date           |

---

## Medical Report Listing

Displays uploaded medical reports.

| Field Name  | Description                  |
| ----------- | ---------------------------- |
| Report ID   | Unique report identifier     |
| Report Name | Name of the uploaded report  |
| Report Type | Blood Test, X-Ray, MRI, etc. |
| Upload Date | Date of report upload        |
| Status      | Pending / Completed          |

---

## Analysis Result Listing

Displays AI-generated analysis results.

| Field Name    | Description                 |
| ------------- | --------------------------- |
| Analysis ID   | Unique analysis identifier  |
| Report ID     | Associated medical report   |
| Risk Level    | Low, Medium, High           |
| Summary       | AI-generated health summary |
| Analysis Date | Date of analysis            |

---

## Health Parameter Listing

Displays extracted medical parameters.

| Parameter      | Normal Range | Patient Value | Status        |
| -------------- | ------------ | ------------- | ------------- |
| Hemoglobin     | 13–17 g/dL   | 14.2 g/dL     | Normal        |
| Blood Sugar    | 70–140 mg/dL | 165 mg/dL     | High          |
| Cholesterol    | <200 mg/dL   | 190 mg/dL     | Normal        |
| Blood Pressure | 120/80 mmHg  | 130/85 mmHg   | Slightly High |

---

## Features

* View all registered users
* View uploaded medical reports
* Display AI analysis results
* Search records by report name or date
* Filter reports by status
* Download report summaries

---

## Data Flow

1. User uploads a medical report.
2. Report details are stored in the database.
3. AI analyzes the report.
4. Analysis results are generated.
5. Data is displayed in the listing page.
6. Users can search, filter, and view detailed results.

---

## Expected Outcome

The Data Listing module provides a centralized and well-organized view of all project data, enabling users to efficiently access medical reports, AI-generated analyses, and health summaries while improving overall data management.
