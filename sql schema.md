# SQL Schema

## Users Table

```sql
CREATE TABLE Users (
    user_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    password VARCHAR(255) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

## Medical_Reports Table

```sql
CREATE TABLE Medical_Reports (
    report_id INT PRIMARY KEY AUTO_INCREMENT,
    user_id INT,
    report_name VARCHAR(200),
    report_type VARCHAR(50),
    upload_date DATE,
    file_path VARCHAR(255),
    FOREIGN KEY (user_id) REFERENCES Users(user_id)
);


## Analysis_Results Table

```sql
CREATE TABLE Analysis_Results (
    analysis_id INT PRIMARY KEY AUTO_INCREMENT,
    report_id INT,
    extracted_text TEXT,
    summary TEXT,
    risk_level VARCHAR(50),
    analyzed_date DATE,
    FOREIGN KEY (report_id) REFERENCES Medical_Reports(report_id)
);


## Parameters Table

```sql
CREATE TABLE Parameters (
    parameter_id INT PRIMARY KEY AUTO_INCREMENT,
    parameter_name VARCHAR(100),
    normal_min FLOAT,
    normal_max FLOAT,
    unit VARCHAR(20)
);


## Result_Values Table

```sql
CREATE TABLE Result_Values (
    result_id INT PRIMARY KEY AUTO_INCREMENT,
    analysis_id INT,
    parameter_id INT,
    value FLOAT,
    is_abnormal BOOLEAN,
    FOREIGN KEY (analysis_id) REFERENCES Analysis_Results(analysis_id),
    FOREIGN KEY (parameter_id) REFERENCES Parameters(parameter_id)
);

## Database Relationships

* One User can upload multiple Medical Reports.
* One Medical Report can have one Analysis Result.
* One Analysis Result can contain multiple Parameter Values.
* Parameters store standard medical reference ranges.
* Result Values identify whether a parameter is Normal or Abnormal.

