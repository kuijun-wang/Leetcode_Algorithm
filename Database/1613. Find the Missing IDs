WITH RECURSIVE seq AS (
    SELECT 1 AS value UNION ALL SELECT value + 1 FROM seq WHERE value < (select max(customer_id)from customers)
    )

SELECT value ids FROM seq
where value not in (select customer_id from customers)
order by value
