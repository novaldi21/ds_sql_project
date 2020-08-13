# Comparing The Number of Managers based on Gender: Project Overview 
* Created SQL query language using MySQL to compare number of managers based on their gender.
* Database used was consisted with 3 tables, which were employees data, departments data, department managers data.
* Number of rows and columns for tables: employees data (135369, 6), departments data (9, 2), department managers data (144, 4)
* Created data visualization using Tableau.

## Code and Resources Used 
**MySQL Version:** 8.0  
**Tableau Public:** 2020.1

## Project Task 
The task of the project was "Compare the number of male managers to the number of female managers from different departments for each year from 1990 to 2002"

## Database
Database used for the project is employee database named "employee_mod_db" that consisted with 3 tables, which are:
<br />
**1. Employees data:** (t_employees) 
<br />Table of employee's details that consisted with 135369 rows and 6 columns, which are:
* Employee number (emp_no) **primary key**
* Employee's birth date (birth_date)
* Employee's first name (first_name)
* Employee's last name (last_name)
* Employee's gender (gender)
* Employee's hire date (hire_date)

**2. Departments data:** (t_departments)
<br />Table of company's departments details consisted with 9 rows and 2 columns, which are:
* Department number (dept_no) **primary key**
* Department name (dept_name)

**3. Department managers data:** (t_dept_manager)
<br />Table of company's department managers details consisted with 144 rows and 4 columns, which are:
* Employee number (emp_no) **foreign key**
* Department number (dept_no) **foreign key**
* Date of start as manager (from_date)
* Date of quit as manager (to_date)
