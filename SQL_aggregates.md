## COUNT()

```
SELECT COUNT(*)
  FROM table_name; 

SELECT COUNT(*)
  FROM movies
  WHERE ratings < 2; 
```

--- 

## SUM()
```
SELECT SUM(col_name)
  FROM table_name; 
```

--- 

## MAX() MIN()
```
SELECT MAX(downloads)
  FROM table_name; 


SELEC MIN(sales)
  FROM store_name; 
```

--- 

## AVG()
```
SELECT AVG(rating) FROM movies; 
```

--- 

## ROUND()
```
SELECT name, AVG(rating) FROM restaurants; 

SELECT name, ROUND(AVG(price), 2) FROM table_name; 
```

--- 

## GROUP BY
```
SELECT year, AVG(rating)
FROM movies
GROUP BY year
ORDER BY year;
```

--- 

## HAVING
```
SELECT price, 
   ROUND(AVG(downloads)),
   COUNT(*)
FROM fake_apps
GROUP BY price
             HAVING COUNT(price) > 10;
```

--- 

## AGGREGATE FUNCS 
```

    GROUP BY is a clause used with aggregate functions to combine data from one or more columns.
    HAVING limit the results of a query based on an aggregate property.
```
