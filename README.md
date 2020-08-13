# Comparing The Number of Managers based on Gender: Project Overview 
* Created SQL query language using MySQL to compare number of managers based on their gender.
* Database used was consisted with 3 tables, which were employees, departments, and department managers table.
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
**1. Employees table:** (t_employees) 
<br />Table of employee's details that consisted with 135369 rows and 6 columns, which are:
* Employee number (emp_no) **primary key**
* Employee's birth date (birth_date)
* Employee's first name (first_name)
* Employee's last name (last_name)
* Employee's gender (gender)
* Employee's hire date (hire_date)

**2. Departments table:** (t_departments)
<br />Table of company's departments details consisted with 9 rows and 2 columns, which are:
* Department number (dept_no) **primary key**
* Department name (dept_name)

**3. Department managers table:** (t_dept_manager)
<br />Table of company's department manager details consisted with 144 rows and 4 columns, which are:
* Employee number (emp_no) **foreign key**
* Department number (dept_no) **foreign key**
* Date of start as manager (from_date)
* Date of quit as manager (to_date)

## Query Building 
Before building the query, I defined columns that were needed to be returned for clasifying managers by gender. Column that were returned are:
<br />
* Department name (dept_name) from **Departments table**
* Employee's gender (gender) from **Employees data**
* Date of start as manager (from_date) from **Department managers table**
* Date of quit as manager (to_date) from **Department managers table**
* The year of employee's hire date (calendar_year) YEARS format of (hire_date) from **Employees data**
* The active status of manager, compared from their managerial periode and hire date (active_status) from **Employees data** and **Department managers table**
<br />
To get the columns needed, I did a CROSS JOIN to join all tables based on their relation. 
<br />These are the link to the [Task Query](https://github.com/novaldi21/ds_sql_project/blob/master/Task_query.sql) and [Return Spreadsheet](https://github.com/novaldi21/ds_sql_project/blob/master/Task.csv)

## Data Visualization
Data visualization was built using Tableau and using the return spreadsheet from query. Data visualization is presented below and from the figure we can se that the proportion of male manager (blue) and female manager (orange) in the company from 1990 to 2002 are about 3:2 (60% male and 40% female)
![Alt](https://github.com/novaldi21/ds_sql_project/blob/master/task_visualization.png)


