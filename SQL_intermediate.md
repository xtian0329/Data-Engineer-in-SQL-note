## Roadmap
- querying database
- count and view specific records
- quey execution and style
- filtering
- aggregate functions
- sorting and grouping

Function 1: **COUNT()**
```sql
SELECT COUNT(birthdate) AS count_birthdates
FROM people;
```
counts the number of records with a value in the field
**count_birthdates** is an alias for clarity

```sql
SELECT COUNT(..) AS .., COUNT(..) AS ..
FROM ..
```
