# Perform Calculations in SQL  
## Count Rows  
```sql 
SELECT COUNT(*)
FROM log_in_attempts;
```

## Count by Group  
```sql 
SELECT department,
COUNT(*) AS employee_count
FROM employees GROUP BY department;
```
## Failed Logins by User  
```sql 
SELECT username,
COUNT(*) AS failed_attempts
FROM log_in_attempts
WHERE success = 0
GROUP BY username
ORDER BY failed_attempts DESC;
```
## Aggregate Functions  
| Function | Purpose |
|---|---|
| `COUNT()` | Count rows or values |
| `SUM()` | Add numeric values |
| `AVG()` | Calculate average |
| `MIN()` | Smallest value |
| `MAX()` | Largest value |  

## HAVING  Filters grouped results.  
```sql 
SELECT username,
COUNT(*) AS failed_attempts
FROM log_in_attempts
WHERE success = 0
GROUP BY username HAVING COUNT(*) >= 3;
```
Document the query, time range, data source, and interpretation when using calculations in an investigation. 
---------------

The following SQL keywords are aggregate functions and are helpful when performing calculations.

Commands| Purpose | Example|
--------|---------|--------|
AVG | Returns a single number that represents the average of the numerical data in a column; placed after SELECT| SELECT AVG(height): Returns the average height from all records that have a value in the height column
COUNT | Returns a single number that represents the number of records returned from a query; placed after SELECT| SELECT COUNT(firstname): Returns the number of records that have a value in the firstname column
SUM| Returns a single number that represents the sum of the numerical data in a column; placed after SELECT| SELECT SUM(cost):Returns the sum of costs from all records that have a value in the cost column


