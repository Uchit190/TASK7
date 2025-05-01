# Task 7: Basic Sales Summary using SQLite and Python

## Objective
Use SQL inside Python (with SQLite) to get a basic sales summary and visualize it.

## Tools Used
- Python (Jupyter Notebook)
- SQLite (`sqlite3` module)
- pandas
- matplotlib

## What I Did
1. Created a SQLite database (`sales_data.db`)
2. Created a `sales` table and inserted sample data
3. Wrote SQL query to calculate:
   - Total quantity sold per product
   - Total revenue per product
4. Loaded SQL query results into a pandas DataFrame
5. Displayed the summary using a bar chart

## SQL Query Used
```sql
SELECT 
    product, 
    SUM(quantity) AS total_qty, 
    SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY produc
