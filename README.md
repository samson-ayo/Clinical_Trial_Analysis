# Clinical Trial Data Analysis using Apache Spark, Databricks & AWS

🔍 Project Overview

This project focuses on the large-scale analysis of clinical trial datasets. The goal is to extract valuable insights by integrating clinical trial data with pharmaceutical company listings and condition hierarchy information. The analysis is conducted using Apache Spark (RDD and DataFrame APIs) on Databricks and further extended with AWS Redshift and Athena for scalable querying and reporting.
 
Objectives
 
Ingest and process raw clinical trial data at scale
Join and integrate condition hierarchy and pharmaceutical company datasets
Perform trend analysis and aggregation for reporting
Leverage distributed computing with Spark (RDD and DataFrames)
Store and query data with AWS Redshift and Athena.

Platfrom used (Databricks and AWS)

Tools (Apache Spark (RDD and DataFrame) and AWS (Redshift and Athena))

Data Sources
 
Clinical Trial Datasets
Includes details like trial ID, title, condition, sponsor, and outcome.
Pharmaceutical Companies
Company names, trial involvements, and contact metadata.
Condition Hierarchy
Nested relationships between trial conditions (e.g., parent-child disease classifications).

 Key Tasks Performed
 
Data Ingestion:
Loaded CSV/Parquet datasets into Spark RDDs and DataFrames
Stored intermediate results in AWS S3

Data Integration:

Performed joins across datasets to map trials to pharmaceutical companies and conditions
Cleaned and transformed raw fields using PySpark

Exploratory Data Analysis:

Trend analysis on trial phases, conditions, and sponsors
Aggregation of trial counts per company and condition group

Optimization:
Partitioning and caching strategies for performance tuning
Broadcast joins for smaller lookup datasets

Cloud Querying:

Exported clean datasets to AWS Redshift
Created external tables and ran queries using AWS Athena

Deployment Notes

Spark jobs were run on Databricks notebooks using clusters with 4–8 nodes.
Cleaned data was stored as Parquet in AWS S3 for querying in Athena.
Analytical summaries were loaded into Redshift for business intelligence dashboards.

Outcomes

Created a scalable pipeline for clinical trial data analysis
Improved visibility into trial activity across companies and conditions
Enabled stakeholders to query results without technical knowledge via Athena dashboards
