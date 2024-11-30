# **SQL**

| **Data Definition** | **Data Manipulation** |
| ------------------- | --------------------- |
| [CREATE](#create-database)              | [SELECT](#select-data)                |
| [ALTER](#alter-table)               | [INSERT INTO](#insert-into-table)           |
| [DROP](#drop-table)                | [UPDATE](#update-data)                |
| [RENAME](#rename-table)              | [DELETE](#delete-data)                |

## Create Database {#create-database}

> Command

```sql
CREATE DATABASE database_name;
```

**Explanation:**
The `CREATE DATABASE` command is used to create a new database. Replace `database_name` with the desired name of your database.

**Example Output:**
When executed, this command creates a database named `school`.

```sql
CREATE DATABASE school;
```

---

## Use Database {#use-database}

> Command

```sql
USE database_name;
```

**Explanation:**
The `USE` command sets the context to a specific database so that subsequent commands operate on it. Replace `database_name` with the name of the database you want to use.

**Example Output:**

```sql
USE school;
```

---

## CREATE Table {#create-table}

> Command

```sql
CREATE TABLE table_name (
  column1 datatype,
  column2 datatype,
  ...
);
```

**Explanation:**
The `CREATE TABLE` command creates a new table with specified columns and data types.

**Example Output:**

```sql
CREATE TABLE students (
  id INT,
  name VARCHAR(50),
  age INT
);
```

---

## ALTER Table {#alter-table}

> Command

```sql
ALTER TABLE table_name
ADD column_name datatype;
```

**Explanation:**
The `ALTER TABLE` command is used to modify an existing table by adding, deleting, or modifying columns.

**Example Output:**

```sql
ALTER TABLE students
ADD grade VARCHAR(10);
```

---

## DROP Table {#drop-table}

> Command

```sql
DROP TABLE table_name;
```

**Explanation:**
The `DROP TABLE` command removes an existing table and all its data.

**Example Output:**

```sql
DROP TABLE students;
```

---

## RENAME Table {#rename-table}

> Command

```sql
RENAME TABLE old_name TO new_name;
```

**Explanation:**
The `RENAME TABLE` command changes the name of an existing table.

**Example Output:**

```sql
RENAME TABLE students TO learners;
```

---

## SELECT Data {#select-data}

> Command

```sql
SELECT column1, column2
FROM table_name;
```

**Explanation:**
The `SELECT` command is used to retrieve data from a table. Replace `column1` and `column2` with the columns you want to retrieve, or use `*` to select all columns.

**Example Output:**

```sql
SELECT name, age
FROM students;
```

---

## INSERT INTO Table {#insert-into-table}

> Command

```sql
INSERT INTO table_name (column1, column2)
VALUES (value1, value2);
```

**Explanation:**
The `INSERT INTO` command adds new data to a table. Specify the columns and corresponding values to insert.

**Example Output:**

```sql
INSERT INTO students (id, name, age)
VALUES (1, 'Alice', 20);
```

---

## UPDATE Data {#update-data}

> Command

```sql
UPDATE table_name
SET column1 = value1
WHERE condition;
```

**Explanation:**
The `UPDATE` command modifies existing data in a table. Use the `WHERE` clause to specify which rows to update.

**Example Output:**

```sql
UPDATE students
SET age = 21
WHERE name = 'Alice';
```

---

## DELETE Data {#delete-data}

> Command

```sql
DELETE FROM table_name
WHERE condition;
```

**Explanation:**
The `DELETE` command removes data from a table. Use the `WHERE` clause to specify which rows to delete.

**Example Output:**

```sql
DELETE FROM students
WHERE age < 18;
```

---

---

*This document was created for educational purposes and shared among friends.*

**Made by Sithija Dewmina**
