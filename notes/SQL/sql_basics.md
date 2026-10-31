# SQL Basics  

## Query Structure  
```sql 
SELECT column_name FROM table_name
WHERE condition;
```

## Select All Columns  
```sql 
SELECT * FROM employees;
```
## Select Specific Columns  
```sql 
SELECT username, department
FROM employees;
```
## Limit Results  
```sql
SELECT * FROM employees 
LIMIT 15;
```
## Sort Results  
```sql 
SELECT *
FROM log_in_attempts
ORDER BY login_date DESC, login_time DESC;
```
## Security Relevance  
SQL helps analysts review login attempts, asset records, account information, alerts, and other structured investigation data. 
