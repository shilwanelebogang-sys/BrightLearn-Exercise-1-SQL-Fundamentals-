# 📊 SQL Fundamentals — SELECT & Filtering Exercise

This exercise demonstrates my ability to retrieve, filter, and organize structured data using SQL.

Using an employee dataset, I solved 10 queries that simulate common business scenarios such as identifying high-performing employees, filtering by department, and ranking salaries.

---

## 🚀 Exercise Overview

In this exercise, I worked with a single dataset (`employees`) to:

- Retrieve data using `SELECT`  
- Filter records using `WHERE` conditions  
- Apply logical operators (`AND`, `OR`, `NOT`, `IN`)  
- Sort data using `ORDER BY`  
- Limit results using `LIMIT`  

The exercise reflects how SQL is used in:
- Operational reporting  
- Employee and HR analysis  
- Basic data extraction tasks  

---

## 🧠 Skills Demonstrated

### 🔹 SQL Fundamentals
- Selecting all vs specific columns  
- Removing duplicates using `DISTINCT`  
- Filtering rows using `WHERE`  
- Sorting results with `ORDER BY`  
- Limiting output using `LIMIT`  

### 🔹 Query Logic & Structure
- Use of logical operators (`AND`, `OR`, `NOT`, `IN`)  
- Writing clean and readable SQL queries  
- Understanding SQL clause order  

### 🔹 Analytical Thinking
- Translating business questions into SQL queries  
- Filtering datasets based on multiple conditions  
- Identifying key records (e.g., top earners)  

### 🔹 Data Validation & Presentation
- Manual validation of outputs  
- Structuring query results clearly  
- Documenting queries and expected outputs  

---

## 🗂 Dataset Used

### `employees`

| Column       | Description                  |
|-------------|------------------------------|
| id          | Employee ID                  |
| first_name  | First name                   |
| last_name   | Last name                    |
| department  | Department                   |
| salary      | Salary                       |
| hire_date   | Date of hire                 |
| city        | Employee location            |

---

## 💻 SQL Queries

```sql
-- Question 1
SELECT * FROM employees;

-- Question 2
SELECT DISTINCT department FROM employees;

-- Question 3
SELECT first_name, last_name
FROM employees
ORDER BY salary DESC;

-- Question 4
SELECT id, first_name, last_name, salary
FROM employees
ORDER BY salary DESC
LIMIT 3;

-- Question 5
SELECT id, first_name, last_name, department
FROM employees
WHERE department = 'IT';

-- Question 6
SELECT id, first_name, last_name, department, salary
FROM employees
WHERE department = 'Finance'
AND salary > 60000;

-- Question 7
SELECT id, first_name, last_name, department
FROM employees
WHERE department = 'HR'
OR department = 'Marketing';

-- Question 8
SELECT id, first_name, last_name, department
FROM employees
WHERE department <> 'IT';

-- Question 9
SELECT id, first_name, last_name, department
FROM employees
WHERE department IN ('IT', 'HR', 'Finance');

-- Question 10
SELECT 
    id, 
    first_name, 
    last_name, 
    department, 
    salary, 
    city
FROM employees
WHERE department = 'IT'
AND salary > 65000
AND city = 'Johannesburg';
