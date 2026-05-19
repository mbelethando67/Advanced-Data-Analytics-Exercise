Coffee Sales SQL Window Functions & Wildcards Exercise
Overview
This project demonstrates the use of advanced SQL concepts using the coffee_sales dataset.
The exercises focus on:


Wildcards with LIKE and RLIKE


Window Functions


Ranking Functions


Running Totals


Revenue Analysis


Partitioning Data


Lead & Lag Analysis


Quartile Segmentation


The goal of the exercise was to strengthen analytical SQL skills used in real-world business analytics and data analysis.

Dataset Used
Table: coffee_sales
Main columns used:


transaction_id


store_location


product_category


product_detail


transaction_qty


unit_price


transaction_date


transaction_time



SQL Concepts Practiced
1. LIKE & Wildcards
Used:


% → matches multiple characters


_ → matches exactly one character


Examples:
LIKE '%Lg'LIKE '% __'

2. RLIKE (Regular Expressions)
Used regex patterns to filter text containing numbers or specific patterns.
Example:
RLIKE '[0-9]'

3. Window Functions
Used OVER() with:


PARTITION BY


ORDER BY


Functions practiced:


SUM()


AVG()


ROW_NUMBER()


RANK()


DENSE_RANK()


NTILE()


LAG()


LEAD()


FIRST_VALUE()



Key Exercises Completed
Store Revenue Analysis
Calculated:


Total revenue per store


Percentage contribution of each transaction


Running totals


Example:
SUM(transaction_qty * unit_price)OVER(PARTITION BY store_location)

Ranking Transactions
Ranked transactions within each store by revenue.
Functions compared:


ROW_NUMBER()


RANK()


DENSE_RANK()



Quartile Segmentation
Used NTILE(4) to divide transactions into revenue quartiles.

Previous & Next Transaction Analysis
Used:


LAG() to compare with previous transactions


LEAD() to compare with upcoming transactions



Cheapest Product Per Category
Used FIRST_VALUE() to identify the cheapest product within each category.

Combined Wildcards + Window Functions
Filtered only:


Lg


Rg


products using LIKE, then:


ranked transactions


calculated store average revenue



Skills Demonstrated


SQL filtering


Text pattern matching


Revenue calculations


Business analytics logic


Window function analysis


Ranking and segmentation


Data partitioning


Running totals and trend analysis



Tools Used


Databricks SQL


SQL Window Functions


GitHub



Learning Outcome
This exercise improved understanding of:


analytical SQL


business reporting


advanced query writing


real-world sales analysis techniques


It also strengthened confidence in using SQL for data analytics and reporting tasks.
