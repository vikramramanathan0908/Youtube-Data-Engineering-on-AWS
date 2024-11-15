# Youtube-Data-Engineering-on-AWS
This repository showcases an end-to-end data engineering project using AWS services (S3, Glue, Lambda, Athena, QuickSight) to process and analyze YouTube trending data. It covers automated ETL pipelines, data transformations, and insightful visualizations to uncover trends in video engagement and performance.

## Overview
This project focuses on building an end-to-end data engineering solution using the YouTube trending dataset from Kaggle. The goal is to process and analyze YouTube trending videos to derive meaningful insights, using various AWS services for data storage, transformation, and visualization.

## Project Objectives
- Create a cloud-based data pipeline to ingest, transform, and visualize YouTube data.
- Understand and analyze key factors that contribute to the popularity of YouTube videos.
- Provide actionable insights for targeted advertising strategies on YouTube.

## Data Sources
The dataset consists of:
- JSON file containing video categories.
- CSV file with trending video data from multiple regions.

## Architecture
![Project Architecture](Replace with your image link)

## AWS Services Used
- **Amazon S3**: For data storage.
- **AWS Glue**: For data cataloging and ETL operations.
- **AWS Lambda**: For serverless data transformation.
- **Amazon Athena**: For querying and analyzing data.
- **AWS QuickSight**: For data visualization and dashboards.

## Steps Involved

### 1. Data Ingestion
- Created an S3 bucket and uploaded raw data (JSON and CSV files).
- Used AWS CLI to manage data upload.

### 2. Data Cataloging with AWS Glue
- Created Glue Crawlers to scan and extract metadata from raw data.
- Generated Glue Data Catalogs for efficient querying with Athena.

### 3. Data Transformation
- Used AWS Lambda functions to normalize JSON data and convert it to Apache Parquet format.
- Created Glue ETL jobs to transform raw CSV data into query-optimized formats.

### 4. Data Analysis with Amazon Athena
- Queried and joined raw and cleaned datasets.
- Handled data type mismatches and optimized query performance.

### 5. Data Visualization
- Created interactive dashboards with AWS QuickSight, showcasing views, likes, comments, engagement rates, and more.
- Provided insights into video performance and user engagement trends.

## Key Features
- Automated ETL pipeline using AWS services.
- Data partitioning for optimized query performance.
- Interactive dashboards for business insights.

## Challenges and Solutions
- **Handling Nested JSON**: Used AWS Lambda to flatten and transform data.
- **Schema Mismatch**: Resolved data type inconsistencies for optimized queries.
- **Non-English Characters**: Applied filters to manage language-specific data processing.
