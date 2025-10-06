# 📊 Retail Sales & Inventory Analysis (Excel Project)

### 🧩 Project Objective
This project simulates a real-world retail analytics scenario using **Excel only** (no SQL or Python).  
The goal: clean, analyze, and visualize a messy 5,000-row sales dataset to uncover insights about sales performance, top products, store trends, and customer behavior.

---

## 📂 Dataset Overview
| Dataset | Description |
|----------|--------------|
| [**Raw Data (Retail_Sales_Raw.csv)**](https://github.com/KilsonJ/Retail_Sales_project/blob/main/Raw%20Data%20(Retail_Sales_Raw.csv)) | Contains messy values (dates, currency symbols, typos, duplicates, missing fields). |
| [**Cleaned Data (Retail_Sales_Clean.xlsx)**](https://github.com/KilsonJ/Retail_Sales_project/blob/main/Clean%20Data%20(Retail_Sales_Clean.xlsx)) | Fully standardized and formatted for analysis. |
| [**Dashboard (Retail_Sales_Dashboard.xlsx)**](https://github.com/KilsonJ/Retail_Sales_project/blob/main/Dashboard%20(Retail_Sales_Dashboard.xlsx)) | Interactive Excel dashboard using PivotTables, charts, and slicers. |

### 🧾 Sample Data Preview

| Order Date | Product Name  | Unit Price | Quantity | Store    | Customer Type |
|-------------|----------------|-------------|-----------|-----------|----------------|
| "12/01/25" | "Nike P-6000" | "£25" | "two" | "Lonodn" | "" |
| 2025-01-12 | "Nike P6000" | 25.00 | 2 | "London" | "Returning" |

---

## 🔄 Methodology & Workflow

### 1️⃣ Data Cleaning (Excel + Power Query)
- **Standardized Dates** → unified mixed formats (`12/01/25`, `Jan-12-2025`, etc.).
- **Fixed Text Fields** → trimmed, capitalized, corrected typos (`Lonodn → London`, `Clothng → Clothing`).
- **Converted Values** → changed text numbers (“two”) into numeric values.
- **Removed Duplicates** → eliminated duplicate orders.
- **Recalculated Totals** → ensured `Total = Quantity × Unit Price`.
- **Handled Missing Values** → filled blanks in Payment Method & Customer Type.

### 2️⃣ Analysis (Formulas + PivotTables)
Used Excel formulas and pivot logic to calculate key KPIs:

| Business Question | Excel Technique Used |
|--------------------|----------------------|
| Total Revenue by Category / Store | `SUMIFS()` |
| Top 10 Best-Selling Products | PivotTable Sorting |
| New vs Returning Customers % | `COUNTIFS()` + Pivot Charts |
| Monthly Sales Trends | Pivot Line Chart |
| Store with Highest Sales | `MAX()` + Filters |
| Average Basket Size | `=SUM(Qty)/COUNT(Orders)` |
| Average Order Value (AOV) | `=SUM(Total)/COUNT(Orders)` |
| Lookup Product Price | `=XLOOKUP("Nike Tech Fleece",C:C,F:F)` |

---

## 📊 Dashboard Highlights
The Excel dashboard brings the data to life through interactive visuals:

- **KPI Cards:** Total Revenue, Average Order Value (£42), Basket Size (2.3 units), Returning Customer % (~65%)
- **Line Chart:** Monthly Sales Trend
- **Bar Chart:** Revenue by Category / Store
- **Donut Chart:** New vs Returning Customers
- **Slicers:** Month | Category | Store | Payment Method

> *(Screenshots can be added here for visual preview.)*

---

## 💡 Key Insights
- **Footwear** category generated the highest overall revenue.  
- **Footwear** showed the fastest growth trend month-on-month.  
- **Returning customers** drove ~33% of total revenue.  
- **Manchester store** consistently outperformed Birmingham and Manchester.  
- **PayPal** emerged as the fastest-growing payment method.  
- **Average basket size:** 2.3 units/order | **Average order value:** £313.

---

## 🛠 Tools & Techniques
- **Microsoft Excel**
  - Power Query (data cleaning & transformation)
  - PivotTables & Charts
  - Slicers & Dashboards
  - Formulas: `SUMIFS`, `COUNTIFS`, `IF`, `AVERAGEIFS`, `XLOOKUP`
- **Data Storytelling:** converting findings into business insights.

---

## 🚀 How to Explore This Project
1. Download or clone this repository.
2. Open **Retail_Sales_Dashboard.xlsx**.
3. Use slicers (Month, Store, Category) to explore sales patterns.
4. Review pivot tables to see the underlying calculations.
5. Compare findings with insights above.

---

## 🔮 Future Enhancements
- Add **“What-If” Analysis** (impact of price or discount changes).
- Introduce **Rolling 3-Month Sales Trend** for seasonality tracking.
- Build **forecasting model** with Excel trendlines or Python integration.
- Expand dataset for more stores and customer demographics.

---

## 🧠 Key Takeaway
This project showcases an end-to-end Excel workflow:
- **Data Cleaning → Analysis → Visualization → Insights**

It replicates the day-to-day tasks of a **Junior Data Analyst** and proves capability in handling messy data, performing structured analysis, and communicating business value through clear dashboards.

---

### 👤 Author
**Kilson Joaquim**  
📍 London, UK  
🔗 [LinkedIn](https://www.linkedin.com/in/kilsonjoaquim/) | [GitHub](https://github.com/KilsonJ)
