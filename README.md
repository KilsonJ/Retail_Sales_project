📊 Retail Sales & Inventory Analysis (Excel Project)
🔎 Project Objective

This project simulates a real-world retail analytics scenario using Excel only (no SQL or Python).
The goal: clean, analyze, and visualize a messy 5,000-row retail dataset to uncover insights about sales performance, top products, store trends, and customer behavior.

📂 Dataset Overview
Dataset	Description
Raw Data (Retail_Sales_Raw.csv).xlsx
	Contains messy values (dates, currency symbols, typos, duplicates, missing fields).
Clean Data (Retail_Sales_Raw.csv).xlsx
	Fully standardized and formatted for analysis.
Dashboard (Retail_Sales_Dashboard.xlsx)	(Coming soon — interactive Excel dashboard using PivotTables, charts, and slicers.)
🧹 Data Cleaning (Excel + Power Query)

Cleaning Steps:

Standardized inconsistent date formats.

Trimmed, corrected, and capitalized all text fields (Product, Category, Store).

Fixed common typos (Clothng → Clothing, Lonodn → London).

Converted Quantity text values ("two", "three") into numbers.

Removed currency symbols (£) and formatted Unit Price as numeric.

Recalculated totals (Total = Quantity × Unit Price).

Filled missing values in Payment Method and Customer Type.

Removed duplicate rows to ensure data integrity.

📈 Analysis (Excel Formulas + PivotTables)

Business Questions Answered:

Question	Excel Feature Used
What is total revenue per category and store?	SUMIFS, PivotTables
Which are the top 10 best-selling products?	PivotTable + RANK
What % of customers are returning vs new?	COUNTIFS, PivotChart
Which store generated the highest sales?	PivotTables
What are the monthly sales trends?	Line chart using MONTH()
What is the Average Order Value (AOV)?	SUM(Total)/COUNTA(OrderID)
What is the Average Basket Size (Units/Order)?	AVERAGE(Quantity)

Example Formulas:

=SUMIFS(G:G, C:C, "Clothing") → Revenue by Category

=XLOOKUP("Nike Tech Fleece", C:C, F:F, "Not Found") → Product Price Lookup

=SUMIFS(G:G, I:I, "Returning")/SUM(G:G) → % Returning Customers

📊 Dashboard (Coming Soon)

An interactive Excel dashboard will summarize all KPIs and insights visually.

Planned Features:

KPI Cards: Total Revenue, AOV, Basket Size, Returning Customer %

Line Chart: Monthly Sales Trend

Bar Charts: Top 10 Products, Revenue by Category

Column Chart: Store Location Performance

Donut Chart: New vs Returning Customers

Slicers: Filter by Month, Store, and Category

(Once uploaded, the dashboard file link will be added here.)

💡 Key Insights (From Cleaned Data)

Clothing generated the highest revenue overall.

Footwear showed the fastest month-over-month growth trend.

Returning customers contributed approximately 65% of total revenue.

London store consistently outperformed Birmingham & Manchester.

Average Basket Size: 2.3 units per order.

Average Order Value (AOV): £42.

🖼 Dashboard Screenshots

Here are sample visuals from the dashboard and pivot analysis:




(Add more screenshots as you finalize your visuals.)

🛠 Tools & Skills Demonstrated

Microsoft Excel

Power Query (data cleaning & transformations)

PivotTables & PivotCharts

Slicers & interactive dashboards

Core formulas: SUMIFS, COUNTIFS, AVERAGEIFS, IF, XLOOKUP

Data Cleaning

KPI Development & Visualization

Business Insight Communication

🚀 Outcome

This project replicates the real workflow of a junior/entry-level data analyst, proving:

Ability to clean and transform messy datasets.

Proficiency in analyzing and visualizing business data in Excel.

Skill in communicating insights clearly through dashboards and storytelling.

🔗 Future Improvements

Upload and link the Retail_Sales_Dashboard.xlsx file.

Add scenario analysis (e.g., 5% price increase impact on revenue).

Introduce rolling averages to smooth monthly trends.

Add profit margin analysis (once cost data is included).

🧠 Learning Reflection

This project helped strengthen my understanding of:

Excel’s end-to-end data workflow (from messy data → insights)

Business-oriented storytelling through dashboards

Power Query & advanced lookup/aggregation logic

Author: Kilson Joaquim

📍 London, UK
🎯 Aspiring Data Analyst focusing on Excel, SQL, and Tableau.

#️⃣ Tags
#Excel #DataAnalytics #Dashboard #PowerQuery #PortfolioProject #DataCleaning #KPI #Visualization

✅ Instructions

Paste this into your GitHub README.md

It will render perfectly — no formatting cutoff

When you upload your dashboard Excel file later, just replace the placeholder link above
