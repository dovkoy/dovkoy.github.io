B"H

[← Back to Home](/)

# Big Data Pipeline: Advertisement Performance Analysis

## Research Question
How can we orchestrate a complete big data pipeline using NiFi, HDFS, Hive, Spark, and HBase to ingest, store, process, and analyze online advertisement performance data, and what is the predictive power of advertising metrics against total revenue?

## Project Overview
This project demonstrates end-to-end big data pipeline orchestration by deploying a complete workflow that moves an advertisement-performance dataset through multiple big data technologies: Apache NiFi for data ingestion, HDFS for distributed storage, Hive for structured data access, Spark (via YARN) for distributed processing and machine learning, and HBase for NoSQL persistence. The pipeline includes building and evaluating a Linear Regression model to understand the predictive power of advertising metrics against total revenue.

The implementation encompasses four major components:

1. **Data Ingestion with NiFi** - Configuring a NiFi flow to download a synthetic online advertising dataset (100 campaigns with metrics: ad spend, impressions, clicks, conversions, CTR, revenue) from a public GitHub repository and writing it to HDFS, demonstrating real-time data pipeline orchestration

2. **Structured Storage with Hive** - Creating Hive table schemas with appropriate data types (INT for campaign_id and counts, DOUBLE for rates and monetary values), loading CSV data into Hive tables, and handling data quality issues like header row ingestion

3. **Distributed Processing with Spark** - Running Spark MLlib Linear Regression models on YARN cluster, reading data from Hive, training models to predict revenue from advertising metrics, and evaluating performance using RMSE and R² metrics across multiple runs

4. **NoSQL Persistence with HBase** - Creating HBase tables and column families, installing and configuring Thrift server for Spark-HBase communication, and storing model evaluation results (RMSE, R²) in HBase for persistent access

The project demonstrates production-grade big data engineering practices including multi-technology integration, Docker container management, distributed computing with YARN resource allocation, and end-to-end workflow orchestration. Results show the Linear Regression model achieving RMSE values ranging from $4,700 to $6,100 and R² values from 0.16 to 0.50, indicating moderate predictive power that reflects realistic advertising behavior patterns.

## Project Files
- [White Paper (PDF)](https://github.com/dovkoy/msds-portfolio/tree/trunk/docs/projects/big_data_pipeline/white_paper.pdf)

