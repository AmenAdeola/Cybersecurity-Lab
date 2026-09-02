The following SQL keywords are used to join tables.
FULL OUTER JOIN
Returns all records from both tables; the column used to join the tables is specified following FULL OUTER JOIN with syntax that includes ON and equal to (=)

SELECT *
FROM employees
FULL OUTER JOIN machines ON employees.device_id = machines.device_id;
Returns all records from the employees table and machines table; uses the device_id column to join the two tables
INNER JOIN
Returns records matching on a specified column that exists in more than one table; the column used to join the tables is specified following INNER JOIN with syntax that includes ON and equal to (=)

SELECT *
FROM employees
INNER JOIN machines ON employees.device_id = machines.device_id;
Returns all records that have a value in the  device_id column in the employees table that matches a value in the device_id column in the machines table
LEFT JOIN
Returns all the records of the first table, but only returns records of the second table that match on a specified column; the first (or left) table appears directly after the keyword FROM; the column used to join the tables is specified following LEFT JOIN with syntax that includes ON and equal to (=)

SELECT *
FROM employees
LEFT JOIN machines ON employees.device_id = machines.device_id;
Returns all records from the employees table but only the records from the machines table that have a value in the device_id column that matches a value in the device_id column in the employees table
RIGHT JOIN
Returns all of the records of the second table, but only returns records from the first table that match on a specified column; the second (or right) table appears directly after the RIGHT JOIN keyword; the column used to join the tables is specified following RIGHT JOIN with syntax that includes ON and equal to (=)

SELECT *
FROM employees
RIGHT JOIN machines ON employees.device_id = machines.device_id;
Returns all records from the machines table but only the records from the employees table that have a value in the device_id column that matches a value in the device_id column in the machines table

