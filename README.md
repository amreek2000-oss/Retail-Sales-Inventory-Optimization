🛒 Enterprise Retail Analytics & Inventory OptimizationAn end-to-end data engineering and business intelligence project demonstrating scalable ETL processing, relational schema design, and interactive decision-support analytics over 301,647 enterprise transaction records.📌 Business Overview & Problem StatementModern retail enterprises manage high-volume transactional pipelines across diverse product lines and payment channels. Without automated preprocessing and central business intelligence, organizations face:Inventory Disconnects: Overstocking low-margin SKUs while facing stockouts on top revenue drivers.Data Quality Bottlenecks: Fragmented records, inconsistent column formats, and uncategorized entries impacting board-level metrics.Reporting Inefficiencies: Lack of dynamic dashboards for tracking Revenue, Order Value (AOV), and customer buying behavior in real time.This project delivers an automated pipeline that cleanses raw transaction streams, constructs a normalized database model in MySQL, and serves executive metrics via interactive Power BI visual models.📊 Executive Key Performance Indicators (KPIs)MetricEnterprise ValueBusiness SignificanceTotal Revenue$76.78MNet top-line performance across all product categories.Unique Customers86,728Distinct customer base engaging in transaction volume.Total Order Volume1.61M+ UnitsTotal item-level inventory purchases tracked.Average Order Value (AOV)$255.16Average spend generated per customer transaction.🏗️ System Architecture & Data Flow+------------------+      +-------------------------+      +------------------------+
|  Raw Retail Data | ---> |  Python ETL Engine      | ---> | Cleansed CSV Pipeline  |
|  (301k+ Records) |      |  - Null Remediation     |      | (Cleaned_Retail.csv)   |
+------------------+      |  - Type Coercion        |      +------------------------+
                          |  - Structural Normalization       |
                          +-------------------------+                 |
                                                                      v
+------------------+      +-------------------------+      +------------------------+
| Executive BI     | <--- | Business Intelligence   | <--- | MySQL Database         |
| Dashboard        |      | Layer (Power BI DAX)    |      | (retail_inventory_db)  |
+------------------+      +-------------------------+      +------------------------+
🛠️ Tech Stack & Technical Implementation1. Data Pipeline & Processing (Python / Pandas)Automated Ingestion: Handles raw data, standardizing field headers into normalized snake_case formatting.Null Value Remediation: Replaces non-standard values across categorical attributes with explicit tags to preserve data completeness.Numeric Standardization: Coerces financial and volume fields (amount, total_purchases, rating_products) into optimized data types.2. Relational Database Modeling (MySQL)Structured relational schema (retail_inventory_db) utilizing optimized SQL DDL data types (VARCHAR, DECIMAL(10,2), INT).Primary Key and index indexing strategy designed for scalable query performance across millions of rows.3. Analytics & Visualization (Power BI)Developed specialized DAX measures for core business calculations (Total Revenue, Total Customers, Average Order Value).Implemented multi-slicer filtering (Country, Payment Channel, Product Category) to enable drill-down analysis.📈 Key Insights & Strategic RecommendationsCategory Performance Engine: Electronics and Grocery contribute over 45% of total gross sales revenue, signaling key focus areas for supplier negotiation and priority warehousing.SKU Profitability: Top-tier electronics (e.g., HDR TV, Google Pixel) generate high gross margins and should be backed by safety stock buffer targets.Order Flow Optimization: Seasonal trends indicate revenue surges during specific operating quarters, requiring proactive inventory staging 30 days prior to peak periods.📂 Repository Structure├── 📁 data/
│   └── Cleaned_Retail_Sales.csv          # Production-ready dataset
├── 📁 scripts/
│   └── data_cleaning.py                  # Python ETL pipeline script
├── 📁 database/
│   └── schema_ddl.sql                    # MySQL schema creation DDL
├── 📁 assets/
│   ├── Dashboard_Overview.png            # Main Power BI dashboard interface
│   ├── monthly_revenue_trend.png        # Time-series trend analytics visual
│   └── revenue_by_category.png          # Category breakdown bar visual
├── 📄 project_report.md                  # Detailed Analytical Project Report
└── 📄 README.md                          # Repository Documentation
🚀 Execution & Setup Guide1. PrerequisitesPython 3.9+MySQL Server 8.0+Power BI Desktop2. ETL Execution# Clone the repository
git clone https://github.com/your-username/retail-sales-inventory-optimization.git

# Navigate into project directory
cd retail-sales-inventory-optimization

# Execute data cleaning script
python scripts/data_cleaning.py
3. Database DeploymentLoad and execute database/schema_ddl.sql in MySQL Workbench or terminal client:SOURCE database/schema_ddl.sql;
👤 Author & ConnectAmreekData Analyst | Analytics & Business Intelligence SpecialistLinkedIn: Your LinkedIn ProfileGitHub: Your GitHub ProfileIf you find this project informative or useful, please consider giving it a ⭐!
