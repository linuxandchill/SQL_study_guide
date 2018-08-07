## MAKING QUERIES

```
SELECT col_name AS "column alias"
FROM table_name; 
```

--- 

## RETURNING UNIQUES/ FILTERING
```
SELECT tools FROM inventory;

vs

SELECT DISTINC tools FROM inventory; 

SELECT * FROM movies
WHERE ratings >= 4; 
```

--- 
## LIKE & WILDCARD OPERATORS
```
SELECT * FROM movies
WHERE title LIKE "Ho_se"; 

SELECT * FROM movies
WHERE title LIKE "A%"
```
