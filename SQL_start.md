# Introduction to SQL

## Databases Overview

- **Relational Databases**: Define relationships between tables of data.
- **Advantages**:
  - More storage than spreadsheet applications.
  - More secure storage.

---

## SQL Overview

- **SQL**: Structured Query Language, widely used for databases.
  - Example Query:
    ```sql
    SELECT * 
    FROM patrons 
    LIMIT 30;
    ```

---

## Tables

- **Records and Fields**: Table rows are called records, and columns are called fields.
- **Table Naming Conventions**:
  - Names should be lowercase.
  - Use underscores instead of spaces.
  - Refer to a collective group or be plural.
- **Field Naming Conventions**:
  - Names should be lowercase and singular.
  - No spaces or duplication with other field names or table names.
- **Unique Identifiers**: Used to identify records uniquely in a table (often numbers).

---

## SQL Data Types

- **Strings**: Sequence of characters (e.g., letters, punctuation).
  - Common data type: `VARCHAR`
- **Integers**: Whole numbers.
  - Common data type: `INT`
- **Floats**: Numbers including fractional parts.
  - Common data type: `NUMERIC`

## Querying

  - Example Query:
    ```sql
    SELECT name
    FROM patrons;
    ```
    Query results often called result set.
  - ```sql
    SELECT card_num, name
    FROM patrons;
    ```
    First column: card_num \
    Second column: name.
  - ```sql
    SELECT card_num, name
    FROM patrons;
    ```
    First column: name \
    Second column: card_num.
   - ```sql
     SELECT *
     FROM patrons;
     ```
     select all fields.

## Aliasing

  - ```sql
    SELECT name AS first_name, year_hired
    FROM employees;
    ```
    Rename fields.
  - ```sql
    SELECT year_hired
    FROM employees;
    ```
    Select the entire field "year_hired".
  - ```sql
    SELECT DISTINCT year_hired
    FROM employees;
    ```
    Select only the distinct year from the field "year_hired".
  - ```sql
    SELECTDISTINCT dept_id, year_hired
    FROM employees;
    ```
    | dept_id | year_hired |
    |---------|------------|
    | 1       | 2020       |
    | 2       | 2017       |
    | 2       | 2022       |
    | 3       | 2021       |
    | 2       | 2020       |
    Select multiple fields and apply distinct filter on them
## Views

 - A view is a virtual table that is the result of a saved SQL SELECT statement
 - When accessed, views automatically update in response to updates in the underlying data
```sql
CREATE VIEW employee_hire_years AS
SELECT id, name, year_hired
FROM employees;
```
 - example:
   ```sql
   SELECT id, name
   FROM employee_hire_years;
   ```
   | id    | name    |
   |-------|---------|
   | 54378 | Darius  |
   | 94722 | Raven   |
   | 45783 | Eduardo |
   | 90123 | Maggie  |
   | 67284 | Amy     |
   | 26148 | Meehir  |




