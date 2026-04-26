# End-to-End Data Warehouse Project using PySpark, Hive, AWS S3 and Athena

## Overview
This project demonstrates an end-to-end Data Warehouse implementation using PySpark, Hive Metastore, AWS S3, and Athena following a layered data architecture.

### Features
- Data ingestion and processing using PySpark  
- Landing, Staging, and EDW layers  
- Dimension and Fact table creation  
- Hive external table integration  
- AWS S3 data lake storage  
- Athena query support  
- Dockerized development environment  

# Architecture
Source Data → Landing Layer → Staging Layer → EDW (Dimensions + Facts) → Athena Analytics

## Tech Stack
- Python
- PySpark
- Apache Spark
- Hive
- AWS S3
- Amazon Athena
- Docker
- Jupyter Notebook


# Project Structure

```bash
data_with_pyspark/
│
├── datasets/
├── sql/
├── lib/
├── 01_init_db.ipynb
├── 02_date_landing.ipynb
├── 03_date_staging.ipynb
├── 04_date_dim.ipynb
├── 05_store_landing.ipynb
├── 06_store_staging.ipynb
├── 07_store_dim.ipynb
├── 08_customer_landing.ipynb
├── ...
└── 98_generate_athena_ddl.ipynb

# Data Warehouse Layers

## Landing Layer
- Raw data ingestion  
- Minimal transformations  
- Data stored in S3  

## Staging Layer
- Data cleansing  
- Standardization  
- Intermediate transformations  

## Enterprise Data Warehouse (EDW)
- Dimension tables  
- Fact tables  
- Star schema modeling  


# Data Model
Includes:

- Customer Dimension  
- Store Dimension  
- Date Dimension  
- Sales Fact Table  
- Job Control Metadata Table  


# ETL Workflow
1. Load source data into Landing Layer  
2. Transform and validate in Staging Layer  
3. Build Dimensions and Fact tables in EDW  
4. Generate Athena DDLs  
5. Query curated data in Athena  


# Setup Instructions

## Clone Repository
```bash
git clone https://github.com/AkanshaRawat01/data-warehouse-pyspark-project.git
cd data-warehouse-pyspark-project


## Start Docker Environment
```bash
docker-compose up


## Launch Jupyter
```bash
http://localhost:8888


# Key Highlights
- End-to-end Data Warehouse implementation  
- Layered Medallion architecture  
- PySpark ETL pipelines  
- Hive + S3 integration  
- Athena analytics support  
- Docker-based local setup  


# Future Enhancements
- Delta Lake integration  
- Airflow orchestration  
- Data quality validations  
- CI/CD for ETL pipelines  


