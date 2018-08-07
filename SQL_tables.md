## JOIN

```
SELECT * FROM table_1
JOIN table_2 
ON table_1.column = table_2.column; 


SELECT table_1.column_name, table_2.column_name FROM table_1
JOIN table_2 
ON table_1.column = table_2.column; 


SELECT * FROM orders
JOIN subscriptions
ON orders.subscription_id = subscriptions.subscription_id
WHERE subscriptions.description = "RAZORS"
```

--- 

## LEFT JOIN
```
SELECT * FROM newspaper
LEFT JOIN online
ON newspaper.id = online.id; 
```

--- 

## PRIMARY KEY & FOREIGN KEYS INNER JOIN
```
SELECT * FROM classes
JOIN students
ONE classes.id = students.class_id;
```

--- 

## CROSS JOIN
```

SELECT month, 
  COUNT(*)
FROM newspaper
CROSS JOIN months
WHERE start_month <= month 
  AND end_month >= month
GROUP BY month;
```

--- 

## CROSS JOIN
```
SELECT * FROM table1
UNION 
SELECT * FROM table2; 
```

---

## WITH 

```
WITH previous_query AS (
    SELECT customer_id,
       COUNT(subscription_id) AS 'subscriptions'
       FROM orders
       GROUP BY customer_id

    )

SELECT customers.customer_name, previous_query.subscriptions FROM 
previous_query JOIN customers
ON previous_query.customer_id = customers.customer_id; 
```

---

## REVIEW
```


    JOIN will combine rows from different tables if the join condition is true.

    LEFT JOIN will return every row in the left table, and if the join condition is not met, NULL values are used to fill in the columns from the right table.

    Primary key is a column that serves a unique identifier for the rows in the table.

    Foreign key is a column that contains the primary key to another table.

    CROSS JOIN lets us combine all rows of one table with all rows of another table.

    UNION stacks one dataset on top of another.

    WITH allows us to define one or more temporary tables that can be used in the final query.

```
