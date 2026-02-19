SQL-Sales-Analytics-Project
This project simulates a real-world B2B FMCG distribution system operating across multiple states in Nigeria. The goal was to design and query a relational database that tracks sales operations, product distribution, agent performance, customer credit exposure, and payment reconciliation.
📖 Overview

This project demonstrates end-to-end SQL Server data analytics using a structured relational database.

The dataset simulates a commercial sales environment including:

Retailers (Customers)

Agents (Sales Representatives)

Sales Orders

Sales Order Lines

Payments

Credit Limits

All analysis was performed using Microsoft SQL Server (T-SQL).

🎯 Business Objectives

The project answers critical business questions such as:

What is the total Gross Merchandise Value (GMV)?

Which agents generate the highest revenue?

Which retailers have outstanding balances?

What orders were delivered but not paid?

Which customers exceed their credit limits?

🛠 Technical Skills Demonstrated

INNER JOIN / LEFT JOIN

GROUP BY & HAVING

Aggregate Functions (SUM, COUNT, AVG)

Window Functions (RANK, ROW_NUMBER)

NULL handling (IS NULL, COALESCE)

Subqueries & NOT EXISTS

Query Optimization Techniques

Stored Procedures & Variables

🧠 Sample SQL Concepts Used
✔ Revenue Aggregation
SELECT SUM(NetAmount) AS TotalRevenue
FROM SalesOrders
WHERE Status = 'Delivered';

✔ Ranking Top Agents
RANK() OVER (ORDER BY SUM(NetAmount) DESC)

✔ Detecting Unpaid Orders
WHERE PaymentID IS NULL

📈 Key Insights Generated

Identified top-performing sales agents

Detected customers with high outstanding balances

Evaluated credit exposure risks

Measured delivery performance trends

Ranked sales contribution by region

📦 Tools Used

SQL Server (T-SQL)

Relational Data Modeling

Aggregation & Window Functions
