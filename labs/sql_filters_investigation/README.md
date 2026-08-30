# SQL Filters Investigation

## Overview

This project demonstrates the use of SQL filters to investigate potential security issues within an organization's environment.

Using data stored in the 'employees' and 'log-in_attempts' tables, I applied SQL filtering techniques to identify failed login attempts, review suspicious activity, retrieve records from specific departments, and support security-related decision making.

## skills demonstrated

-  SLQ Querying
-  Data Retrieval
-  Data Filtering
-  Security Investigations
-  Access Monitoring
-  Log Analysis
-  SQL Pattern Matching
-  Cybersecurity Data Analysis

## SQL Concepts Used

-  Select
-  From
-  Where
-  And
-  Or
-  Not
-  Like
-  %
-  Limit

## Investigation Tasks

### Retrieve After-Hours Failed
Login Attempts

Identify unsuccessful login attempts that occurred after business hours.

### Retrieve Login Attempts on Specific Dates

Investigate login activity that occurred during a suspicious time period

### Retrieve Login Attempts Outside of Mexico

Filter authentication activity based on geographic location.

### Retrieve employees in Marketing

Identify employees who require a security update.

### Retrieve Employees in Finance or Sales

Identify users from multiple business units.

### Retrieve Employees Not in Information Technology

Determnine systems that still require updates outside the IT department.

## sample Query

'''sql
Select * from log_in_attempts where login_time >v'18:00:00' and sucess = o
