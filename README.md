# Payroll Service Database

## UC1

>To see all Database

`SHOW DATABASES;`

>Creating payroll Database

`CREATE DATABASE payroll_service;`

>To use payroll Database

`USE payroll_service;`

>To select current database

`SELECT DATABASE();`

## UC2 

> Creating table employee_payroll

```
CREATE TABLE employee_payroll
(
     id      INT unsigned NOT NULL AUTO_INCREMENT,
     name    VARCHAR(150) NOT NULL,
     salary  Double NOT NULL,
     start   DATE NOT NULL,
     PRIMARY KEY (id)
);

```

> To describe table

`DESCRIBE employee_payroll;`

## UC3

> Adding Data to employee payroll table

```
 INSERT INTO employee_payroll (name,salary,start) VALUES
    ('Karzman',700000,'2018-05-07'),
    ('Alex',900000,'2019-07-07'),
    ('Nadia',1200000,'2020-07-06');
```

> Retrieving Records in employee table

`SELECT * FROM employee_payroll;`

## UC4

>Retrieving salary records

`SELECT salary FROM employee_payroll;`

## UC5

> Retrieving Alex salary

`SELECT salary FROM employee_payroll WHERE name='Alex';`

> Selecting records after particular date

```
SELECT * FROM employee_payroll 
WHERE start BETWEEN CAST('2018-07-10' AS DATE) AND DATE(NOW());
```
