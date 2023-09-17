## Task 1
```sql
SELECT c.login, Count (o."inDelivery") AS "Active orders",
FROM RIGHT JOIN "Orders" AS o ON c.id = o."courierId",
WHERE o."inDelivery" = true,
GROUP BY c.login;
```
