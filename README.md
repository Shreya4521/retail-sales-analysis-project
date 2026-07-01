# 🛍️ Retail Sales Analysis Dashboard (Excel)

A complete, end-to-end data analytics project built entirely in **Microsoft Excel** — from raw data to a formula-driven dashboard with KPIs and charts. Built as a portfolio project to demonstrate core data analyst skills: data cleaning, formulas, aggregation, and data visualization.

![Dashboard Preview](screenshots/retail_dashboard_preview.png)
---

## 📌 Project Overview

This project analyzes **2,200 retail transactions** across India (Jan 2023 – Dec 2024) spanning 4 regions, 5 product categories, and 3 customer segments. The goal is to identify sales trends, top-performing regions/products, and profitability drivers — then present the findings in an interactive Excel dashboard.

**Objective:** Simulate a real-world retail analyst task — take messy-ish raw transactional data and turn it into decision-ready insights.

---

## 🧰 Tools & Skills Used

| Skill | Applied As |
|---|---|
| Data Cleaning | Consistent date formats, no blanks/duplicates, structured Excel Table |
| Formulas | `SUMIF`, `SUMPRODUCT`, `COUNTIF`, `AVERAGEIF`, `INDEX/MATCH`, `LARGE`, `IFERROR` |
| Aggregation | Pivot-style summary tables by Region, Category, and Month |
| Visualization | Bar chart, Pie chart, Line chart (trend), KPI cards |
| Formatting | Conditional formatting (color scales), currency/percent number formats, Excel Tables |
| Dashboarding | Single-sheet dashboard combining KPIs + charts, all formula-linked to raw data |

---

## 📁 Repo Structure

```
retail-sales-analysis-dashboard/
├── README.md
├── INSIGHTS.md
├── data/
│   └── retail_sales_data.csv          # Raw dataset (2,200 rows)
├── dashboard/
│   └── Retail_Sales_Dashboard.xlsx    # Full workbook: Raw Data + Analysis + Dashboard
└── screenshots/
    └── dashboard_preview.png
```

---

## 📊 Inside the Workbook

The `.xlsx` file has **3 sheets**:

1. **Raw Data** — the full transactional dataset, formatted as a structured Excel Table (`RawData`), with 16 columns: Order ID, Order Date, Ship Date, Ship Mode, Customer Name, Segment, Region, State, City, Category, Product Name, Quantity, Unit Price, Discount, Sales, Profit.

2. **Analysis** — formula-driven summary tables, all calculated *live* from Raw Data (nothing hardcoded):
   - Sales & Profit by Region
   - Sales & Profit by Category (with conditional color-scale formatting)
   - Monthly Sales Trend (2023–2024)
   - Top 10 Products by Sales (via `LARGE` + `INDEX/MATCH`)

3. **Dashboard** — the executive summary view:
   - 6 KPI cards: Total Revenue, Total Profit, Profit Margin, Total Orders, Avg Order Value, Units Sold
   - Bar chart: Sales by Region
   - Pie chart: Sales share by Category
   - Line chart: Monthly sales trend
   - Bar chart: Top 5 products by sales

> Every number on the Dashboard and Analysis sheets is a live formula referencing Raw Data — change the raw data and the entire dashboard recalculates automatically.

---

## 🔑 Key Insights

See [INSIGHTS.md](INSIGHTS.md) for the full write-up. Highlights:

- **West region** leads in total revenue, but all four regions are within ~11% of each other — no single region dominates.
- **Furniture** is the top-grossing category by a wide margin, despite having the lowest profit margin (~7.6%) of all categories.
- **Stationery** has the smallest revenue share but the highest profit margin (~29%) — a high-margin, low-volume category.
- Sales peak sharply in **September–October**, consistent with festive-season buying patterns in India.
- **Standard shipping** is used in ~60% of orders, indicating most customers are not paying for speed.

---

## ▶️ How to Use

1. Download `dashboard/Retail_Sales_Dashboard.xlsx`
2. Open in Excel (or Google Sheets / LibreOffice Calc — formulas are standard Excel syntax)
3. Go to the **Dashboard** sheet for the summary view
4. Explore **Analysis** for the underlying formula logic
5. Explore **Raw Data** — it's a structured Table, so you can insert your own PivotTable/PivotChart on top of it too

---

## 🎯 Why This Project

This project was built to demonstrate the core toolkit expected of an entry-level Data Analyst:
- Comfort working with real transactional data structures
- Writing lookup/aggregation formulas instead of manually computing values
- Building visuals that communicate insight, not just decoration
- Structuring a project cleanly enough for someone else to open and understand immediately

---

## 📬 Contact

Feel free to reach out or connect if you have feedback on this project!
