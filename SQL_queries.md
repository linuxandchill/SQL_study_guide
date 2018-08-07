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
WHERE title LIKE "A%";
```
--- 

## IS & IS NOT CONDITIONALS
```
SELECT col_name
FROM table_name
WHERE other_col IS NOT NULL;
```

--- 

## BETWEEN
```
SELECT * FROM movies
WHERE name BETWEEN 'A' and 'T'; 

SELECT * FROM movies
WHERE name BETWEEN 1950 and 1959; 

SELECT * FROM employees
WHERE productivity BETWEEN 4 and 5 
  AND age BETWEEN 20 and 30 ; 

SELECT * FROM restaurants
WHERE ratings = 5 AND cuisine_type = 'Indian'; 
```

--- 

## OR
```
SELECT * FROM table_name
WHERE year > 2014 
OR rating > 5;
```

--- 

## SORTING

```
SELECT name,
FROM employes
ORDER BY age;

SELECT name, year
FROM movies
ORDER BY experience DESC;
```

---

## LIMIT 

```
SELECT * 
FROM employees
LIMIT 100; 

SELECT * FROM movies
ORDER BY rating DESC
LIMIT 5; 
```

--- 

## CASE

```
SELECT name,
       CASE 
       WHEN genre = 'comedy' THEN 'Funny'

       ELSE 'Not funny'

       END AS 'Funny-ness level'
  FROM movies; 
```

--- 

## SUMMARY

```

    SELECT is the clause we use every time we want to query information from a database.
    AS renames a column or table.
    DISTINCT return unique values.
    WHERE is a popular command that lets you filter the results of the query based on conditions that you specify.
    LIKE and BETWEEN are special operators.
    AND and OR combines multiple conditions.
    ORDER BY sorts the result.
    LIMIT specifies the maximum number of rows that the query will return.
    CASE creates different outputs.

```
