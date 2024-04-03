
1. **INSERT**: Adds new rows of data into a table.
   Syntax:
   ```sql
   INSERT INTO table_name (column1, column2, ...)
   VALUES (value1, value2, ...);
   ```

2. **UPDATE**: Modifies existing data in a table.
   Syntax:
   ```sql
   UPDATE table_name
   SET column1 = value1, column2 = value2, ...
   WHERE condition;
   ```

3. **DELETE**: Removes rows of data from a table.
   Syntax:
   ```sql
   DELETE FROM table_name
   WHERE condition;
   ```

4. **MERGE**: Combines INSERT, UPDATE, and DELETE operations based on a specified condition.
   Syntax:
   ```sql
   MERGE INTO target_table
   USING source_table
   ON (join_condition)
   WHEN MATCHED THEN
     UPDATE SET column1 = value1, column2 = value2, ...
   WHEN NOT MATCHED THEN
     INSERT (column1, column2, ...) VALUES (value1, value2, ...);
   ```

5. **SELECT**: Retrieves data from one or more tables.
   Syntax:
   ```sql
   SELECT column1, column2, ...
   FROM table_name
   WHERE condition;
   ```
