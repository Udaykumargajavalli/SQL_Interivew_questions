### 1. What is SQL?

SQL (Structured Query Language) is a standard language for accessing and manipulating relational databases. It is used to query, insert, update, and delete data, as well as to create and modify the structure of database systems.
---
### 2. What are the different types of SQL statements?

- DDL (Data Definition Language): CREATE, ALTER, DROP
- DML (Data Manipulation Language): SELECT, INSERT, UPDATE, DELETE
- DCL (Data Control Language): GRANT, REVOKE
- TCL (Transaction Control Language): COMMIT, ROLLBACK, SAVEPOINT
---
### 3. What is the difference between WHERE and HAVING?

- `WHERE` filters rows before grouping.
- `HAVING` filters groups after aggregation.

Example:
```sql
SELECT department, COUNT(*) 
FROM employees 
WHERE salary > 50000 
GROUP BY department 
HAVING COUNT(*) > 5;
```
---
### 4. What is a primary key?
A primary key is a field in a table which uniquely identifies each row/record in that table. Primary keys must contain unique values and cannot contain NULL values.
---
### 5. What is a foreign key?
A foreign key is a field (or collection of fields) in one table that uniquely identifies a row of another table. The foreign key is defined in a second table, but it refers to the primary key or a unique key in the first table.
---
### 6. What is a join?
A JOIN clause is used to combine rows from two or more tables, based on a related column between them.
---
### 7. What are the different types of joins?
The different types of joins are INNER JOIN, LEFT JOIN (or LEFT OUTER JOIN), RIGHT JOIN (or RIGHT OUTER JOIN), and FULL JOIN (or FULL OUTER JOIN).
---
### 8. What is an index?
An index is a performance-tuning method of allowing faster retrieval of records from the table. An index creates an entry for each value and it will be faster to retrieve data.
---
### 9. What is normalization?
Normalization is the process of organizing data to minimize redundancy. Normalization usually involves dividing a database into two or more tables and defining relationships between the tables.
---
### 10. What is denormalization?
Denormalization is the process of attempting to optimize the read performance of a database by adding redundant data or by grouping data. It is the opposite of normalization.
---
### 11. What is a view?
A view is a virtual table based on the result-set of an SQL statement. It contains rows and columns, just like a real table. The fields in a view are fields from one or more real tables in the database.
---
### 12. What is a stored procedure?
A stored procedure is a prepared SQL code that you can save, so the code can be reused over and over again. You can also pass parameters to a stored procedure, so that the stored procedure can act based on the parameter value(s) that is passed.
---
### 13. What is a trigger?
A trigger is a set of SQL statements that automatically 'fires' or executes when certain events occur. Triggers are used to maintain the integrity of the information on the database.
---
### 14. What is a subquery?
A subquery is a query within another query. The outer query is called the main query, and the inner query is called the subquery. Subqueries are used to return data that will be used in the main query as a condition to further restrict the data to be retrieved.
---
### 15. What is a transaction?
A transaction is a sequence of one or more SQL operations treated as a unit. If one part of the transaction fails, the entire transaction fails, and the database state is left unchanged.
---
### 16. What is a constraint?
Constraints are used to specify rules for the data in a table. Constraints can be specified when the table is created (inside the CREATE TABLE statement) or after the table is created (inside the ALTER TABLE statement).
---
### 17. What is a unique constraint?
A unique constraint ensures that all values in a column are different. Both the UNIQUE and PRIMARY KEY constraints provide a guarantee for uniqueness for a column or set of columns.
---
### 18. What is a check constraint?
A check constraint is used to limit the value range that can be placed in a column. If you define a check constraint on a column, it will allow only certain values for this column.
---
### 19. What is a default constraint?
A default constraint is used to provide a default value for a column. The default value will be added to all new records if no other value is specified.
---
### 20. What is a composite key?
A composite key is a combination of two or more columns in a table that can be used to uniquely identify each row in the table.
---
### 21. What is a self join?
A self join is a regular join, but the table is joined with itself.
---
### 22. What is a cross join?
A cross join is a Cartesian product of the two tables involved in the join. The result set will contain all combinations of rows from the two tables.
---
### 23. What is a union?
The UNION operator is used to combine the result set of two or more SELECT statements. Each SELECT statement within the UNION must have the same number of columns in the result sets with similar data types.
---
### 24. What is the difference between UNION and UNION ALL?
The UNION operator selects only distinct values by default. The UNION ALL operator selects all values, including duplicates.
---
### 25. What is a cursor?
A cursor is a database object that allows you to retrieve each row from a result set one at a time. Cursors are used when the user needs to update records in a database table one row at a time.
---
### 26. What is an alias?
An alias is a temporary name given to a table or column for the purpose of a particular SQL query. Aliases are created to make table or column names more readable.
---
### 27. What is a case statement?
The CASE statement is SQL's way of handling if/then logic. It allows you to perform conditional logic in a SQL query.
---
### 28. What is the difference between DELETE and TRUNCATE?
DELETE is a DML command and removes rows one at a time and records an entry in the transaction log for each deleted row. TRUNCATE is a DDL command and removes all rows from a table without logging the individual row deletions.
---
### 39. What is the difference between DROP and TRUNCATE?
DROP is a DDL command that removes a table from the database. TRUNCATE is a DDL command that removes all rows from a table but does not remove the table itself.
---
### 40. What is the difference between CHAR and VARCHAR?
CHAR is a fixed-length data type, while VARCHAR is a variable-length data type. CHAR will always use the same amount of storage space, while VARCHAR will use only the amount of space needed to store the data.
---
### 41. What is the difference between IN and EXISTS?
The IN operator is used to compare a value to a list of values, while the EXISTS operator is used to check the existence of a result of a subquery.
---
### 42. What is the difference between a clustered and a non-clustered index?
A clustered index determines the physical order of data in a table and is used to improve the performance of data retrieval. A non-clustered index does not alter the physical order of data and is used to create a logical order for data rows.
---
### 43. What is the difference between a primary key and a unique key?
A primary key uniquely identifies each row in a table and cannot contain NULL values. A unique key also ensures the uniqueness of the column but can contain NULL values.
---
### 44. What is the difference between a left join and a right join?
A left join returns all rows from the left table and the matched rows from the right table. A right join returns all rows from the right table and the matched rows from the left table.
---
### 45. What is the difference between a full join and an inner join?
A full join returns all rows when there is a match in either table. An inner join returns only the rows that have matching values in both tables.
---
### 46. What is the difference between a subquery and a join?
A subquery is a query within another query, while a join is used to combine rows from two or more tables based on a related column between them.
---
### 47. What is the difference between a stored procedure and a function?
A stored procedure is a set of SQL statements that can perform a specific task, while a function is a set of SQL statements that can return a single value. Functions can be used in SQL statements, while stored procedures cannot.
---
### 48. What is the difference between a view and a table?
A view is a virtual table based on the result-set of an SQL statement, while a table is a collection of related data held in a structured format within a database.
---
### 49. What are the properties of a transaction in sql?
In SQL, the properties of a transaction are defined by the ACID principle, which ensures the reliability and integrity of database operations.

