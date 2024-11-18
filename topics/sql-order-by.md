# SQL ORDER BY

### The SQL ORDER BY

The `ORDER BY` keyword is used to sort the result-set in ascending or descending order.

**Example**

Sort the products by price:

```sql
SELECT * FROM Products
ORDER BY Price;
```

### Syntax

```sql
SELECT column1, column2,
FROM table_name
ORDER BY column1, column2, ASC|DESC;
```

### DESC

The `ORDER BY` keyword sorts the records in ascending order by default. To sort the records in descending order, use the `DESC` keyword.

**Example**

Sort the products from highest to lowest price:

```sql
SELECT * FROM Products
ORDER BY Price DESC;
```

### Order Alphabetically

For string values the `ORDER BY` keyword will order alphabetically:

**Example:**

Sort the products alphabetically by ProductName:

```sql
SELECT * FROM Products
ORDER BY ProductName;
```

### Alphabetically DESC

To sort the table reverse alphabetically, use the `DESC` keyword:

**Example:**

Sort the products by ProductName in reverse order:

```sql
SELECT * FROM Products
ORDER BY ProductName DESC;
```

### ORDER BY Several Columns

The following SQL statement selects all customers from the "Customers" table, sorted by the "Country" and the "CustomerName" column. This means that it orders by Country, but if some rows have the same Country, it orders them by CustomerName:

**Example:**

```sql
SELECT * FROM Customers
ORDER BY Country, CustomerName;
```

### Using Both ASC and DESC

The following SQL statement selects all customers from the "Customers" table, sorted ascending by the "Country" and descending by the "CustomerName" column:

```sql
SELECT * FROM Customers
ORDER BY Country ASC, CustomerName DESC;
```
