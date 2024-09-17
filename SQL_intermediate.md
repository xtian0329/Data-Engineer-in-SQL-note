## Roadmap
- querying database
- count and view specific records
- quey execution and style
- filtering
- aggregate functions
- sorting and grouping

# QUERY Function
Function 1: **COUNT()**
```sql
SELECT COUNT(birthdate) AS count_birthdates
FROM people;
```
counts the number of records with a value in the field
**count_birthdates** is an alias for clarity

```sql
SELECT COUNT(..) AS .., COUNT(..) AS ..
FROM ..;
```

```sql
SELECT COUNT(*) AS total_records(rows)
FROM ..;
```
\* represents all fields, count(*) represents the count records in a table.

Function 2: **DISTINCT()**
```sql
SELECT DISTINCT language
FROM films;
```
Combine COUNT with DISTINCT
```sql
SELECT COUNT(DISTINCT birthdate) AS COUNT_distinct_birthdates
FROM people;
```
# QUERY execution

Order of execution:

1. FROM
2. SELECT
3. eg. LIMIT

Debugging SQL:
<img width="1079" alt="Screenshot 2024-09-16 at 6 28 47 PM" src="https://github.com/user-attachments/assets/ce414c95-5a00-4f85-ba6e-15f6b9e89b4a">

SQL formatting:

1. several lines
2. write clear and readable code
3. Semicolon at the end of the sentence
4. Double quotes are used for identifiers (like table names or column names)
5. Single quotes are used for string literals

check https://www.sqlstyle.guide/

# Filtering execution

Function 1: **WHERE**
```sql
SELECT title
FROM films
WHERE release_year >1960;
```
|title                |
|---------------------|
|Judgment at Nuremberg|
|Pocketful of Miracles|
|The Hustler          |
|The Misfits          |
...

There are also "<", ">", "<=", ">=", "=" \
"<>" means **not equal to**

# Multiple Criteria

AND, OR, BETWEEN

<img width="535" alt="Screenshot 2024-09-16 at 9 01 21 PM" src="https://github.com/user-attachments/assets/5893dd23-ee82-4926-be5f-88fa3dc28e28">

When using WHERE and OR, specify the filtering clearly for each value:

<img width="518" alt="Screenshot 2024-09-16 at 9 21 57 PM" src="https://github.com/user-attachments/assets/6782998e-204d-46a4-934e-11a654367365">

Instead of blablabla = 12 or 20

Using AND and OR together:
<img width="1061" alt="Screenshot 2024-09-16 at 9 25 29 PM" src="https://github.com/user-attachments/assets/124d6507-65bb-4365-92b3-ce478bef17cc">

Using Between:

<img width="518" alt="Screenshot 2024-09-16 at 9 28 13 PM" src="https://github.com/user-attachments/assets/49d3638e-4847-4fc0-8ad2-dc2ed64a94f7">

We can also write between 1994 AND 2001 AND country = 'UK' (another AND statement)


