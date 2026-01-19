📂 Dataset

One of the following datasets was used:

Chinook Database (Beginner-friendly SQL database)

Superstore Dataset (CSV imported into SQL)

Retail Sales Dataset

The dataset was imported into a relational database and verified for correctness before analysis.

🛠 Tools Used

Primary Databases:

MySQL (Community Edition)

PostgreSQL

Free Online Alternatives:

SQLite Online

DB Fiddle

GUI Tools:

MySQL Workbench

DBeaver / pgAdmin

📁 Project Files
File Name	Description
queries_task3.sql	SQL script containing all queries written for this task
sales_summary.csv	Exported CSV file with aggregated query results
README.md	Documentation explaining queries and learning outcomes
🔧 SQL Tasks Performed
1️⃣ Database & Table Setup

Created a new database schema.

Designed tables with appropriate data types (INT, VARCHAR, DATE, DECIMAL).

Imported CSV data using database import tools.

2️⃣ Basic Data Exploration

Used SELECT * to explore table structure.

Verified total records using:

SELECT COUNT(*) FROM table_name;


Ensured record count matched the original CSV file.

3️⃣ Filtering & Sorting Queries

Filtered records using WHERE clause:

SELECT * FROM sales
WHERE category = 'Technology';


Sorted results using ORDER BY:

SELECT * FROM sales
ORDER BY sales DESC;

4️⃣ Aggregation & Grouping

Calculated total sales, average profit, and record count:

SELECT category, SUM(sales), AVG(profit), COUNT(*)
FROM sales
GROUP BY category;

5️⃣ HAVING Clause for Group Filters

Filtered aggregated results:

SELECT category, SUM(sales)
FROM sales
GROUP BY category
HAVING SUM(sales) > 100000;

6️⃣ Date Range & Pattern Matching

Used BETWEEN for time-based analysis:

SELECT * FROM sales
WHERE order_date BETWEEN '2023-01-01' AND '2023-01-31';


Used LIKE for pattern search:

SELECT * FROM customers
WHERE customer_name LIKE '%Smith%';

7️⃣ Exporting Results

Exported summary query results to:

sales_summary.csv


Saved all queries in a reusable .sql file.

📈 Key Learning Outcomes

Understood relational database structure.

Gained confidence in writing SELECT, WHERE, ORDER BY, GROUP BY, and HAVING queries.

Learned how to analyze sales data using SQL aggregations.

Practiced exporting SQL results for reporting and documentation.

Followed professional SQL scripting practices.
