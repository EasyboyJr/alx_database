# SQL More Queries

SQL (Structured Query Language) is a powerful tool for managing and manipulating data in relational databases. Beyond the basics, there are advanced SQL queries that allow you to perform complex operations and gain deeper insights from your data.

## Advanced Query Types:

1. **Aggregation:
Use functions like `SUM`, `AVG`, `COUNT`, and `GROUP BY` to perform calculations on data and summarize results.

2. **Subqueries**:
Embed queries within other queries to retrieve data based on conditions or perform calculations using subquery results.

3. **Joins**:
Combine data from multiple tables using `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, and `FULL OUTER JOIN` operations.

4. **Window Functions**:
Analytical functions like `ROW_NUMBER`, `RANK`, and `LEAD` allow you to analyze data within a specific window or partition.

5. **UNION and UNION ALL**:
Combine the results of multiple `SELECT` queries, either eliminating duplicates (`UNION`) or including them (`UNION ALL`).

## Examples:

1. **Aggregation**:
```
SELECT department, AVG(salary) AS avg_salary
FROM employees
GROUP BY department;
```

2. **Subqueries**:
```
SELECT product_name, price
FROM products
WHERE price > (SELECT AVG(price) FROM products);

```

3. **Joins**:
```
SELECT orders.order_id, customers.customer_name
FROM orders
INNER JOIN customers ON orders.customer_id = customers.customer_id;
```

SQL's advanced query capabilities allow you to dive deeper into data analysis, generate insightful reports, and extract meaningful information from your relational databases. Learning these advanced techniques empowers you to handle complex scenarios and make informed decisions based on your data.