**1. Atomicity**

Definition: Atomicity ensures that a transaction is treated as a single, indivisible unit of work. Either all operations within the transaction are completed successfully, or none are.
Example: If you're transferring money from Account A to Account B, both the debit from A and the credit to B must succeed. If one fails, the entire transaction is rolled back.

**2. Consistency**

Definition: Consistency ensures that a transaction brings the database from one valid state to another, maintaining all predefined rules, such as constraints, cascades, and triggers.
Example: If a table has a constraint that a column must be unique, a transaction that violates this rule will not be allowed to commit.

**3. Isolation**

Definition: Isolation ensures that concurrent transactions do not interfere with each other. The intermediate state of a transaction is invisible to other transactions.
Example: If two users are booking the last seat on a flight simultaneously, isolation ensures that only one booking is confirmed, avoiding double-booking.

**4. Durability**

Definition: Durability guarantees that once a transaction is committed, its changes are permanent, even in the event of a system failure.
Example: After a successful transaction that updates a customer’s address, the new address remains saved even if the system crashes immediately afterward.
---
### 50. What is the difference between a temporary table and a table variable?
A temporary table is a table that is created and exists temporarily on the database server, while a table variable is a variable that holds a table and is created and exists temporarily in the memory.
---
### 51. What is the difference between a correlated subquery and a non-correlated subquery?
A correlated subquery is a subquery that references columns from the outer query, while a non-correlated subquery is a subquery that does not reference columns from the outer query.
---
### 52. Query to find Nth salary of employee data

```sql
SELECT DISTINCT salary
FROM Employee
ORDER BY salary DESC
LIMIT 1 OFFSET N-1;
```
---
### 53. Difference between rank and dense rank. Explain with an example
Both are window functions used to assign a ranking to rows based on a specific column's values. The key difference is how they handle ties (duplicate values).

`RANK()` and `DENSE_RANK()` are SQL window functions used to assign ranks to rows based on the order of a specified column. They are often used in analytical queries like finding top-N results or ranking employees by salary.

### 🔍 Key Differences

| Feature       | `RANK()`                          | `DENSE_RANK()`                     |
|---------------|-----------------------------------|------------------------------------|
| Tie Handling  | Same rank for ties, **skips** next rank(s) | Same rank for ties, **no skipping** |
| Gaps in Rank? | ✅ Yes                             | ❌ No                               |

### 📋 Sample Data

Let's assume we have the following `Employee` table:

