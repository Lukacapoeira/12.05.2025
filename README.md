📊 SQL Challenge – Top Categories by Revenue
This SQL query analyzes product sales and returns the top 2 categories within each product group, based on total revenue.

🔍 Problem Statement
For each product_group, identify the two category values that generate the highest revenue.
Revenue is calculated as: item_quantity × product_price.

⚙️ Data Tables Used:
products – contains product details and prices

order_positions – includes sold quantities per product

product_groups – maps product IDs to categories and groups

🧠 Logic Overview:
Join products, order_positions, and product_groups.

Calculate total revenue per category and price point (to account for products sold at multiple prices).

Use ROW_NUMBER() to rank categories by revenue within each group.

Filter to return only the top 2 for each product_group.

📌 SQL Features Used:
JOIN

GROUP BY

SUM()

ROW_NUMBER() OVER (PARTITION BY … ORDER BY …)

Common Table Expressions (WITH)

💡 Sample use cases:
Business dashboards: top-performing categories per department

Inventory planning and strategic pricing

Marketing prioritization based on sales revenue
