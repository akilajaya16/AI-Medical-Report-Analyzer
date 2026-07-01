# Registration Module

## Overview

The Registration Module enables new users to create an account in the AI-Based Medical Report Analyzer system. It collects user information, validates the entered data, and securely stores user details in the database for future authentication and access.

---

## Objective

* Allow new users to register in the system.
* Collect essential user information.
* Validate registration details.
* Store user data securely.
* Create unique user accounts.

---

## Features

### New User Registration

Users can create an account by providing their personal information.

### Input Validation

The system validates all required fields before registration.

### Unique Email Verification

Prevents duplicate accounts using the same email address.

### Secure Password Storage

Passwords are encrypted before storing in the database.

### Registration Confirmation

Users receive confirmation after successful account creation.

---

## Registration Process

1. User enters Name.
2. User enters Email Address.
3. User creates Password.
4. User confirms Password.
5. System validates the entered information.
6. User details are stored in the database.
7. Registration is completed successfully.
8. User can proceed to Login.

---

## Input Fields

| Field Name       | Type     | Description           |
| ---------------- | -------- | --------------------- |
| Name             | Text     | Full Name of User     |
| Email            | Email    | Unique Email Address  |
| Password         | Password | User Password         |
| Confirm Password | Password | Password Verification |

---

## Validation Rules

* Name field cannot be empty.
* Email field must be unique.
* Email must follow valid format.
* Password must contain minimum required characters.
* Password and Confirm Password must match.

---

## Database Interaction

The Registration Module stores user information in the Users table.

### Users Table

| Field Name | Description                |
| ---------- | -------------------------- |
| user_id    | Unique User Identifier     |
| name       | User Full Name             |
| email      | Registered Email Address   |
| password   | Encrypted Password         |
| created_at | Registration Date and Time |

---

## Security Features

* Password Encryption
* Duplicate Email Prevention
* Input Validation
* Secure User Data Storage

---

## Expected Outcome

The Registration Module allows users to create secure accounts and gain access to the AI-Based Medical Report Analyzer system. It ensures data integrity, security, and reliable user management.
