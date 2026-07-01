# React Project Setup

## Overview

The frontend of the AI-Based Medical Report Analyzer is developed using React.js to provide a fast, responsive, and user-friendly interface. React enables efficient component-based development and seamless integration with backend APIs.

---

## Project Initialization

Create a new React application using the following command:

```bash
npx create-react-app ai-medical-report-analyzer
```

Move to the project directory:

```bash
cd ai-medical-report-analyzer
```

Start the development server:

```bash
npm start
```

---

## Required Dependencies

Install the required packages:

```bash
npm install react-router-dom axios bootstrap
```

### Package Usage

| Package          | Purpose                |
| ---------------- | ---------------------- |
| react-router-dom | Navigation and Routing |
| axios            | API Communication      |
| bootstrap        | Responsive UI Design   |

---

## Project Structure

```text
src/
│
├── components/
│   ├── Navbar.jsx
│   ├── Sidebar.jsx
│   └── ReportCard.jsx
│
├── pages/
│   ├── Login.jsx
│   ├── Dashboard.jsx
│   ├── UploadReport.jsx
│   ├── AnalysisResult.jsx
│   ├── HealthSummary.jsx
│   └── Profile.jsx
│
├── services/
│   └── api.js
│
├── App.js
└── index.js
```

---

## Main Screens

### Login Page

Provides secure user authentication.

### Dashboard Page

Displays report statistics and recent activities.

### Upload Report Page

Allows users to upload medical reports for analysis.

### Analysis Result Page

Shows extracted medical data and AI-generated insights.

### Health Summary Page

Provides simplified medical report explanations.

### Profile Page

Manages user account information.

---

## API Integration

The React application communicates with the backend using REST APIs.

Example:

```javascript
axios.get("/api/reports")
     .then(response => console.log(response.data));
```

---

## Benefits of React

* Component-Based Architecture
* Fast Rendering with Virtual DOM
* Reusable UI Components
* Easy API Integration
* Responsive User Experience
* Scalable Application Structure

---

## Expected Outcome

The React frontend provides an intuitive interface for uploading medical reports, viewing analysis results, and accessing AI-generated health summaries efficiently.
