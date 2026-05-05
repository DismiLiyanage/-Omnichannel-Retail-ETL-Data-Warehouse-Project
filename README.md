#Retail Performance & Analytics Platform (End-to-End BI Solution)

📌 Project Overview

The project transforms fragmented retail data (2020-2024) into a strategic asset using a robust Data Warehouse architecture. It is divided into two core phases:

Phase 01: ETL (Extract, Transform, Load) using SSIS to build a Star Schema.  

Phase 02: Multi-dimensional OLAP modeling with SSAS and interactive visualization with Power BI.

🏗 System Architecture

The solution follows a structured three-tier approach:

Staging Layer: Initial ingestion into Retail_Staging to clean and standardize raw CSV/Excel data.  

Warehouse Layer: Structured Retail_DW utilizing a Star Schema for optimized analytical performance.  

Semantic Layer: SSAS Cubes for complex calculations and Power BI for executive dashboards.  

⚙️ Phase 01: Data Engineering (ETL)

Built using SQL Server Integration Services (SSIS), the ETL pipeline ensures high data quality.

Dimensional Modeling
Fact Tables: Sales, Support, Interactions, and Product Reviews.  

Dimension Tables: Customer, Product, Date, and Marketing Campaigns.  

Key Transformations
Data Conversion: Standardizing data types for mathematical consistency.  

Lookup Logic: Efficiently mapping business keys to surrogate keys.  

Derived Columns: Calculating complex metrics like TotalAmount and txn_process_time_hours.  

💎 Phase 02: Business Intelligence (SSAS & Visualization)

This phase focuses on making the data actionable for decision-makers.

OLAP Modeling (SSAS)
Cube Structure: Developed a multi-dimensional cube in SQL Server Analysis Services.  

Hierarchies: Created drill-down capabilities (e.g., Year > Quarter > Month > Day).  

Calculated Measures: Implemented KPIs using MDX to track retail performance.  

Data Visualization (Power BI)
Interactive dashboards were designed to monitor:

Sales Performance: Identifying top-selling categories and seasonal trends.  

Customer Insights: Analyzing demographics and regional purchase patterns.  

Service Efficiency: Tracking support response times and customer satisfaction.  

✅ Quality Assurance

To guarantee "Single Version of Truth," the following was implemented:

Data Validation: Row count audits between Source, Staging, and DW.  

Integrity Checks: Group-by analysis to identify and eliminate duplicate primary keys.  

🛠 Tech Stack

Databases: MS SQL Server (SSMS)

Integration: SQL Server Integration Services (SSIS)

Analytics: SQL Server Analysis Services (SSAS)

Visualization: Power BI Desktop

Source Formats: CSV, Excel (.xlsx)
