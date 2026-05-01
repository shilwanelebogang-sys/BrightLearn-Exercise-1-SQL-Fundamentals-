# 📊 SQL Fundamentals Portfolio Project — Employee Data Analysis

This project showcases my foundational SQL skills through a structured, hands-on analysis of an employee dataset. It simulates real-world business queries and demonstrates my ability to extract, filter, and present data effectively using SQL.

---

## 🚀 Project Overview

- ✔️ Developed 10 SQL queries based on business scenarios  
- ✔️ Applied filtering, sorting, and logical operators  
- ✔️ Practiced clean and readable SQL syntax  
- ✔️ Validated outputs and documented results  

This project reflects how SQL is used in real-world data analysis roles to support decision-making.

---

## 🗂 Dataset Description

**Table: `employees`**

| Column       | Description                  |
|-------------|------------------------------|
| id          | Unique employee ID           |
| first_name  | Employee first name          |
| last_name   | Employee last name           |
| department  | Department (IT, HR, etc.)    |
| salary      | Salary                       |
| hire_date   | Date of hire                 |
| city        | Employee location            |

---

## 🧠 Skills Demonstrated

- SQL query writing and structuring  
- Data filtering using `WHERE`, `AND`, `OR`, `NOT`, `IN`  
- Sorting with `ORDER BY`  
- Limiting results using `LIMIT`  
- Removing duplicates using `DISTINCT`  
- Translating business problems into SQL queries  

---

## 📌 Example Business Query

**Problem:** Identify high-earning IT employees located in Johannesburg.

```sql
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
