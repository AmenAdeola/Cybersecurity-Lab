The SELECT, FROM, and ORDER BY keywords are used when retrieving information from a database.

Commands|Purposes | Examples
--------|---------|---------
FROM| Indicates which table to query; required to perform a query | FROM employees: Indicates to query the employees table
ORDER BY | Sequences the records returned by a query based on a specified column or columns |ORDER BY department: Sorts the records in ascending order by the department column; ORDER BY department ASC: also sorts the records in ascending order by the department column; ORDER BY city DESC: Sorts the records in descending order by the city column; ORDER BY country, city: Sorts the records in ascending order by multiple columns; first sorts the output by country, and for records with the same country, sorts them based on city
SELECT | Indicates which columns to return; required to perform a query | SELECT employee_id: Returns the employee_id column; SELECT * Returns all columns in a table

WHERE and the other SQL keywords and characters that follow are used when applying filters to SQL queries.
AND
Specifies that both conditions must be met simultaneously in a filter that contains two conditions

WHERE region = 5 AND country = 'USA'
Returns all records with a value in the region column of 5 and a value in the country column of 'USA'
BETWEEN
Filters for numbers or dates within a range; BETWEEN is followed by the first value to include in the range, the AND operator, and the last value to include in the range 

WHERE hiredate BETWEEN '2002-01-01' AND '2003-01-01'
Returns all records with a value in the hiredate column that is between '2002-01-01' and '2003-01-01'
= (equal to)
Used in filters to return only the records that contain a value in a specified column that is equal to a particular value

WHERE birthdate = '1980-05-15'
Returns all records with a value in the birthdate column that equals '1980-05-15'
> (greater than)
Used in filters to return only the records that contain a value in a specified column that is greater than a particular value

WHERE birthdate > '1970-01-01'
Returns all records with a value in the birthdate column that is greater than '1970-01-01'
>= (greater than or equal to)
Used in filters to return only the records that contain a value in a specified column that is greater than or equal to a particular value

WHERE birthdate >= '1965-06-30'
Returns all records with a value in the birthdate column that is greater than or equal to '1965-06-30'
< (less than)
Used in filters to return only the records that contain a value in a specified column that is less than a particular value 

WHERE date < '2023-01-31'
Returns all records with a value in the date column that is less than '2023-01-31'
