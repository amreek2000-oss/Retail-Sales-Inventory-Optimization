🛒 Retail & Sales Inventory OptimizationAn enterprise-grade, end-to-end Data Analytics portfolio project demonstrating Data Engineering, Relational Database Design, and Executive Dashboarding using a massive dataset of 301,647 transaction records.📌 Executive SummaryThis project analyzes retail transaction patterns and inventory metrics to empower stakeholders with actionable sales insights. By building an automated data pipeline and visual analytics reporting suite, this solution optimizes stock levels, tracks consumer spending, and evaluates top-performing product categories.🎯 Key Performance Indicators (KPIs)💰 Total Revenue👥 Total Customers📦 Total Purchases💳 Avg Order Value$76.78M86,7281.61M+$255.16🏗️ Technical Architecture┌─────────────────┐      ┌─────────────────┐      ┌─────────────────┐
│   Raw Data      │ ───► │  Python Pipeline│ ───► │  Cleaned Data   │
│ (301k+ Records) │      │ (Pandas/NumPy)  │      │  (CSV Storage)  │
└─────────────────┘      └─────────────────┘      └─────────────────┘
                                                           │
                                                           ▼
┌─────────────────┐      ┌─────────────────┐      ┌─────────────────┐
│ Power BI Dashboard│ ◄───│ Relational DB   │ ◄───│  MySQL Database │
│ (Visual Analytics)│    │ (Data Modeling) │      │ (Schema & DDL)  │
└─────────────────┘      └─────────────────┘      └─────────────────┘
📊 Key Dashboard InsightsMonthly Revenue Trends: Identified high-volume peak months, allowing inventory managers to pre-stock fast-moving inventory.Category Breakdown: Electronics and Grocery emerge as primary revenue engines, together generating over 45% of total enterprise sales.Top 10 Product Ranking: Product-level ranking pinpoints high-margin SKUs such as HDR TV, Literary Fiction, and Google Pixel.🛠️ Tooling & Tech StackPython (Pandas & NumPy): Automated cleaning, missing value handling, datetime standardization, and deduplication.MySQL: Custom database architecture (retail_inventory_db), explicit column typing, and schema design.Power BI Desktop: Dynamic DAX metrics, custom interactivity, multi-slicer filtering, and user-centric layout formatting.📂 Repository Layout.
├── 📁 data/
│   └── Cleaned_Retail_Sales.csv       # Production-ready dataset
├── 📁 scripts/
│   └── data_cleaning.py               # Automated Python ETL pipeline
├── 📁 database/
│   └── schema_ddl.sql                 # MySQL schema creation scripts
├── 📁 assets/
│   ├── Dashboard_Overview.png         # Power BI dashboard screenshot
│   ├── monthly_revenue_trend.png     # Trend graph visual
│   └── revenue_by_category.png       # Category breakdown visual
├── 📄 project_report.md               # Comprehensive Analytical Project Report
└── 📄 README.md                       # Repository Documentation
🚀 Getting StartedPrerequisitesPython 3.8+MySQL Workbench / ServerPower BI DesktopQuickstart GuideClone the repository:git clone https://github.com/your-username/retail-sales-inventory-optimization.git
Run Data Preprocessing:python scripts/data_cleaning.py
Set up Database:
Import database/schema_ddl.sql into MySQL Server.View Visuals:
Open the .pbix file in Power BI Desktop or inspect the screenshots in assets/.👤 Author & ContactAmreekData Analyst | BI & Business Intelligence SpecialistLinkedIn: Your LinkedIn ProfilePortfolio: Your Portfolio LinkIf you find this project helpful or inspiring, feel free to give it a ⭐️!