```sql
| EmpID | Salary |
|-------|--------|
| 1     | 5000   |
| 2     | 6000   |
| 3     | 6000   |
| 4     | 7000   |

🏷 Example: Using RANK()
SELECT EmpID, Salary, RANK() OVER (ORDER BY Salary DESC) AS rank
FROM Employee;

| EmpID | Salary | Rank |
| ----- | ------ | ---- |
| 4     | 7000   | 1    |
| 2     | 6000   | 2    |
| 3     | 6000   | 2    |
| 1     | 5000   | 4    |

✅ Notice how rank 3 is skipped due to the tie on salary.

🏷 Example: Using DENSE_RANK()
SELECT EmpID, Salary, DENSE_RANK() OVER (ORDER BY Salary DESC) AS dense_rank
FROM Employee;

| EmpID | Salary | Dense\_Rank |
| ----- | ------ | ----------- |
| 4     | 7000   | 1           |
| 2     | 6000   | 2           |
| 3     | 6000   | 2           |
| 1     | 5000   | 3           |

🚫 No ranks are skipped, even with duplicate values.
```
✅ Summary
* Use RANK() if you want to preserve gaps when values are tied.
* Use DENSE_RANK() when you want consecutive ranks regardless of ties.
---
### 54. Different Types of SQL Joins

SQL joins are used to combine rows from two or more tables based on a related column.

### 1. ✅ INNER JOIN

Returns only matching rows between tables.

```sql
SELECT *
FROM Employees e
INNER JOIN Departments d ON e.DeptID = d.ID;
```
🔍 Keeps only rows where DeptID matches in both tables.

### 2. ⬅️ LEFT JOIN (or LEFT OUTER JOIN)

Returns all rows from the left table, and matching rows from the right.
```sql
SELECT *
FROM Employees e
LEFT JOIN Departments d ON e.DeptID = d.ID;
```
🔍 Unmatched right-side values are returned as NULL.

### 3. ➡️ RIGHT JOIN (or RIGHT OUTER JOIN)
Returns all rows from the right table, and matching rows from the left.
```sql
SELECT *
FROM Employees e
RIGHT JOIN Departments d ON e.DeptID = d.ID;
```
🔍 Unmatched left-side values are returned as NULL.

4. 🔄 FULL OUTER JOIN
Returns all rows when there is a match in either table.
```sql
SELECT *
FROM Employees e
FULL OUTER JOIN Departments d ON e.DeptID = d.ID;
```
🔍 Combines results of LEFT and RIGHT joins. Missing matches are shown as NULL.

5. ❌ CROSS JOIN
Returns Cartesian product — all possible combinations of rows.
```sql
SELECT *
FROM Employees
CROSS JOIN Departments;
```
🔍 Use with caution! Rows = A × B (can be huge).

📌 Summary Table
| Join Type       | Description                                | NULLs Possible? |
| --------------- | ------------------------------------------ | --------------- |
| INNER JOIN      | Matching rows from both tables             | ❌               |
| LEFT JOIN       | All from left + matched from right         | ✅ Right side    |
| RIGHT JOIN      | All from right + matched from left         | ✅ Left side     |
| FULL OUTER JOIN | All rows from both, matched where possible | ✅ Both sides    |
| CROSS JOIN      | All combinations (Cartesian product)       | ❌               |
---
### 55. Minimum and Maximum Rows Returned by SQL Joins

Understanding how many rows a SQL join can return is crucial for query optimization and avoiding unexpected results.

### 🔍 Join Behavior Summary

| Join Type          | Minimum Rows Returned                       | Maximum Rows Returned                      |
|--------------------|---------------------------------------------|--------------------------------------------|
| **INNER JOIN**     | `0` (if no matches exist in either table)   | `min(#rows in A, #rows in B)`              |
| **LEFT JOIN**      | `#rows in A`                                | `#rows in A` (with possible NULLs from B)  |
| **RIGHT JOIN**     | `#rows in B`                                | `#rows in B` (with possible NULLs from A)  |
| **FULL OUTER JOIN**| `max(#rows in A, #rows in B)`               | `#rows in A + #rows in B`                  |
| **CROSS JOIN**     | `#rows in A × #rows in B`                   | `#rows in A × #rows in B`                  |

> ✅ **Note**:  
> - `A` = Left Table  
> - `B` = Right Table  
> - `NULLs` appear when there's no match in non-preserved tables.

### 📘 Example Scenario

Let’s say:

- Table A (Employees): 3 rows  
- Table B (Departments): 2 rows

Then:

| Join Type          | Example Row Count Returned          |
|--------------------|-------------------------------------|
| **INNER JOIN**     | 0 to 2 (depends on matching `DeptID`)|
| **LEFT JOIN**      | 3 (always all from Employees)        |
| **RIGHT JOIN**     | 2 (always all from Departments)      |
| **FULL OUTER JOIN**| 3 to 5 (all unmatched + matched rows)|
| **CROSS JOIN**     | 3 × 2 = 6                            |


### 🔄 Join Behavior Explained

- **INNER JOIN**: Only rows with matching keys in both tables.
- **LEFT JOIN**: All rows from the left table, with NULLs where there's no match on the right.
- **RIGHT JOIN**: All rows from the right table, with NULLs where there's no match on the left.
- **FULL OUTER JOIN**: All rows from both sides, with NULLs for unmatched columns.
- **CROSS JOIN**: Every row in A joins with every row in B (Cartesian product).

📌 Useful for estimating result size and understanding query performance!

---










