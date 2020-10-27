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

