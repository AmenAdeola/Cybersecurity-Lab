The SELECT, FROM, and ORDER BY keywords are used when retrieving information from a database.

Commands|Purposes | Examples
--------|---------|---------
FROM| Indicates which table to query; required to perform a query | FROM employees: Indicates to query the employees table
ORDER BY | Sequences the records returned by a query based on a specified column or columns |ORDER BY department: Sorts the records in ascending order by the department column; ORDER BY department ASC: also sorts the records in ascending order by the department column; ORDER BY city DESC: Sorts the records in descending order by the city column; ORDER BY country, city: Sorts the records in ascending order by multiple columns; first sorts the output by country, and for records with the same country, sorts them based on city
SELECT | Indicates which columns to return; required to perform a query | SELECT employee_id: Returns the employee_id column; SELECT * Returns all columns in a table
