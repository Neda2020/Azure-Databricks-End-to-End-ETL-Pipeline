# Azure-Databricks-End-to-End-ETL-Pipeline

## Overview
This project demonstrates an end-to-end ETL pipeline using PySpark and Delta Lake.

## Architecture
(Bronze → Silver → Gold)
Bronze: (Data ingestion: transactions.csv, customers.csv , ...)
Silver: (Transformation: null handling, type casting, joins, ... & Data Validation: row count check, null check, duplicate check, ...) 
Gold: (Buisiness Ready:aggregated transactions, customer summary, ...)

## Tech Stack
- PySpark
- Delta Lake
- SQL

## Data Flow
1. Raw data ingestion
2. Data cleaning and transformation
3. Data validation
4. Aggregation and final tables

   /data
/notebooks
    - 01_ingestion.py
    - 02_transformation.py
    - 03_validation.py
    - 04_gold_layer.py
/sql
    - validation_queries.sql
/utils
    - helper_functions.py
/README.md

## Key Features
- Data quality validation
- Layered architecture
