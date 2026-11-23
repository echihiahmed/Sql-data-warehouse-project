# SQL Data Warehouse Project

## 📌 Project Overview

This project focuses on building a modern Data Warehouse using **Microsoft SQL Server** to integrate, transform, and analyze data from two different business systems: CRM (Customer Relationship Management) and ERP (Enterprise Resource Planning).

The main objective is to centralize sales and customer data into a structured and reliable database, making it easier to perform analytical queries, generate business insights, and support data-driven decision-making.

The project implements an **ETL (Extract, Transform, Load)** process and follows the **Medallion Architecture**, which organizes data into three layers: Bronze, Silver, and Gold.

## 🏗️ Data Architecture

The Data Warehouse is organized into three main layers:

### 1. Bronze Layer
- Stores raw data extracted from CRM and ERP systems.
- Imports data from CSV files into SQL Server.
- Preserves the original structure of the source data.

### 2. Silver Layer
- Cleans and transforms raw data.
- Handles missing values, duplicates, and data inconsistencies.
- Standardizes and integrates data from different systems.
- Ensures data quality and consistency.

### 3. Gold Layer
- Contains business-ready and analytical data.
- Organizes information using a Star Schema.
- Includes fact and dimension tables.
- Supports reporting and analytical queries.

## 🔄 ETL Process

The project implements an ETL pipeline consisting of three main steps:

1. **Extract:** Import raw data from CRM and ERP CSV files.
2. **Transform:** Clean, standardize, validate, and integrate the data.
3. **Load:** Store the processed data in the appropriate Data Warehouse layers.

SQL scripts and stored procedures are used to automate data loading and transformation operations.

## 📊 Data Modeling

The Gold Layer uses a Star Schema to organize analytical data.

The data model includes:

- **Dimension Customers:** Contains customer-related information.
- **Dimension Products:** Contains product-related information.
- **Fact Sales:** Stores sales transactions and related measures.

This structure simplifies analytical queries and improves data accessibility.

## 🎯 Project Objectives

The Data Warehouse provides a foundation for analyzing key business activities, including:

- **Customer Behavior:** Understand customer information and purchasing patterns.
- **Product Performance:** Evaluate product performance and sales.
- **Sales Trends:** Analyze sales activities and identify business trends.

## 🛠️ Technologies Used

- **Microsoft SQL Server:** Database management and data storage.
- **SQL:** Data manipulation, transformation, and analytical queries.
- **SQL Server Management Studio (SSMS):** Database administration and SQL development.
- **Git & GitHub:** Source code management and version control.
- **Draw.io:** Data architecture and modeling diagrams.

## 📁 Project Structure

```text
Sql-data-warehouse-project/
│
├── datasets/
│   ├── source_crm/
│   └── source_erp/
│
├── docs/
│
├── scripts/
│   ├── init_database.sql
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── tests/
│
├── README.md
└── LICENSE
```

## 🧪 Data Quality & Testing

Data quality checks are performed to ensure the reliability and consistency of the Data Warehouse.

These checks include:
- Identifying duplicate records.
- Detecting missing or invalid values.
- Validating data consistency.
- Checking relationships between tables.
- Verifying the quality of the Silver and Gold layers.

## 🚀 Expected Results

At the end of this project, the Data Warehouse provides:

- A centralized database integrating CRM and ERP data.
- A structured ETL pipeline.
- Clean, standardized, and reliable data.
- An analytical data model based on a Star Schema.
- A foundation for business intelligence and reporting.
