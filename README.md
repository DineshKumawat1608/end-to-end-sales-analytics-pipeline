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
![Data Architecture]((1.%20data%20warehouse/docs/data_architecture.PNG))

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.

---
## 📖 Project Overview

This project involves:

1. **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.


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

### BI: Analytics & Reporting (Data Analysis)

#### Objective
Develop SQL-based analytics to deliver detailed insights into:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

These insights empower stakeholders with key business metrics, enabling strategic decision-making.  

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

2. 

├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├──
├── README.md                           # Project overview and instructions


```
---

## 🌟 About Me

Hi there! I'm **Dinesh Kumawat**. I’m an data analyst with hands-on experience in SQL, Python, Excel, Power BI, and Tableau, and a strong interest in solving real business problems using boring raw_data.

Let's stay in touch! Feel free to connect with me on the following platforms:

[![LinkedIn](www.linkedin.com/in/
dineshkumawat1608
)
