## Statements

SELECT * FROM table_name; 

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

```
## ALTER TABLE
ALTER TABLE table__name ADD COLUMN
email TEXT; 
```

--- 

##DELETE ROWS FROM TABLE
```
DELETE FROM table_name
WHERE email IS NULL; 
```




