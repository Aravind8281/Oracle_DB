1. **COMMIT**: Used to save changes made in the current transaction to the database.

   ```sql
   COMMIT;
   ```

2. **ROLLBACK**: Used to discard changes made in the current transaction and restore the database to the state before the transaction began.

   ```sql
   ROLLBACK;
   ```

3. **SAVEPOINT**: Used to set a named point within a transaction to which you can later roll back.

   ```sql
   SAVEPOINT savepoint_name;
   ```

4. **ROLLBACK TO SAVEPOINT**: Used to roll back the transaction to a specific savepoint.

   ```sql
   ROLLBACK TO SAVEPOINT savepoint_name;
   ```

5. **RELEASE SAVEPOINT**: Used to remove a savepoint from the current transaction.

   ```sql
   RELEASE SAVEPOINT savepoint_name;
   ```
