# YouTube Data Analytics ETL Pipeline with AWS

This project comprises an end-to-end data pipelining process, from collecting raw data to building a dashboard, focusing on YouTube video statistics data. The goal is to securely manage, streamline, and perform analysis on structured and semi-structured YouTube video data based on video categories and trending metrics.

## Project Overview

### Project Objectives

The primary objective of this project is to build an ETL (Extract, Transform, Load) data pipeline on AWS for YouTube data. This pipeline involves using various AWS services to collect, process, and visualize data, facilitating data-driven insights.The project addresses the need of a client who wants to run ads for their product on social media, specifically YouTube.

### Business Problem

The project addresses common challenges in deploying analytics to the cloud. It deals with differences between on-premises and cloud data platforms, security concerns, and governance issues. The safe transfer of on-premises data to the cloud is essential, particularly in regulated industries where data protection is critical.

## Technology Stack

The project leverages the following technologies and services:

- **Languages**: SQL, Python3
- **AWS Services**:
  - **S3**: Used for storing data, providing scalability, and offering features like object versioning and encryption.
  - **IAM (Identity and Access Management)**: Enables the creation and management of roles and policies, granting specific permissions to users and applications.
  - **Glue**: A fully managed data integration service for creating and running ETL jobs, extracting, transforming, and loading data.
  - **Lambda**: A serverless compute service used for running code and automating data ingestion and processing using triggers.
  - **Athena**: A serverless interactive query service that simplifies data analysis using standard SQL.
  - **QuickSight**: A cloud-native business intelligence service for creating interactive dashboards and reports.

## Architecture Diagram
![YT-Analytics_Architecture](https://github.com/Lohitha-Vanteru/Youtube_Analytics/assets/113141006/505f50c7-e3d0-427b-9156-3fbaa6165257)

## Project Workflow

The project follows a step-by-step workflow:

1. **Data Ingestion**:
   - Raw data is uploaded to an S3 bucket using shell commands.

2. **Identity and Access Management (IAM)**:
   - Roles and policies are created to manage permissions for AWS services.

3. **Data Transformation**:
   - A Python function is coded to transform .json files to Parquet format using AWS Lambda.

4. **ETL Process Automation**:
   - Data processing is automated using triggers through AWS Glue crawler.

5. **Data Querying**:
   - AWS Athena is utilized to query the generated database, allowing for data analysis.

6. **Dashboard Visualization**:
   - A dashboard is generated to visualize the data using AWS QuickSight.
## Dashboard
![image](https://github.com/Lohitha-Vanteru/Youtube_Analytics/assets/113141006/9c04f7d9-f363-4887-b5f9-91e594d92965)

## Getting Started

### Prerequisites

- An AWS account with access to the mentioned AWS services.
- Knowledge of SQL and Python3.
- Basic familiarity with AWS S3, IAM, Glue, Lambda, Athena, and QuickSight.

### Installation

No specific installation steps are required as this project primarily utilizes AWS services. Make sure you have the necessary access and permissions in your AWS account.

## Usage

- Clone this repository to your local environment.
- Follow the project workflow and use the provided information to implement your YouTube Data ETL pipeline on AWS.
- Refer to the code and configurations within the repository for guidance.

## Acknowledgments

This project is based on the content and tutorials provided by Darshil Parmar on his YouTube channel. We acknowledge the valuable guidance and resources provided by Darshil Parmar, which served as the foundation for this project. You can find his YouTube channel https://lnkd.in/eCsxh9X3.

