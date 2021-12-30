---
Title: 'Procedures'
Description: 'Procedures are blocks of SQL code that are saved in a database and can be executed repeatedly on demand.'
Subjects:
  - 'Data Science'
Tags:
  - 'Database'
  - 'MySQL'
CatalogContent:
  - 'learn-sql'
  - 'paths/analyze-data-with-sql'
---

Procedures (also stored procedures) are blocks of SQL code that are saved in a database and can be executed repeatedly on demand. Procedures can be defined to take parameters that can be used within the body of the procedure, as well as define parameters that return an output value.

The syntax for creating a procedure varies depending upon the type of database management system (DBMS) being used. Below is an example procedure defined and executed with [MySQL](https://www.mysql.com/); it accepts two parameters and returns an output value.

## MySQL Example

```sql
# Set the default delimiter so the procedure can include semicolons
DELIMITER //
# Create the procedure
CREATE PROCEDURE add_int (IN x INT, IN y INT, OUT z INT)
BEGIN
  SELECT x + y INTO z;
END //

# Set the delimiter back to the default
DELIMITER ;
# Execute the stored procedure
CALL add_int (5, 3, @z);
# Return the output parameter
SELECT @z AS Result;
```

Output:

| Result |
| ------ |
| 8      |
