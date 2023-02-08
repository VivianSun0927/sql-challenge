employees
-
emp_no INT PK
emp_title VARCHAR FK >- titles.title_id
birth_date DATE
first_name VARCHAR
last_name VARCHAR
sex VARCHAR
hire_date DATE

salaries
-
emp_no INT FK >- employees.emp_no
salary INT

dept_emp
-
emp_no INT FK >- employees.emp_no
dept_no INT FK >- departments.dept_no

dept_manager
-
dept_no INT FK >- departments.dept_no
emp_no INT FK >- employees.emp_no

titles
-
title_id VARCHAR PK
title VARCHAR

departments
-
dept_no VARCHAR PK
dept_name VARCHAR