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