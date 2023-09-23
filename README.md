# YouTrend Insights: Analyzing YouTube Video Landscape

## Project Overview
This project is centered around efficiently managing, streamlining, and performing comprehensive analysis on structured and semi-structured YouTube video data. The initiative begins by ingesting data from the Kaggle Dataset. Thereafter, we utilize AWS Lambda for the data cleaning process. The subsequent phase involves processing via the Glue ETL job. Once the processing is complete, the data finds its resting place in AWS Athena, achieved by running Glue Crawler on the dedicated S3 buckets. The culmination of the project lies in the analysis, executed through AWS Quicksight. Additionally, efforts have been put into generating insightful reports via Tableau.

## Architecture Diagram
![Architecture Diagram](https://github.com/dhvani-k/YouTrend_Insights_Analyzing_YouTube_Video_Landscape/blob/main/img/architecture_YouTube%20Trending%20Video%20Analysis.jpeg) 

## What's Inside?
- **Data Ingestion**: Pulling rich datasets straight from Kaggle.
- **Data Cleaning**: Ensuring data quality and integrity using AWS Lambda.
- **Data Transformation**: Harnessing AWS Glue for a robust ETL pipeline.
- **Analysis & Reporting**: Craft beautiful visuals with AWS QuickSight and Tableau.

## AWS Services Implemented:
- **Amazon S3**: Acts as the storage realm, particularly for our structured data in the format of a data lake. Emphasis has been put on partitioning and securely storing data within S3 buckets.
- **AWS IAM**: Dedicated to the management of AWS resources access. Customized IAM policies are a part of this layer, ensuring data access only to those bearing requisite authorization.
- **QuickSight/Tableau**: AWS QuickSight steps into the shoes of a report and insight generator, tapping into the vast reservoir of data within the data lake. Moreover, the platform promises a seamless user interface for crafting reports. Tableau further augments the reporting capabilities.
- **AWS Glue**: Serves as the backbone for the ETL (Extract, Transform, Load) system. Glue seamlessly orchestrates the migration of data into the data lake.
- **AWS Lambda**: A versatile service that springs into action in the face of certain events. Notably, Lambda steps up when there's new data in the source S3 path, initiating the ETL process. Additionally, it plays a crucial role in the data cleansing phase.
- **AWS Athena**: Empowers users with the ability to run SQL queries on data residing in the data lake, all without the hassle of server management.

## Importance of Trend Analysis
The digital age is governed by data. Analyzing YouTube's trending videos provides:

- **User Insights**: Understand the pulse of the audience.
- **Content Strategy**: Unearth what kind of content resonates.
- **Marketing Leverage**: Optimize advertising and outreach efforts.

