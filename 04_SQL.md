### SQL USEFUL Commands
SQL stands for Structured Query Language

Functionalities include: **creating** database, table, inserting records, **retrieve/read**, **update**, **delete** operations +  execute queries against a database.

Fact tables and dimension tables are key components of a schema in a data warehouse
|1. Dimension Table | 2. Fact Table    |
|-------------------|------------------|
|  Dimension tables, provide the context and background information for the measures recorded in the fact table. | A fact table contains records that combine attributes from different dimension tables.|
| A dimension table usually has a primary key and descriptive columns. Each row represents a unique dimension member.  |A fact table contains foreign keys that link to the dimension tables and measures. |

One of the main differences between fact tables and dimension tables is that dimension tables contain the attributes that the measures in the fact table are based on.

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
| **Windows Functions** |SUM(), AVG(), ROW_NUMBER(), RANK(), DENSE_RANK(), LEAD(), LAG()| |
|  SUM(), AVG()  |  SUM(revenue) OVER (PARTITION BY product_id ORDER BY sale_date) AS running_total  |  running total of revenue for each product, ordered by sale date   |
|   |    |    |
|   ROW_NUMBER(), RANK(), DENSE_RANK()| ROW_NUMBER() OVER (PARTITION BY product_id ORDER BY sale_date) AS row_num, RANK() OVER (PARTITION BY product_id ORDER BY sale_date) AS rank_val,    DENSE_RANK() OVER (PARTITION BY product_id ORDER BY sale_date) AS dense_rank_val   | Each row is assigned a row number based on its order within its respective product partition.   |
|  LEAD(), LAG()    | LEAD(revenue) OVER (PARTITION BY product_id ORDER BY sale_date) AS next_revenue,    LAG(revenue) OVER (PARTITION BY product_id ORDER BY sale_date) AS prev_revenue   |  ![image](https://github.com/dhirajmahato/Cheatsheet/assets/33785298/3d721717-2398-4dc0-a617-c05c2b1ca7d7)  |
| DATE and its Operations|    |    |
| formating   | SELECT YEAR(sale_date) AS sale_year, MONTH(sale_date) AS sale_month, DAY(sale_date) AS sale_day FROM sales;   |    |
| DATEADD()   | SELECT sale_date, DATEADD(DAY, 7, sale_date) AS future_date FROM sales;    |    |
| DATEDIFF()  | SELECT start_date, end_date, DATEDIFF(DAY, start_date, end_date) AS date_difference FROM date_ranges;    |    |

**GROUP BY** is used to aggregate and summarize data at a higher level, reducing the number of rows returned by the query.

**Window Functions** operate on the result set but do not reduce the number of rows; instead, they provide additional information about each row based on the defined window.

**Common Table Expression vs Subquery**- Differ in scope of reference within a query
```
-- CTE example
WITH HighSalaryEmployees AS (
    SELECT employee_id, employee_name, salary
    FROM employees
    WHERE salary > 50000
)
SELECT *
FROM HighSalaryEmployees;

-- Subquery example
SELECT department_name
FROM departments
WHERE department_id IN (
    SELECT department_id
    FROM employees
    WHERE salary > 50000
);
```
