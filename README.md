# 📊 Retail Sales & Inventory Analysis (Excel Project)

## 🔎 Project Objective
This project simulates a real-world retail analytics scenario using **Excel only** (no SQL or Python).  
The goal: clean, analyze, and visualize a messy **5,000-row retail dataset** to uncover insights about **sales performance, top products, store trends, and customer behavior.**

---

## 📂 Dataset Overview

| Dataset | Description |
|----------|--------------|
| [**Raw Data (Retail_Sales_Raw.csv).xlsx**](https://github.com/KilsonJ/Retail_Sales_project/blob/main/Raw%20Data%20(Retail_Sales_Raw.csv).xlsx) | Contains messy values (dates, currency symbols, typos, duplicates, missing fields). |
| [**Clean Data (Retail_Sales_Raw.csv).xlsx**](https://github.com/KilsonJ/Retail_Sales_project/blob/main/Clean%20Data%20(Retail_Sales_Raw.csv).xlsx) | Fully standardized and formatted for analysis. |
| **Dashboard (Retail_Sales_Dashboard.xlsx)** | *(Coming soon — interactive Excel dashboard using PivotTables, charts, and slicers.)* |

---

## 🧹 Data Cleaning (Excel + Power Query)

**Cleaning Steps:**
1. Standardized inconsistent **date formats**.  
2. Trimmed, corrected, and capitalized all **text fields** (Product, Category, Store).  
3. Fixed common typos (Clothng → Clothing, Lonodn → London).  
4. Converted **Quantity** text values ("two", "three") into numbers.  
5. Removed currency symbols (£) and formatted **Unit Price** as numeric.  
6. Recalculated totals (Total = Quantity × Unit Price).  
7. Filled missing values in **Payment Method** and **Customer Type**.  
8. Removed **duplicate rows** to ensure data integrity.  

---

## 📈 Analysis (Excel Formulas + PivotTables)

**Business Questions Answered:**

| Question | Excel Feature Used |
|-----------|--------------------|
| What is total revenue per category and store? | SUMIFS, PivotTables |
| Which are the top 10 best-selling products? | PivotTable + RANK |
| What % of customers are returning vs new? | COUNTIFS, PivotChart |
| Which store generated the highest sales? | PivotTables |
| What are the monthly sales trends? | Line chart using MONTH() |
| What is the Average Order Value (AOV)? | SUM(Total)/COUNTA(OrderID) |
| What is the Average Basket Size (Units/Order)? | AVERAGE(Quantity) |

**Example Formulas:**
- `=SUMIFS(G:G, C:C, "Clothing")` → Revenue by Category  
- `=XLOOKUP("Nike Tech Fleece", C:C, F:F, "Not Found")` → Product Price Lookup  
- `=SUMIFS(G:G, I:I, "Returning")/SUM(G:G)` → % Returning Customers  

---

## 📊 Dashboard (Coming Soon)

An **interactive Excel dashboard** will summarize all KPIs and insights visually.

### Planned Features:
- **KPI Cards:** Total Revenue, AOV, Basket Size, Returning Customer %  
- **Line Chart:** Monthly Sales Trend  
- **Bar Charts:** Top 10 Products, Revenue by Category  
- **Column Chart:** Store Location Performance  
- **Donut Chart:** New vs Returning Customers  
- **Slicers:** Filter by Month, Store
