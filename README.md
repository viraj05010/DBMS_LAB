# DBMS Lab - SQL Learning Repository

A comprehensive collection of SQL scripts for Database Management System (DBMS) lab exercises covering fundamental to intermediate SQL concepts.

## 📋 Repository Contents

### 1. **Creating Tables.sql**
Demonstrates the fundamentals of database and table creation:
- Creating a database (`college_db`)
- Creating multiple related tables (`students`, `instructor`, `alumni`)
- Using AUTO_INCREMENT for primary keys
- Inserting sample data
- Data types: INT, VARCHAR, DECIMAL
- Table descriptions and constraints

### 2. **Data Constraints.sql**
Covers database integrity and relationships:
- PRIMARY KEY constraints
- FOREIGN KEY constraints
- UNIQUE INDEX creation
- Table relationships (One-to-Many, Many-to-Many)
- Example: Department → Faculty → Student relationships
- Example: Department → Subject relationships

### 3. **Aggregates Function and Group By.sql**
Explores aggregate functions and grouping:
- **Aggregate Functions**: COUNT(), AVG(), SUM()
- Handling NULL values in aggregates
- GROUP BY clause for department-wise analysis
- Examples: Total count, salary calculations, department-wise averages

### 4. **Null Values and Null Values (Cont.).sql**
In-depth coverage of NULL value handling:
- IS NULL and IS NOT NULL operators
- Comparison with NULL values
- Logical operations (AND, OR, NOT) with unknown values
- Filtering records based on NULL conditions
- NULL in salary calculations

### 5. **Type of Joints.sql**
Comprehensive JOIN operations:
- **INNER JOIN**: Returns matching rows from both tables
- **LEFT JOIN**: Returns all rows from left table with matching rows from right
- **RIGHT JOIN**: Returns all rows from right table with matching rows from left
- **FULL OUTER JOIN**: Using UNION to combine LEFT and RIGHT joins
- **CROSS JOIN**: Cartesian product of two tables
- Examples with students and department tables

### 6. **Subqueries in Form and With Clause.sql**
Advanced query techniques:
- **Subqueries in FROM clause**: Using derived tables
- Aliasing subqueries for complex queries
- **Common Table Expressions (CTE)**: Using WITH clause
- Filtering results based on subquery results
- Example: Finding departments with average salary > 42000

### 7. **String and Set Operation, Order By.sql**
String operations and result set manipulation:
- **String Operations**: LIKE operator with wildcards (%, _)
- **ORDER BY**: Sorting in ascending (ASC) and descending (DESC) order
- **BETWEEN operator**: Range filtering
- **Set Operations**:
  - UNION: Combine results from multiple queries
  - Intersection logic: AND conditions
  - EXCEPT: Difference between two sets

### 8. **Exists and Not Exists.sql**
Existential logic in queries:
- EXISTS clause: Check for existence of rows in subqueries
- NOT EXISTS clause: Check for non-existence of rows
- Correlated subqueries
- Use case: Finding courses offered in both semesters

### 9. **SOME and ALL Clause.sql**
Comparative operations with multiple values:
- SOME operator: Compare value with any value in a set
- ALL operator: Compare value with all values in a set
- Salary comparison queries
- Department-wise comparisons

### 10. **SQL Triggers.sql**
Database triggers and automation:
- Creating triggers on INSERT events
- AFTER INSERT trigger: Logging teacher insertions
- BEFORE INSERT trigger: Computing derived values
- Conditional logic in triggers (IF-ELSE)
- Practical example: Auto-calculating student pass/fail status
- Delimiter management for trigger creation

### 11. **Views in SQL.sql**
Creating and using database views:
- Creating virtual tables (views) from queries
- JOIN-based views: `student_department_view`
- Filtered views: `high_marks_students`
- Using views for simplified queries
- Filtering data through views

## 📊 Sample Database Schema

### Tables Used:
- **students**: Student information (id, name, age, course, city, marks)
- **instructor**: Faculty information (id, name, department, salary)
- **alumni**: Alumni records (PRN, Name)
- **department**: Department details (dept_id, dept_name)
- **faculty**: Faculty information with department reference
- **subject**: Subject information linked to faculty and department
- **teacher**: Teacher records for trigger examples

## 🎯 Learning Objectives

This repository helps you master:
- ✅ Table creation and data insertion
- ✅ Data constraints and integrity
- ✅ Querying with aggregate functions
- ✅ NULL value handling
- ✅ Different types of JOINs
- ✅ Subqueries and CTEs
- ✅ String operations and sorting
- ✅ Set operations
- ✅ Existential logic (EXISTS/NOT EXISTS)
- ✅ Comparative operations (SOME/ALL)
- ✅ Triggers for automation
- ✅ Views for simplified data access

## 🚀 How to Use

1. **Set up the database**: Execute `Creating tables.sql` first to create the base schema
2. **Learn incrementally**: Follow the numbered files or specific topics
3. **Execute queries**: Run each SQL file in your DBMS (MySQL, PostgreSQL, SQL Server, etc.)
4. **Experiment**: Modify queries to understand different outcomes
5. **Combine concepts**: Create complex queries using multiple concepts

## 💻 Prerequisites

- Any SQL Database Management System (MySQL, PostgreSQL, SQL Server, SQLite, etc.)
- Basic understanding of SQL syntax
- Database client or terminal access

## 📝 Notes

- Some queries may need database-specific syntax adjustments
- Sample data is included in table creation files
- Use `DESCRIBE` or `DESC` command to view table structure
- The `DELIMITER //` syntax is specific to MySQL

## 📧 Author

DBMS Lab - SQL Learning Repository

---

**Happy Learning!** Feel free to fork, modify, and expand this repository with additional SQL concepts.
