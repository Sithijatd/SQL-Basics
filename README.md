# <img width="25" height="25" src="https://img.icons8.com/external-those-icons-flat-those-icons/48/external-MySQL-programming-and-development-those-icons-flat-those-icons.png" alt="external-MySQL-programming-and-development-those-icons-flat-those-icons"/> **SQL For A/Ls** 

| **Data Definition** | **Data Manipulation** |
|:----:|:-----:|
|CREATE|SELECT|
|ALTER|INSERT INTO|
|DROP|UPDATE|
|RENAME|DELETE|

---
## ![sql-icon](https://img.icons8.com/external-vectorslab-flat-vectorslab/18/external-Sql-Website-servers-and-databases-vectorslab-flat-vectorslab.png) Create Database

```sql
CREATE DATABASE database_name;
```

මෙහිදී  `CREATE DATABASE` විධානය වන අතර, `database_name` සඳහා දත්ත් සමුදායෙහි නම ලබ දෙයි.

---

## Use Database (#use)

```sql
USE database_name;
```
`USE` විදානය මගින් දත්ත සමුදායට පිවිසීම සිදු කරනු ලබයි, `database_name` සඳහා දත්ත සමුදායෙහි නම භවිතා කරන්න.

---

## ![sql-icon](https://img.icons8.com/external-vectorslab-flat-vectorslab/18/external-Sql-Website-servers-and-databases-vectorslab-flat-vectorslab.png) CREATE Table

```sql
CREATE TABLE table_name (
  column1 datatype,
  column2 datatype,
  ...
);
```

The `CREATE TABLE` විදානය මගින් දත්ත සමුදය තුල නව වගුවක් නිර්මනය සිදුකරයි.

**උදාහරණ:**
```sql
CREATE TABLE students (
  id INT,
  name VARCHAR(50),
  age INT
);
```

---

## ![sql-icon](https://img.icons8.com/external-vectorslab-flat-vectorslab/18/external-Sql-Website-servers-and-databases-vectorslab-flat-vectorslab.png) ALTER Table

```sql
ALTER TABLE table_name
ADD column_name datatype;
```

The `ALTER TABLE` විදනය මගින් පවතින වගුවකට නව තිරුවක් එකතු කිරිම සිදු කරනු ලබයි.

**උදාහරණ:**
```sql
ALTER TABLE students
ADD grade VARCHAR(10);
```

---

## ![sql-icon](https://img.icons8.com/external-vectorslab-flat-vectorslab/18/external-Sql-Website-servers-and-databases-vectorslab-flat-vectorslab.png) DROP Table

```sql
DROP TABLE table_name;
```
`DROP TABLE` විදනය මගින් `table_name` ලෙස ලබා දෙන වගුව පවති නම් එය දත්ත සමුදායෙන් ඉවත් කිරීම සිදුකරනු ලබයි.


```sql
DROP TABLE students;
```

---

## ![sql-icon](https://img.icons8.com/external-vectorslab-flat-vectorslab/18/external-Sql-Website-servers-and-databases-vectorslab-flat-vectorslab.png) RENAME Table

```sql
RENAME TABLE old_name TO new_name;
```

`RENAME TABLE` විදනයෙන් පවතින වගුවක නමය වෙනස් කරනු ලබයි,
මෙහිදි `old_name` සඳහා පැරණි නමයද `new_name` සඳහා නව නමයද ලබාදෙනු ලබයි.

**උදාහරණ:**
```sql
RENAME TABLE students TO learners;
```

---

## ![sql-icon](https://img.icons8.com/external-vectorslab-flat-vectorslab/18/external-Sql-Website-servers-and-databases-vectorslab-flat-vectorslab.png) SELECT Data

```sql
SELECT column1, column2
FROM table_name;
```


`SELECT` විදානය මගින් වගුවක දත්ත තේරීම සිදු කරනු ලබයි.
`column1` සහ `column2` සඳහා දත්ත ලබාගැනීමට අවශ්‍ය තීරු ලබාදිමෙන් හෝ `*` හරහා සියලුම තීරු වල දත්ත තොරාගත හැකිය.

**උදාහරණ:**
```sql
SELECT name, age
FROM students;
```

---

## ![sql-icon](https://img.icons8.com/external-vectorslab-flat-vectorslab/18/external-Sql-Website-servers-and-databases-vectorslab-flat-vectorslab.png) INSERT INTO Table

```sql
INSERT INTO table_name (column1, column2)
VALUES (value1, value2);
```


`INSERT INTO` මගින් වගුවක් සඳහා දත්ත ඇතුලත් කිරීම සිදු කරයි.
**උදාහරණ:**
```sql
INSERT INTO students (id, name, age)
VALUES (1, 'Alice', 20);
```

---

## ![sql-icon](https://img.icons8.com/external-vectorslab-flat-vectorslab/18/external-Sql-Website-servers-and-databases-vectorslab-flat-vectorslab.png) UPDATE Data

```sql
UPDATE table_name
SET column1 = value1
WHERE condition;
```


 `UPDATE` විදානය මගින් වගුවක අති දත්තයක් යාවත්කලින කිරීම සිදු කරනු ලබයි. මෙහිදි `WHERE` සඳහා තිරුවක වෙනස් කිරීමට අවශ්‍ය දත්තයෙ ස්තනය ලබා දෙනු ලබයි.

**උදාහරණ:**
```sql
UPDATE students
SET age = 21
WHERE name = 'Alice';
```

---

## ![sql-icon](https://img.icons8.com/external-vectorslab-flat-vectorslab/18/external-Sql-Website-servers-and-databases-vectorslab-flat-vectorslab.png) DELETE Data

```sql
DELETE FROM table_name
WHERE condition;
```


`DELETE` command removes data from a table. Use the `WHERE` මගින් වගුවෙ ඉවත් කිරීමට අවශ්‍ය තිරුව ලබා දෙනු ලබයි.

**උදාහරණ:**
```sql
DELETE FROM students
WHERE age < 18;
```

---

`© 2024 This document was created for educational purposes and shared among friends.`

> ![git](https://img.icons8.com/external-those-icons-flat-those-icons/12/external-GitHub-Logo-social-media-those-icons-flat-those-icons.png) Made by [Sithija Dewmina](https://github.com/Sithijatd) 
