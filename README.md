# AWS Data Pipeline Project: Electric Vehicles in Washington State

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
https://github.com/markcoty/aws-end-to-end-pipeline-project/blob/main/Job%20Flow%20Image.png

## Data Transformation Steps
1. Column removals (redundant, irrelevant, or mostly null values)
2. Sporadic null values replacemed with column means
3. Column standardization and removals
4. Derived column creation
5. Export to Parquet for optimized queries

## Athena Queries


## Dashboard Preview


## Cost Notes

