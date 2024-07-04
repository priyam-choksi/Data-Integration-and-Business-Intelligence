# Sales & Purchasing Data Warehouse Integration Project

## Project Overview
This project involves creating a robust data warehouse to support the sales and purchasing operations of the AdventureWorks company. Utilizing multiple data sources from different database systems, the main goal is to provide a unified view that facilitates complex queries and reporting, enhancing business intelligence and decision-making capabilities.

## System Architecture
Multiple databases are used as the source systems for this project:
- **AdventureWorks2016_us** (SQL Server)
- **AdventureWorks2016_eu** (MySQL)
- **AdventureWorks2016_au** (PostgreSQL)
- **AdventureWorks2016_ca** (Oracle)

The target database systems include:
- **AdventureWorksDW_neu** (MySQL for Talend Target)
- **AdventureWorksDW_neu** (SQL Server for SSIS Target)

## Data Integration Strategy
The data integration process involves ETL operations that are performed using Talend and SQL Server Integration Services (SSIS). The main tasks include:
- Loading tables in the target database with data from various source systems.
- Ensuring data quality and consistency across different systems.
- Implementing Slowly Changing Dimensions (SCD Type 1) to handle business changes over time.

## Key Tables in Data Warehouse
The target data warehouse, `AdventureWorksDW_neu`, includes several dimension and fact tables such as:
- **Dimension Tables**: DimStore, DimCustomerPerson, DimCurrency, DimPromotion, DimSalesTerritory, etc.
- **Fact Tables**: FactInternetSales, FactStoreSales, FactPurchases, etc.
- **Reject Tables**: To handle data that does not meet the quality standards.

These tables support a wide range of business queries and are crucial for the analytical reporting of sales and purchasing activities.

## Project Objectives
- **Data Consolidation**: Consolidate data from different geographical locations into a central data warehouse.
- **Business Intelligence**: Enable complex BI queries on consolidated data to provide insights into purchasing patterns, sales performance, and operational efficiency.
- **Reporting**: Support detailed reporting on various dimensions like products, vendors, employees, and sales territories.

## Deliverables
- **Schema List of Tables**: A detailed schema list including tables and row counts.
- **ETL Process Documentation**: Documentation of the ETL processes executed in Talend and SSIS, including screen captures of successful runs.
- **BI Queries and Results**: Execution of various SQL queries to rank vendors by purchase amount, products by sales, and detailed lists of employees and vendors involved in purchasing processes.

---
