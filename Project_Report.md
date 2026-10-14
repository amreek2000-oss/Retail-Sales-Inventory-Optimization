# 📊 End-to-End Retail & Sales Inventory Optimization Report

## 📌 Executive Summary

The **Retail & Sales Inventory Optimization** project is an end-to-end data analytics solution designed to monitor enterprise revenue channels, analyze multi-category product demand, evaluate regional purchasing behavior, and optimize inventory tracking. By bridging Python-based Extract, Transform, Load (ETL) pipelines with an advanced Power BI executive dashboard, this project delivers real-time actionable insights into top-performing stockkeeping units (SKUs) and gross sales performance.

## 🏗️ Architecture & Workflow

The data pipeline spans raw ingestion to interactive business intelligence delivery:

```
[ Raw Dataset ] ➔ [ Python (Pandas) ETL & Data Cleaning ] ➔ [ Cleaned CSV ] ➔ [ Power BI / DAX Modeling ] ➔ [ Executive Dashboard & Visuals ]
```

1. **Data Preprocessing (Python):** Handled missing records, standardized datetime structures, and engineered chronological ordering attributes (`Month_Number`).

2. **Data Modeling (Power BI):** Established tabular relationships, built custom measure configurations, and structured multi-criteria data slicers.

3. **Interactive Visualization:** Designed clean, executive-level metric cards, dynamic time-series trends, and categorical distribution breakdowns.

## 📈 Key Performance Indicators (KPIs) & Financial Metrics

The system tracks core operational and monetary indicators dynamically based on selected regional and payment filters:

| Metric Name | Value / Scope | Business Significance |
| :--- | :--- | :--- |
| **Total Revenue** | \$76,973.25K | Measures top-line financial performance across global sales channels. |
| **Total Customer Base** | 86,754 | Quantifies unique consumer footprint and customer acquisition reach. |
| **Total Unit Purchases** | 1,614.9K | Tracks inventory movement, product velocity, and stock depletion rates. |
| **Average Order Value (AOV)** | \$255.18 | Evaluates basket size efficiency and customer spending power per transaction. |

## 📊 Analytical Visualizations & Insights

### 1. Monthly Revenue Trend (Chronological Time-Series)
* **Visualization Type:** Spline Line Chart with Data Markers.
* **Technical Implementation:** Resolved default alphabetical sorting issues by mapping month names to a custom numeric `Month_Number` column via DAX (`MONTH([Date])`).
* **Key Insight:** Highlights peak revenue seasons, identifies sales velocity dips, and enables future demand forecasting.

### 2. Revenue Distribution by Product Category
* **Visualization Type:** Donut Chart ($50\%$ Hole Configuration).
* **Key Insight:** Breakdown of percentage contribution across core categories (Electronics, Apparel, Home Decor, Books, Groceries), identifying primary revenue-driving inventory divisions.

### 3. Top 10 High-Demand SKUs
* **Visualization Type:** Horizontal Clustered Bar Chart.
* **Key Insight:** Pinpoints the top-performing products by total revenue generation, allowing inventory managers to prevent stockouts on high-velocity items.

### 4. Regional & Payment Method Slicers
* **Visualization Type:** Global Interactive Dropdown Slicers.
* **Key Insight:** Empowers stakeholders to slice data dynamically by country and payment preference to uncover localized consumer trends.

## 🛠️ Tech Stack & Skills Demonstrated
* **Languages & Scripting:** Python, Pandas
* **Business Intelligence:** Power BI Desktop, Power Query, DAX Expressions
* **Data Management:** Data Cleaning, Type Casting, Missing Value Imputation, Chronological Sorting Logic
* **Version Control:** Git & GitHub Professional Repository Management

## 🚀 How to Run / Replicate This Project
1. Clone or download this repository.
2. Open the `Retail_Sales_Inventory_Optimization.pbix` file using **Power BI Desktop**.
3. Ensure the underlying source points to `Cleaned_Retail_Sales.csv`.

*Project curated and maintained by **Amreek**.*