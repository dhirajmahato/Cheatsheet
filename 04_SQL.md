### SQL USEFUL Commands
SQL stands for Structured Query Language

Functionalities include: **creating** database, table, inserting records, **retrieve/read**, **update**, **delete** operations +  execute queries against a database.


Clauses    |  Query  | Usage
-------------|---------------------|---------------------|
| SELECT  | SELECT * FROM Student;  | * Shows all the records available in the _Student_ Table  |
| DISTINCT  |  SELECT DISTINCT Country FROM Customers; | Shows distinct _Country_ which is a field recorded in the _Customer_ table  |
| WHERE  | SELECT Country FROM Customers WHERE Country ='INDIA' ; | Filter those rows where _Country_ field has value as "INDIA" |
| IN  | SELECT * FROM Customers WHERE Country IN ('Germany', 'France', 'UK'); |   |
| BETWEEN  | SELECT * FROM Orders WHERE OrderDate BETWEEN '1996-07-01' AND '1996-07-31'; |  shows records between the given range |
| CASE | CASE WHEN salary > 50000 THEN 'High Salary'  WHEN salary >= 30000 AND salary <= 50000 THEN 'Medium Salary'  ELSE 'Low Salary'  END AS salary_category|  categorical  conditional logical data segregation within a query |
| ORDER BY |  SELECT name FROM Customers ORDER by name ASC | arrange the records in _name_ field in ascending order  |
|  **Aggregate function** | MAX(), MIN(), COUNT(), AVG(), SUM()|   |
| GROUP BY | SELECT COUNT(CustomerID), Country FROM Customers GROUP BY Country| groups rows that have the same values |
| FILTER  | SELECT department,    AVG(salary) FILTER (WHERE salary > 50000) AS avg_high_salary,    AVG(salary) FILTER (WHERE salary >= 30000 AND salary <= 50000) AS avg_medium_salary,    AVG(salary) FILTER (WHERE salary < 30000) AS avg_low_salary FROM employees GROUP BY department; | when you want to apply conditions to the rows being aggregated within the aggregate function itself. |
| HAVING  |  SELECT COUNT(CustomerID), Country FROM Customers GROUP BY Country HAVING COUNT(CustomerID) > 5; | when you want to filter the results of aggregate functions based on conditions after grouping. |
| **Windows Functions** | | |
