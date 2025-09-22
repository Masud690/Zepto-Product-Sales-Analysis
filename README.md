1# Zepto-Product-Sales-Analysis
2 🗄 Dataset Description

Briefly describe important fields:

name → product name

mrp → maximum retail price

discountPercent → % discount offered

discountedSellingPrice → final price after discount

availableQuantity → stock available

outOfStock → stock status

weightInGms → product weight in grams

category → product category

3. 🔍 Key Business Questions & SQL Queries

Q1: Top 10 best-value products by discount %

Q2: High-MRP but out-of-stock products

Q3: Estimated revenue by category

Q4: High MRP, low discount products

Q5: Top 5 categories by average discount %

Q6: Price per gram ranking

Q7: Product weight categorization (CASE statement)

Q8: Total inventory weight by category

You can show code snippets like:

-- Q3: Estimated revenue for each category
select category, 
       sum(discountedSellingPrice * availableQuantity) as revenue
from zepto
group by category
order by revenue desc;

4. 📊 Insights & Findings

Categories like X and Y bring the most estimated revenue.

Some high-MRP products (>₹300) are out of stock, indicating supply-chain issues.

Bulk products (>5000g) form a small percentage of inventory but carry heavy weight in stock volume.

5. ⚙️ Tools & Skills Demonstrated

SQL: filtering, joins (if added), CASE statements, aggregations, GROUP BY, ORDER BY.

Business Analytics: inventory management, pricing strategy, discount optimization.

Data Cleaning & Loading: CSV → SQL table.

6. 🚀 How to Run

Load zepto_v1.csv into MySQL/PostgreSQL/SQLite.

Run queries from /sql folder.

7. 🏆 What I Learned

Writing optimized SQL queries for real-world datasets.

Translating business questions into analytical queries.

Building a complete mini-project workflow (data → queries → insights).
