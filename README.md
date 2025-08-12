# SQL-Task-6
# Overview

This project demonstrates the use of SQL subqueries to retrieve, filter, and manipulate data efficiently.
The database is created from scratch, sample data is inserted, and multiple queries are written to showcase nested queries in real-world scenarios.


---

# Setup Instructions

1. Create the database
Run the CREATE DATABASE statement provided in the script.


2. Switch to the new database

USE your_database_name;


3. Create tables
Execute all the CREATE TABLE statements from the script to set up the structure.


4. Insert sample data
Run all INSERT INTO statements to populate the database.


5. Run subqueries
Execute each SQL subquery provided in the script to see how data is filtered or computed using nested queries.




---

# File Structure

subqueries.sql → Contains all SQL commands from database creation to subquery execution.



---

# Key Concepts Covered

Single-row subqueries (e.g., retrieving the maximum salary and finding employees with that salary)

Multiple-row subqueries (e.g., using IN, ANY, ALL)

Nested subqueries (e.g., subqueries inside WHERE clauses)

Subqueries with aggregation functions (MAX, MIN, AVG)

Correlated subqueries (queries that depend on outer queries)



---

# Example Subquery

SELECT name, salary
FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);

This query returns all employees whose salary is greater than the average salary.

