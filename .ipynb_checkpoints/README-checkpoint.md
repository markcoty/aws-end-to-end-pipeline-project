# End-to-End AWS Data Pipeline Project: Electric Vehicles in Washington State

## Overview
This project demonstrates an end-to-end cloud-based data pipeline using AWS services. A raw dataset was ingested into S3, cataloged and cleaned using AWS Glue, queried using Athena, and visualized in QuickSight.

## Tools Used
- AWS S3
- AWS Glue (Crawler + PySpark ETL Job)
- AWS Athena
- Amazon QuickSight

## Dataset
**Name**: Electric_Vehicle_Population_Data  
**Source**: https://catalog.data.gov/dataset/electric-vehicle-population-data 
**Description**: The data contained a large number of missing values (especially in the MSRP, range, and clean alternative fuel vehicle status columns).

## Pipeline Architecture
https://github.com/markcoty/aws-end-to-end-pipeline-project/blob/main/AWS-architecture.png

## Data Transformation Steps
1. Null value removal
2. Column standardization
3. Derived column creation
4. Export to Parquet for optimized queries

## Athena Queries
- [Top 10 regions by incident count](athena_queries/example_query_1.sql)
- [Time-series analysis of XYZ](athena_queries/example_query_2.sql)

## Dashboard Preview
![QuickSight Dashboard](quicksight/dashboard_screenshot.png)

## Cost Notes
Total AWS usage during the project: ~$1.50  
See: [Cost Alert Setup](cost_tracking/budget_alert_config.md)
