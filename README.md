### 1. What is SQL?
**Answer:**
SQL (Structured Query Language) is a standard language for accessing and manipulating relational databases. It is used to query, insert, update, and delete data, as well as to create and modify the structure of database systems.

### 2. What are the different types of SQL statements?
**Answer:**
- DDL (Data Definition Language): CREATE, ALTER, DROP
- DML (Data Manipulation Language): SELECT, INSERT, UPDATE, DELETE
- DCL (Data Control Language): GRANT, REVOKE
- TCL (Transaction Control Language): COMMIT, ROLLBACK, SAVEPOINT

### 3. What is the difference between WHERE and HAVING?
**Answer:**
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

### 4. What is a primary key?
A primary key is a field in a table which uniquely identifies each row/record in that table. Primary keys must contain unique values and cannot contain NULL values.

### 5. What is a foreign key?
A foreign key is a field (or collection of fields) in one table that uniquely identifies a row of another table. The foreign key is defined in a second table, but it refers to the primary key or a unique key in the first table.

### 6. What is a join?
A JOIN clause is used to combine rows from two or more tables, based on a related column between them.

