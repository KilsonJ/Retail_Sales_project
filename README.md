# 📊 Retail Sales & Inventory Analysis (Excel Project)
🔎 Overview

This project demonstrates how I cleaned, analyzed, and visualized a messy retail sales dataset using Excel only (no SQL or Python).
It simulates a real business scenario where a retailer wants to understand their sales performance, top products, and customer behavior.

The dataset was  messy (~5,000 rows) to showcase data wrangling, formulas, PivotTables, and dashboards.

🗂 Dataset

Raw Dataset (CSV/Excel): messy dates, misspellings, inconsistent formats, duplicates, and missing values.

Cleaned Dataset (Excel): structured, standardized, and ready for analysis.

Dashboard File (Excel): interactive with PivotTables, slicers, and charts.

Columns Included:

Order Date (mixed formats: 12/01/25, Jan-12-2025, etc.)

Product Name (duplicates like “Nike P6000”, “Nike P-6000”)

Category (e.g., Clothng vs Clothing)

Quantity (numbers + text like "two")

Unit Price (£25, “25.00”, “£25”)

Total (sometimes incorrect)

Payment Method (missing or inconsistent)

Store Location (e.g., Lonodn vs London)

Customer Type (New vs Returning, with blanks)

🧹 Data Cleaning (Excel + Power Query)

Steps taken:

Dates → standardized all formats into a clean Date field.

Text Fields → trimmed, cleaned, and capitalized product/category/store names.

Typos → fixed common misspellings (Clothng → Clothing, Lonodn → London).

Quantity → converted text (“two”, “three”) into numbers.

Unit Price → removed “£” and converted to numeric format.

Total → recalculated Quantity × Unit Price and flagged mismatches.

Missing Values → filled blanks in Payment Method & Customer Type.

Duplicates → removed duplicate transactions.

📈 Analysis (Excel Formulas + PivotTables)

I built PivotTables and used formulas to answer key business questions:

Total Revenue per Category / Store

Top 10 Best-Selling Products

% of Customers: New vs Returning

Store with Highest Sales

Monthly Sales Trends

Popular Payment Method

Average Basket Size (units per order)

Average Order Value (AOV)

Example Formulas:

Total Revenue:
=SUM(G:G)

Average Order Value (AOV):
=SUM(G:G)/COUNTA(G:G)

Revenue by Category (e.g., Clothing):
=SUMIFS(G:G,C:C,"Clothing")

% Returning Customers:
=SUMIFS(G:G,I:I,"Returning")/SUM(G:G)

XLOOKUP (Unit Price of Product):
=XLOOKUP("Nike Tech Fleece",C:C,F:F,"Not Found")

📊 Dashboard

An interactive Excel Dashboard was built including:

KPI Cards: Total Revenue, AOV, Basket Size, Returning Customer %

Line Chart: Monthly Sales Trend

Bar Charts: Revenue by Category, Top 10 Products, Store Location Sales

Donut Chart: New vs Returning Customers

Slicers: by Month, Store, Category

(Insert screenshots of dashboard here)

💡 Key Insights

Clothing generated the highest revenue, but Footwear had the fastest growth trend.

London store consistently outperformed Birmingham & Manchester.

Returning customers contributed ~65% of total revenue.

PayPal was the fastest-growing payment method.

Average basket size: 2.3 units/order.

Average order value (AOV): £42.

🛠 Tools Used

Microsoft Excel

Power Query (for cleaning)

PivotTables & Charts

Slicers & Dashboards

Formulas: SUMIFS, COUNTIFS, XLOOKUP, IF, AVERAGEIFS

📂 Deliverables

Raw Dataset (Retail_Sales_Raw.csv)

Cleaned Dataset (Retail_Sales_Clean.xlsx)

Dashboard File (Retail_Sales_Dashboard.xlsx)

README (this file)

🚀 Why This Project?

This project showcases the end-to-end Excel workflow every analyst must master:

Taking messy raw data

Cleaning & transforming it into a usable dataset

Analyzing with formulas & PivotTables

Communicating insights via a clear dashboard

It’s designed to replicate real-world analyst tasks and prove practical Excel skills for junior/entry-level data roles.
