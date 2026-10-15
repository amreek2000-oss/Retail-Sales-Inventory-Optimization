🛒 Enterprise Retail Analytics & Inventory Optimization

📌 Executive Summary:

An end-to-end data engineering and business intelligence solution processing 301,647 enterprise transaction records. This project transforms raw, unstructured sales data into a normalized MySQL relational model and serves interactive executive dashboards via Power BI.

🎯 Key Performance Indicators (KPIs):

💰 Total Revenue: $76.78M:- (Net top-line financial performance across all product categories).
👥 Unique Customers: 86,728:- (Total distinct customer base engaging in active transactions).
📦 Total Items Purchased: 1.61M+ Units:- (Complete volume of inventory units sold across channels).
💳 Average Order Value (AOV): $255.16:- (Mean monetary spend generated per customer transaction).

🏗️ System Architecture & Data Pipeline:

Raw Transaction Logs (301k+ Records) 👇  (Inconsistent formats, missing values, duplicates).

🐍 Python ETL Engine (data_cleaning.py)👇  (Null remediation, schema standardization, type casting).

📄 Cleaned CSV Data Pipeline (Cleaned_Retail_Sales.csv)👇  (Production-ready dataset).

🐬 MySQL Relational Database (retail_inventory_db)👇  (Normalized DDL schemas & primary key indexing).

📊 Interactive Power BI BI Suite (Dashboard.pbix)👇  (Executive KPIs, temporal trends & category breakdowns).

🛠️ Technical Stack & Implementation Details:

🐍 1. Python Data Preprocessing (data_cleaning.py):-
🧹 Null Treatment: Safely populated missing categorical entries without dropping valuable records.
🔢 Type Normalization: Explicitly converted financial and volumetric columns (amount, total_purchases) to numerical data types.
🔤 Header Formatting: Standardized column names into consistent snake_case.

🐬 2. Relational Database Schema (MySQL):- 
📐 DDL Implementation: Enforced explicit column data typing (DECIMAL, VARCHAR, INT) optimized for rapid querying.
⚡ Data Integrity: Applied indexed primary keys for efficient join operations and relational scaling.

📊 3. Interactive Dashboards (Power BI):-
📈 Revenue Trend Analysis: Time-series line chart tracking monthly seasonal fluctuations.
🍩 Category Breakdown: Donut chart evaluating top sales contributors across Electronics, Grocery, Clothing, Books, and Home Decor.
🎛️ Dynamic Slicers: Interactive filtering for target market slicing by Country and Payment Method.

💡 Strategic Business Insights:-
📱 Core Revenue Drivers: Electronics and Grocery generate the highest revenue volumes (~45%+ of aggregate sales).
🛍️ High-Value SKUs: Premium items like HDR TV and Google Pixel drive elevated order totals.
💳 Payment Preferences: Digital channels (Credit Card, PayPal, Debit Card) capture over 80% of consumer transactions.

📂 Project Repository Structure:-

├── 📁 data/
│   └── Cleaned_Retail_Sales.csv          # Cleaned production dataset (301k rows)
├── 📁 scripts/
│   └── data_cleaning.py                  # Python ETL pipeline script
├── 📁 database/
│   └── schema_ddl.sql                    # MySQL database creation SQL schema
├── 📁 assets/
│   ├── Dashboard_Overview.png            # Executive Power BI dashboard screenshot
│   ├── monthly_revenue_trend.png        # Monthly trend chart visualization
│   └── revenue_by_category.png          # Category breakdown visual chart
├── 📄 project_report.md                  # Detailed business intelligence report
└── 📄 README.md                          # Repository documentation

🚀 How to Run This Project:-

1️⃣ Clone the Repository:-
git clone https://github.com/your-username/Retail-Sales-Inventory-Optimization.git
cd Retail-Sales-Inventory-Optimization


2️⃣ Run Python Data Pipeline:-
python scripts/data_cleaning.py

3️⃣ Import Database Schema:-
SOURCE database/schema_ddl.sql;


👤 Author & Contact:- Amreek Singh


🌐 GitHub: Amreek2000-oss

💼 LinkedIn: https://www.linkedin.com/in/amreek-singh-767394272

⭐ If you find this project useful, please consider giving it a star on GitHub!







