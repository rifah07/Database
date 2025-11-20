# Introduction to SQL

SQL (Structured Query Language) is the standard language used to communicate with relational databases. It allows you to create, read, update, and delete (CRUD) data stored in tables.

## Key Concepts

- **Database:** A collection of organized data.
- **Table:** A set of rows and columns where data is stored.
- **Row:** A single record in a table.
- **Column:** A field in a table representing a data attribute.
- **Primary Key:** A column (or set of columns) that uniquely identifies each row.
- **Foreign Key:** A column that creates a relationship between two tables.

## Basic SQL Commands

- **SELECT:** Retrieve data from one or more tables.
- **INSERT:** Add new rows to a table.
- **UPDATE:** Modify existing rows.
- **DELETE:** Remove rows from a table.
- **CREATE TABLE:** Define a new table.
- **ALTER TABLE:** Modify an existing table.
- **DROP TABLE:** Delete a table.

---

# SQL Questions

## 1. Write a query to select all columns from a table called `employees`.

```
SELECT * FROM employees;
```

## 2. Write a query to find the name and salary of employees who earn more than 50,000.

```
SELECT name, salary FROM employees WHERE salary > 50000;
```

## 3. Write a query to insert a new employee into the `employees` table.
```
INSERT INTO employees (name, position, salary) VALUES ('John Doe', 'Developer', 60000);
```
