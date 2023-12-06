# Pewlett Hackard Historical Workforce Analysis

## Project Introduction
As a newly appointed data engineer at Pewlett Hackard, I've embarked on a crucial research project focused on individuals employed by the company during the 1980s and 1990s. The challenge lies in the limited remnants of the employee database from that era, which are encapsulated in six CSV files.

## Objectivess
1. Data Modeling:
- Design appropriate SQL tables to effectively house the data extracted from the six CSV files.

2. Data Engineering:
- Import the CSV files into a SQL database, ensuring seamless integration and data integrity.

3. Data Analysis:
Answer key questions about the employee data, gaining insights into the workforce during the specified period.

## Completed tasks breakdown
### Data Engineering
## Tables Creation
1. Table: Employees
- Columns: employee_number (Primary Key), last_name, first_name, sex, salary
- Data Types: INT, VARCHAR(255), VARCHAR(255), CHAR(1), DECIMAL(10, 2)

2. Table: Departments
- Columns: department_number (Primary Key), department_name
- Data Types: INT, VARCHAR(255)

3. Table: Salaries
- Columns: employee_number (Primary Key, Foreign Key), salary, from_date, to_date
- Data Types: INT, DECIMAL(10, 2), DATE, DATE

4. Table: Titles
- Columns: employee_number (Primary Key, Foreign Key), title, from_date, to_date
- Data Types: INT, VARCHAR(255), DATE, DATE

5. Table: Dept_Employees
- Columns: employee_number (Primary Key, Foreign Key), department_number (Primary Key), from_date, to_date
- Data Types: INT, INT, DATE, DATE

6. Table: Dept_Managers
- Columns: department_number (Primary Key, Foreign Key), employee_number (Primary Key), from_date, to_date
- Data Types: INT, INT, DATE, DATE

## Import CSV Files
- Imported data from each CSV file into its corresponding SQL table.
- Ensured proper sequencing of table creation to handle foreign keys.

## Data Analysis
### Employee Information
1. Employee Details:
- Listed employee_number, last_name, first_name, sex, and salary for each employee.

2. 1986 Hires:
- Listed first_name, last_name, and hire_date for employees hired in 1986.

3. Department Managers:
- Listed manager details for each department, including department_number, department_name, employee_number, last_name, and first_name.

4. Employee Departments:
- Listed department_number for each employee, along with employee_number, last_name, first_name, and department_name.

5. Hercules Employees:
- Listed first_name, last_name, and sex for employees named Hercules with last names starting with B.

6. Sales Department Employees:
- Listed employee details for each Sales department employee, including employee_number, last_name, and first_name.

7. Sales and Development Department Employees:
- Listed employee details for Sales and Development departments, including employee_number, last_name, first_name, and department_name.

8. Employee Last Name Frequencies:
Provided frequency counts, in descending order, of all employee last names.

### Note
The completion of the data engineering and analysis phases establishes a robust foundation for exploring Pewlett Hackard's historical workforce. The tables are well-structured, and insightful queries provide a comprehensive view of employee details and organizational dynamics during the specified periods.