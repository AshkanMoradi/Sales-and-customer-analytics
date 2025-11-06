✅ Project Overview:
This project analyzes sales, customer, and product data to derive key business metrics and perform data quality checks.

✅ Files Provided:

Ashkan Moradi - Python Version.ipynb – Python notebook <br />
Ashkan Moradi - SQL Version.sql – SQL script with all queries <br />
README.md – This document

✅ How to Run:

Load the CSV files into your Python environment (or SQL environment) as tables (orders, order_items, products).
Use your database’s import tool or COPY/LOAD DATA command (in case of using in a SQL environment)
Run the script.
Review results for each section.

✅ Assumptions:

Each order_id in orders is unique. <br />
Each order can contain multiple items in order_items. <br />
Product details in the products table (like 'Category' and 'unit_cost') are correct. <br />
the 'total_amount' in orders equals the sum of (quantity * unit_price) from order_items for that order. <br />
All monetary values are stored in the same currency (No need for converting) <br />
Dates are stored in YYYY-MM-DD format. <br />
No taxes are considered unless included in unit_price or total_amount. <br />

✅ Outputs Summary:

Sales Metrics
Total revenue, total cost, and gross margin percentage by product category. <br />
Customer Metrics <br />
Top 2 customers by spending and average order value per customer. <br />
Data Quality Checks <br />
Identify missing references, data type mismatch, or missing values (Null) and duplicate values. <br />
Frequently Purchased Product Pairs. <br />
Top 3 combinations of products are often bought together in the same order. <br />

✅ Data Quality Handling Approach:

Missing Foreign Keys: Enforce referential integrity constraints. <br />
Mismatched Totals: Recalculate from order_items before loading to production. <br />
Missing Values: Flag and filter out invalid records during preprocessing. <br />
Duplicate Rows: check based on unique keys (order_id, product_id). <br />

📫 If you have any questions, don't hesitate to contact me on [**LinkedIn**](https://www.linkedin.com/in/ashkan-moradi-33936278/)
Project Overview:
