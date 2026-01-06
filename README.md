# End-to-End Sales Data Warehouse & Analytics Project

This repository showcases an **end-to-end data analytics project** where raw sales data is transformed into meaningful business insights using a modern data warehouse approach.

The project covers the complete analytics lifecycle — from **building a data warehouse**, performing **ETL and data modeling**, to conducting **SQL-based analysis** and delivering **business-focused dashboards**.

Key dashboards and analysis focus on:
- **Customer behavior and segmentation**
- **Product performance and contribution**
- **Overall sales trends and business KPIs**

This project is created as a **portfolio project** to demonstrate practical, industry-relevant skills in data warehousing, analytics, and reporting.

---
## 🏗️ Data Architecture

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver**, and **Gold** layers:

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.

---

## 📖 Project Overview

This project involves:

1. **Data Architecture**: Designing a modern data warehouse using Medallion Architecture with **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from ERP and CRM source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries and reporting.
4. **Exploratory Data Analysis (EDA)**: Performing initial data exploration and data quality checks to understand patterns, trends, and anomalies in sales data.
5. **Advanced Analysis**: Conducting deeper analysis to evaluate sales performance, customer behavior, and product trends using SQL.
6. **Analytics & Reporting**: Creating SQL-based reports and BI-ready datasets.
7. **Dashboards**: Building customer and product performance dashboards to support decision-making.



---
## 🚀 Project Requirements

### Building the Data Warehouse (Data Engineering)

#### Objective
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

#### Specifications
- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

---

### Data Analysis (EDA & Advanced Analytics)

#### Objective
Analyze sales data to uncover trends, patterns, and performance insights across customers, products, and time to support business decision-making.

#### Specifications
- **Exploratory Data Analysis (EDA)**: Perform database, dimension, date, and measure-level exploration to understand data distribution and quality.
- **Trend Analysis**: Analyze change-over-time and cumulative trends to evaluate sales performance and seasonality.
- **Performance Analysis**: Identify top and bottom customers and products using ranking and magnitude analysis.
- **Advanced Analysis**: Conduct part-to-whole analysis and segmentation to understand customer and product contribution.
- **Reporting**: Convert analytical insights into BI-ready datasets and customer and product dashboards.


---

### Customer & Product Performance Dashboards

#### Objective
Provide clear and easy-to-understand dashboards that help business users understand customer behavior and product performance without technical knowledge.

#### Key Highlights
- Shows overall business metrics such as total sales, total customers, total products, quantity sold, and average sales values.
- Customer insights include:
  - Sales breakdown by customer type, country, gender, and age group.
  - Average sales and orders per customer.
  - Identification of customers who may stop purchasing based on recent activity.
- Product insights include:
  - Sales and quantity performance by product category and subcategory.
  - Top-performing products based on revenue.
  - Comparison of product cost and selling price to understand profitability.
- Simple filters allow users to explore data by customer details, product details, categories, and lifecycle information.

These dashboards convert raw sales data into clear business insights to support better customer and product-related decisions.

---


## 📂 Repository Structure
```
1. data-warehouse/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│
├── docs/                               # Project documentation and architecture details
│   ├── etl.drawio                      # Draw.io file shows all different techniquies and methods of ETL
│   ├── data_architecture.drawio        # Draw.io file shows the project's architecture
│   ├── data_catalog.md                 # Catalog of datasets, including field descriptions and metadata
│   ├── data_flow.drawio                # Draw.io file for the data flow diagram
│   ├── data_models.drawio              # Draw.io file for data models (star schema)
│   ├── naming-conventions.md           # Consistent naming guidelines for tables, columns, and files
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│
├── tests/                              # Test scripts and quality files
---------------------------------------------------------------------------------------------------------
2. analysis/
│
├── datasets/                                     # Gold layer datasets used for analysis
│   ├── gold.dim_customers.csv
│   ├── gold.dim_products.csv
│   └── gold.fact_sales.csv
│
├── eda/                                          # Exploratory Data Analysis
│   ├── sql_scripts/                              # SQL scripts for EDA
│   │   ├── 00_init_database.sql
│   │   ├── 01_database_exploration.sql
│   │   ├── 02_dimensions_exploration.sql
│   │   ├── 03_date_range_exploration.sql
│   │   ├── 04_measures_exploration.sql
│   │   ├── 05_magnitude_analysis.sql
│   │   └── 06_ranking_analysis.sql
│   │
│   └── sql_jupyter_scripts/                      # SQL executed via Jupyter notebooks
│       ├── 01_database_exploration.ipynb
│       ├── 02_dimensions_exploration.ipynb
│       ├── 03_date_range_exploration.ipynb
│       ├── 04_measures_exploration.ipynb
│       ├── 05_magnitude_analysis.ipynb
│       └── 06_ranking_analysis.ipynb
│
├── advanced_analysis/                            # Advanced and business-focused analysis
│   ├── sql_scripts/                              # SQL scripts for advanced analysis
│   │   ├── 07_change_over_time_analysis.sql
│   │   ├── 08_cumulative_analysis.sql
│   │   ├── 09_performance_analysis.sql
│   │   ├── 10_data_segmentation.sql
│   │   ├── 11_part_to_whole_analysis.sql
│   │   ├── 12_report_customers.sql
│   │   └── 13_report_products.sql
│   │
│   └── sql_jupyter_scripts/                      # Advanced analysis via Jupyter notebooks
│       ├── 07_change_over_time_analysis.ipynb
│       ├── 08_cumulative_analysis.ipynb
│       ├── 09_performance_analysis.ipynb
│       ├── 10_data_segmentation.ipynb
│       ├── 11_part_to_whole_analysis.ipynb
│       ├── 12_report_customers.ipynb
│       └── 13_report_products.ipynb
│
├── final_bi_ready_reports/                        # Final datasets prepared for BI tools
│   ├── customers_report.csv
│   └── product_report.csv
│
├── docs/                                          # Analysis documentation
│   └── eda_roadmap.png
│
---------------------------------------------------------------------------------------------------------
3. dashboard/
│
├── datasets/                           # Datasets used for dashboard creation
│   ├── Customers_Report.csv            # BI-ready customer report
│   ├── Product_Report.csv              # BI-ready product report
│   ├── Sales.csv                       # Sales fact data for dashboards
│   ├── customers.csv                   # Customer reference data
│   └── products.csv                    # Product reference data
│
├── powerbi/                            # Power BI dashboard files
│   └── end_to_end_dashboard.pbix       # Final end-to-end Power BI dashboard
│
├── docs/                               # Dashboard documentation and exports
│   └── dashboards_pdf.pdf              # Exported dashboard in PDF format
---------------------------------------------------------------------------------------------------------
│ 
│ 
│ 
├── README.md                           # Project overview and instructions


```
---

## 🌟 About Me

Hi there! I'm **Dinesh Kumawat**. I’m a data analyst with hands-on experience in SQL, Python, Excel, Power BI, and Tableau, and a strong interest in solving real business problems using boring raw_data.

Let's stay in touch! Feel free to connect with me on the following platforms:

[LinkedIn](https://www.linkedin.com/in/dineshkumawat1608/)
