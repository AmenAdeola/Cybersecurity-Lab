# Project Description

In this activity, I used SQL filtering techniques to investigate potential security issues within an organization's systems.
Using the employees and log_in_attempts tables, I applied filters with WHERE, AND, OR, NOT, and LIKE to identify suspicious login activity and retrieve employee records requiring security updates. This project demonstrates how SQL can be used to support security investigations and operational decision-making.


# Retrieve After Hours Failed Login Attempts
Query
SQL:
Select * From log_in_attempts where login_time > '18:00:00" and success = 0;
Explanation: This query identifies failed login attempts that occurred after business hours. The AND operator ensures that only records meeting both conditions are returned: the login occurred later 18:00 and the attempt was unsuccessful

# Retrieve Login Attempts on Specific Dates
Query
SQL:
Select * from log_in_attempts where login_date = '2022-05-09' or login_dates = '2022-0508';
Explanation: this query retrieves login activity that occurred on a suspicious date and the day before. The OR operator allows records matching either date to be returned.

# Retrieve Login Attempts Outside of MEXICO
Query
SQL:
Select * from log_in_attempts where country NOT like 'MEX%' and country NOT like 'MEXICO%';
Explanation: This query identifies login attempts that did not originate from Mexico. The NOT and LIKE operators are used together to exclude records whose country values begin with MEX or MEXICO.

# Retrieve Employees in Marketing
Query
SQL: 
select * from employees where department = 'Marketing' and office like 'East%';
Explanation: This query identifies Marketing employees located in East offices. The AND operator requires both conditions to be true.

# Retrieve Employees in Finance or Sales
Query
SQL:
select * from employees where department = 'Finance' or department = 'Sales';
Explanation: This query retrieves employees who belong to either the Finance or Sales departments using the OR operator.

# Retrieve All Employees Not in IT
Query
SQL:
Select * from employees where NOT department = 'Information technology';

                  OR
Select * from employees where department <> 'Information technology';
Explanation: This query excludes Information Technology employees and returns all remaining departments. The query supports identifying systems that still require updates.

# Summary
This project demonstrates the use of SQL filtering techniques to investigate login activity and retrieve employee information. By applying WHERE, AND, OR, NOT, and LIKE operators, I was able to identify suspicious logins, isolate records based on dates and geographic locations, and retrieve employee groups requiring security actions. these skills are commonly used in cybersecurity investigations and incident analysis.

Explanation:
              
