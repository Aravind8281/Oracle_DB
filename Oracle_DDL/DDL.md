DDL (Data Definition Language) in Oracle SQL is used to define, modify, and remove database objects such as tables, indexes, views, sequences, and so on. Here are the basic syntax examples for some common DDL statements in Oracle SQL:

1. **CREATE TABLE**: Used to create a new table in the database.

```sql
CREATE TABLE table_name (
    column1 datatype [constraint],
    column2 datatype [constraint],
    ...
);
```

Example:
```sql
CREATE TABLE employees (
    employee_id NUMBER PRIMARY KEY,
    first_name VARCHAR2(50),
    last_name VARCHAR2(50),
    hire_date DATE,
    salary NUMBER
);
```

2. **ALTER TABLE**: Used to modify the structure of an existing table.

```sql
ALTER TABLE table_name
    ADD (column_name datatype [constraint],
         ...
    );

ALTER TABLE table_name
    MODIFY (column_name datatype [constraint],
            ...
    );

ALTER TABLE table_name
    DROP COLUMN column_name;
```

3. **DROP TABLE**: Used to remove a table from the database.

```sql
DROP TABLE table_name;
```

4. **CREATE INDEX**: Used to create an index on one or more columns of a table.

```sql
CREATE INDEX index_name
    ON table_name (column1, column2, ...);
```

5. **DROP INDEX**: Used to remove an index from the database.

```sql
DROP INDEX index_name;
```

6. **CREATE VIEW**: Used to create a virtual table based on the result set of a SELECT query.

```sql
CREATE VIEW view_name AS
    SELECT column1, column2, ...
    FROM table_name
    WHERE condition;
```

7. **DROP VIEW**: Used to remove a view from the database.

```sql
DROP VIEW view_name;
```

8. **CREATE SEQUENCE**: Used to create a sequence, which generates unique numeric values.

```sql
CREATE SEQUENCE sequence_name
    START WITH start_value
    INCREMENT BY increment_value
    [MAXVALUE max_value]
    [CYCLE | NOCYCLE];
```

9. **DROP SEQUENCE**: Used to remove a sequence from the database.

```sql
DROP SEQUENCE sequence_name;
```
10. **CREATE USER**: Used to create a new user account in the database.

    ```sql
    CREATE USER username IDENTIFIED BY password;
    ```

11. **DROP USER**: Used to remove a user account from the database.

    ```sql
    DROP USER username [CASCADE];
    ```

12. **GRANT**: Used to grant privileges on database objects to users or roles.

    ```sql
    GRANT privilege(s) ON object TO user_or_role;
    ```

13. **REVOKE**: Used to revoke previously granted privileges from users or roles.

    ```sql
    REVOKE privilege(s) ON object FROM user_or_role;
    ```

14. **CREATE ROLE**: Used to create a new role in the database.

    ```sql
    CREATE ROLE role_name;
    ```

15. **DROP ROLE**: Used to remove a role from the database.

    ```sql
    DROP ROLE role_name;
    ```

16. **ALTER USER**: Used to modify user account properties, such as password and default tablespace.

    ```sql
    ALTER USER username IDENTIFIED BY new_password;
    ```

17. **ALTER ROLE**: Used to modify role properties, such as granting or revoking privileges.

    ```sql
    ALTER ROLE role_name IDENTIFIED BY new_password;
    ```
