## Statements

```
SELECT * FROM table_name; 
```

##TABLES

CREATE TABLE table_name(
id INTEGER, 
name TEXT
); 

--- 

## ADD ROW 

```
INSERT INTO table_name(id ,name)
VALUES (1, 'john');
```

--- 

```
SELECT * FROM table_name; 
SELECT name FROM table_name;  
```

--- 

## EDIT ROW
```
UPDATE table__name
SET col_name = new_val
WHERE id = id_of_row_to_be_edited
```

--- 

## ALTER TABLE
```
ALTER TABLE table_name ADD COLUMN
email TEXT; 
```

--- 

## DELETE ROWS FROM TABLE
```
DELETE FROM table_name
WHERE email IS NULL; 
```
--- 

## CONSTRAINTS: DEFAULT VALS AND PRIMARY KEYS
```
CREATE TABLE customers(
id INTEGER PRIMARY KEY,
name TEXT NOT NULL,
preferred_status TEXT DEFAULT "No"
);

```
---

## COMMON COMMANDS 

```
    CREATE TABLE creates a new table.
    INSERT INTO adds a new row to a table.
    SELECT queries data from a table.
    UPDATE edits a row in a table.
    ALTER TABLE changes an existing table.
    DELETE FROM deletes rows from a table.
```

