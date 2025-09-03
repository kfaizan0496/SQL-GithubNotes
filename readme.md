# SQL Notes

## Introduction
SQL (Structured Query Language) is used to manage and manipulate relational databases.

---

## Basic Commands

### Creating a Table
```sql
CREATE TABLE table_name (
    column1 datatype,
    column2 datatype,
    ...
);
```

### Inserting Data
```sql
INSERT INTO table_name (column1, column2, ...)
VALUES (value1, value2, ...);
```

### Selecting Data
```sql
SELECT column1, column2
FROM table_name
WHERE condition;
```

### Updating Data
```sql
UPDATE table_name
SET column1 = value1
WHERE condition;
```

### Deleting Data
```sql
DELETE FROM table_name
WHERE condition;
```

---

## Useful Clauses

- `WHERE`: Filter records
- `ORDER BY`: Sort results
- `GROUP BY`: Group rows
- `HAVING`: Filter groups

---

## Example Query

```sql
SELECT name, age
FROM users
WHERE age > 18
ORDER BY age DESC;
```

---

## References

- [W3Schools SQL Tutorial](https://www.w3schools.com/sql/)
- [SQL Official Documentation](https://www.iso.org/standard/63555.html)

# Self learning

## create Database

```sql
create college;

```

## Use DB
```sql
use college;
```

## Create Table

![table](<Screenshot 2025-09-03 125159.png>)

```sql
CREATE TABLE student(
    id INT PRIMARY KEY,
    name VARCHAR(30),
    age INT NOT NULL
);

```
## Insert Data into tables

```sql
INSERT INTO student VALUES(1,"FAIZAN",26);
INSERT INTO student VALUES(2,"GHAZI",28);
INSERT INTO student VALUES(3,"RAJPAL",30);


```

## Insert  Mulitiple Data into tables
![alt text](<Screenshot 2025-09-03 161000.png>)

## View/Print Whole Table

```sql
select * from student;
```

## SQL Datatypes

![datatypes](<Screenshot 2025-09-03 130441.png>)

## Types of SQL commands

![SQL Commands](<Screenshot 2025-09-03 130934.png>)

## Database related queries

![Database related queries](<Screenshot 2025-09-03 131257.png>)

## Constraints
- SQL Constraints are used to specify rules for data in a table;
![Constraints](<Screenshot 2025-09-03 163103.png>)


##  2nd way to write primary key
 ![Primary key](<Screenshot 2025-09-03 163713.png>)

 ## Foreign key and default
 ![foreign](<Screenshot 2025-09-03 164026.png>)

 ## check constraints
 ```sql
 create table students(
stud_id int primary key, 
name varchar(20),
city varchar(20),
age int,
 constraint age_check check (age>=18 AND city="Delhi")
);
```

![Check constraints](<Screenshot 2025-09-03 174237.png>)


# project
- create database for college.
- create table of students.
- insert values

```sql
create database college;


```
1.**Use Database**
```sql
use college;

```


2.**create table**
```sql

create table student(
rollno int primary key,
name varchar(50),
marks  int not null,
grade varchar(1),
city varchar(20)

);

```

3.***insert Values**
```sql

insert into student(rollno,name,marks,grade,city)
values
(101,"Anil",78,"C","Pune"),
(102,"Bhumika",93,"A","Mumbai"),
(103,"Chetan",85,"B","Mumbai"),
(104,"Dhruv",96,"A","Delhi"),
(105,"Emanuel",12,"F","Delhi"),
(106,"Farah",82,"B","Delhi");

```

4.**View data based on query**
```sql
select name,marks from student;
```
![data](<Screenshot 2025-09-03 182721.png>)

5.**View all Table Data**
```sql
select * from student;

```

![all data](<Screenshot 2025-09-03 182921.png>)


## use "DISTINCT" Keyword
- used to extract unique data no duplicacy allowed

```sql
select distinct city from student;

```

![distinct](<Screenshot 2025-09-03 183250.png>)