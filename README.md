# Chubb_Assignment_5
# 📊 Sales Performance & Trend Analysis Dashboard (Power BI)

## 📌 Project Overview

This project is an **enterprise-grade Power BI dashboard** designed to analyze **Sales Performance, Profitability, Trends, and Target Achievement**. It enables business users and decision-makers to interactively explore data across **time, region, category, and product dimensions**.

The dashboard follows **industry best practices** in data modeling, DAX calculations, and report design.

---

## 🎯 Objectives

* Analyze **Total Sales, Profit, and Quantity**
* Track **monthly and yearly trends**
* Compare **Actual Sales vs Targets**
* Identify **top-performing and underperforming regions & products**
* Enable **interactive, data-driven decision-making**

---

## 🗂️ Data Sources

* **Sales.xlsx** → FactSales (Orders, Products, Customers, Revenue)
* **Targets.xlsx** → FactTargets (Sales Targets by Year, Region, Category)

📌 Excel files act as the **single source of truth** and support refresh in Power BI.

---

## 🔄 Data Transformation (Power Query)

The following transformations were applied using **Power Query Editor**:

* Removed null and duplicate records
* Standardized data types (Date, Decimal, Whole Number, Text)
* Split and cleaned categorical fields
* Created a **Conditional Column (Sales Band)**:

  * High (> 100,000)
  * Medium (> 50,000)
  * Low (≤ 50,000)

These steps ensure **clean, consistent, and analysis-ready data**.

---

## 🧩 Data Modeling

A **Star Schema** design was implemented for optimal performance:

### Fact Tables

* **FactSales**
* **FactTargets**

### Dimension Tables

* **DimDate** (Date hierarchy for time intelligence)
* **DimYear** (Unique year values for targets)
* **DimRegion** (Avoids many-to-many ambiguity)

✔ One-to-many relationships
✔ No fact-to-fact relationships
✔ Ambiguity-free model

---

## 🧮 DAX Measures

### Core Measures

* Total Sales
* Total Profit
* Total Quantity
* Total Target

### Time Intelligence Measures

* Sales YTD
* Sales Last Year (LY)
* Year-over-Year (YoY) Growth %

Measures were used instead of calculated columns for **better performance and reusability**.

---

## 📑 Report Pages

### 1️⃣ Executive Dashboard

* KPI Cards: Sales, Profit, YoY Growth
* Donut Chart: Sales by Category
* Ribbon Chart: Category Rank Over Time
* Line Chart: Monthly Sales Trend

### 2️⃣ Trend Analysis

* Sales & Profit Trends
* Line + Stacked Column Chart
* Regional Sales Map

### 3️⃣ Product Performance

* Matrix: Category → Subcategory → Product
* Conditional formatting (Data bars & color scales)
* Top-N product analysis

### 4️⃣ Sales Trend (R Script Visual)

* Custom R visual for sales trend analysis
* Line plot created using R to visualize sales distribution over time
* Demonstrates integration of advanced analytics within Power BI

---

## 🔍 Filters & Interactivity

* **Report-level filters**: Year, Region, Category
* **Q&A Visual** for natural language querying
* Cross-filtering enabled across all visuals

---

## 🚀 Advanced Features

* Q&A Visual for user-friendly analytics
* Interactive visuals with drill-down support
* Enterprise-ready data model and DAX logic

---

## 📦 Files Included

* `Sales_Performance_Trend_Analysis.pbix`
* `Sales.xlsx`
* `Targets.xlsx`
* `README.md`

---

## ✅ Conclusion

This Power BI dashboard provides a **comprehensive, scalable, and interactive analytics solution** for monitoring business performance. It demonstrates strong proficiency in **data modeling, DAX, Power Query, and visualization best practices**.


## 👤 Author

**Vivek Kurapati**



