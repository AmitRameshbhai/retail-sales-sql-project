# retail-sales-sql-project
SQL project analyzing a retail sales dataset using queries like joins, window functions, CASE statements, and aggregations.
# 🛒 Retail Sales Analysis using SQL

This SQL-based project dives into transactional retail data to uncover key business insights related to customer behavior, sales trends, and product category performance. The dataset was imported from a CSV and analyzed using SQL queries on a MySQL database.

---

## 📂 Dataset Schema

A single table `retail_sales` was created with the following fields:

- `transaction_id` (INT, Primary Key)
- `sale_date` (DATE)
- `sale_time` (TIME)
- `customer_id` (INT)
- `gender` (VARCHAR)
- `age` (INT)
- `category` (VARCHAR)
- `quantity` (INT)
- `price_per_unit` (FLOAT)
- `cogs` (FLOAT)
- `total_sale` (FLOAT)

---

## 🎯 Project Objectives

- Analyze total sales and unique customers.
- Filter transactions based on date and product category.
- Aggregate sales performance per category and customer.
- Identify high-value transactions and peak months.
- Segment time-of-day performance (Morning/Afternoon/Evening).

---

## 🛠️ Technologies Used

- SQL (MySQL)
- DDL & DML operations
- Aggregate Functions (SUM, AVG, COUNT)
- Conditional Queries (`CASE WHEN`)
- Grouping and Sorting
- Subqueries and CTEs
- Window Functions (`RANK()`)

---

## 🔍 Questions Solved (10 SQL Queries)

1. **Sales on a Specific Date**  
   Retrieve all transactions from `'2022-11-05'`.

2. **High Quantity Clothing Sales in Nov-2022**  
   Filter for category `'Clothing'` with quantity > 4.

3. **Total Sales per Category**  
   Aggregated total sales and order count per category.

4. **Average Age for 'Beauty' Shoppers**  
   Find mean age of customers who bought `'Beauty'` items.

5. **High-Value Sales**  
   Transactions where `total_sale > 1000`.

6. **Gender-wise Sales per Category**  
   Transaction counts segmented by gender and product category.

7. **Top Sales Month Each Year**  
   Use of `RANK()` and window functions to detect best-selling month.

8. **Top 5 Customers by Revenue**  
   Highest spending customers based on total sales.

9. **Unique Customers per Category**  
   Distinct customer count per product category.

10. **Shift-Based Orders**  
   Time segmentation into Morning (<12), Afternoon (12–17), Evening (>17) using `CASE`.

---
