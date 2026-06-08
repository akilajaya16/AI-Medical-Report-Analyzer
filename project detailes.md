# AI-Based Medical Report Analyzer

## Project Title

AI-Based Medical Report Analyzer

## Problem Statement

Medical reports often contain complex medical terminology and numerical test results that are difficult for patients to understand. Manual interpretation of these reports can be time-consuming and may require professional assistance. There is a need for an intelligent system that can automatically analyze medical reports and provide clear, understandable insights to users.

## Project Objectives

* To automate the analysis of medical reports using Artificial Intelligence.
* To extract important medical data from uploaded reports.
* To identify abnormal values and health indicators.
* To generate easy-to-understand summaries for patients.
* To reduce the time required for report interpretation.
* To improve accessibility to healthcare information.

## Module List

1. User Authentication Module
2. Medical Report Upload Module
3. OCR Text Extraction Module
4. AI Analysis Module
5. Abnormal Value Detection Module
6. Health Summary Generation Module
7. Report History Management Module
8. Admin Dashboard Module

## Table List

### User Table

| Field Name | Data Type    |
| ---------- | ------------ |
| user_id    | INT          |
| name       | VARCHAR(100) |
| email      | VARCHAR(100) |
| password   | VARCHAR(255) |

### Medical_Report Table

| Field Name  | Data Type    |
| ----------- | ------------ |
| report_id   | INT          |
| user_id     | INT          |
| report_name | VARCHAR(200) |
| upload_date | DATE         |
| report_file | VARCHAR(255) |

### Analysis_Result Table

| Field Name     | Data Type   |
| -------------- | ----------- |
| analysis_id    | INT         |
| report_id      | INT         |
| extracted_text | TEXT        |
| summary        | TEXT        |
| risk_level     | VARCHAR(50) |
| analyzed_date  | DATE        |

## Technologies Used

* Frontend: HTML, CSS, JavaScript, Bootstrap
* Backend: Java, Spring Boot
* Database: MySQL
* AI/ML: Python, TensorFlow, Scikit-learn
* OCR: Tesseract OCR

## Expected Outcome

The system will automatically analyze medical reports, identify abnormal findings, and provide simplified health summaries, helping users better understand their medical information.
