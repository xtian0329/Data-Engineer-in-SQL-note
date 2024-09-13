# Introduction to SQL

## Course Goals
1. Understand databases and their structure (Chapter 1)
2. Extract information from databases using SQL (Chapter 2)

---

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

