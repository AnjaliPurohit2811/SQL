
# SQL

## Employee DBMS

### Setup
To set up the database, execute the following SQL script to create the employees table:

```sql
CREATE TABLE employees (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name TEXT,
    role TEXT,
    salary INT
    age INT,
    address TEXT,
    phone INT
);
```

### Add Multiple Employees with Selective Data

```sql
INSERT INTO employees (name, role, salary, age, address, phone) VALUES ('ANJALI', 'CEO', 180000, 22, 'Surat', '9601046183');
INSERT INTO employees (name, role, salary, age, address, phone) VALUES ('DIPALI', 'CEO', 150000, 20, 'Surat', '1234567890');
INSERT INTO employees (name, role, salary, age, address, phone) VALUES ('MALTI', 'MANAGER', 100000, 22, 'Mumbai', '7894561230');
INSERT INTO employees (name, role, salary, age, address, phone) VALUES ('JOHN', 'TESTER', 95000, 20, 'Pune', '4569871230');
INSERT INTO employees (name, role, salary, age, address, phone) VALUES ('ANDREW', 'DEVELOPER', 70000, 19, 'Surat', '9874563210');
```

### Retrieve All Employee Information
```sql
SELECT * FROM EmployeesData;
```

### Find Employees with a Specific Role
```sql
SELECT * FROM EmployeesData WHERE role = 'Manager';
```

### Search for Employees with Names Containing "An"
```sql
SELECT * FROM EmployeesData WHERE like 'An%';
```

### Find Employees Older than 30 and Earning More than $70,000
```sql
SELECT * FROM EmployeesData WHERE age > 20 AND salary > 70000;
```

### Change the Salary of an Employee with ID 3
```sql
UPDATE employees SET salary = 90000 WHERE id = 5;
```

### Remove an Employee with ID 4
```sql
DELETE FROM employees WHERE id = 5;
```

## Delete All Employees with Age Less than 20
```sql
DELETE FROM employees WHERE age < 20;
```
