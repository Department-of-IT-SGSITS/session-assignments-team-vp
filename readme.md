Cloud Data Lake with ETL & Analytics

Abstract
This project presents a comprehensive approach to building a cloud data lake for aggregating, processing, and analyzing log data originating from multiple sources such as web servers and applications. Utilizing Amazon Web Services (AWS), the solution employs S3 for durable storage, AWS Glue for scalable ETL (Extract, Transform, Load) operations, Amazon Redshift for high-performance data warehousing, and Amazon QuickSight for business intelligence visualization. The outcome is an automated, cost-efficient, and scalable analytics pipeline that converts raw log streams into insightful dashboards to drive operational and business decisions.

Introduction
Modern enterprises collect vast quantities of log data from various systems—web servers, applications, and services in different formats and structures. Such data needs to be centralized, cleansed, enriched, and analyzed efficiently to realize value. Traditional data processing methods are challenged by scale, diversity, and velocity of these logs.
Cloud data lakes provide a centralized repository to ingest and store raw and processed data at scale. This project demonstrates constructing a cloud-native data lake solution leveraging AWS managed services. The architecture emphasizes serverless technologies to minimize operational overhead, enable rapid data transformation pipelines, and support interactive analytical querying and visualization.

Purpose of Work
The project aims to:
Provide a centralized repository (data lake) capable of ingesting diverse log formats from multiple sources.


Build automated ETL pipelines with schema discovery, cleansing, and transformation to convert raw log data into optimized analytics formats.


Enable efficient querying and data warehousing for business intelligence.


Deliver interactive, real-time dashboards for operational insights using BI tools.


Showcase cloud best practices for scalable, cost-effective log analytics.



Working Steps Diagram



System Architecture



Architecture Highlights
Amazon S3: Durable storage for both raw and processed files.
AWS Glue: Serverless data cataloging and ETL engine automating schema discovery and transformation.
Amazon Redshift: Managed data warehousing for running scalable, complex analytical queries.
Amazon QuickSight: Cloud BI for creating interactive dashboards and visualizations.
AWS Identity and Access Management (IAM): Provides secure, fine-grained access control and permission management across services, enabling Redshift and Glue to access S3 data lakes securely while enforcing least privilege access policies.

Hardware and Software Requirements
Hardware
Internet-connected client machine (laptop or desktop), capable of running AWS Console or AWS CLI tools.


Software
Web browser (latest versions of Chrome, Firefox, Edge)


AWS CLI (optional, for some command-line operations)


Python (optional, for AWS Glue script customization)


AWS Services Utilized
Amazon S3 — for raw and processed log storage.
AWS Glue — for data cataloging, schema discovery, and ETL jobs.
Amazon Redshift Serverless — for scalable data warehousing.
Amazon QuickSight — for BI visualization.
AWS IAM — for managing authentication, authorization, and permissions across all AWS resources in the pipeline, including roles assigned to Glue and Redshift.



Conclusion
This project successfully builds an end-to-end cloud data lake and analytics pipeline for log data from ingestion to visualization, leveraging AWS serverless services. The architecture is modular, scalable, and cost-efficient, suitable for extending to various data types and volumes. Interactive dashboards enable stakeholders to derive actionable insights, improving monitoring and decision-making capabilities.

Github Link
https://github.com/pranav050704/cloud-data-lake-etl-analytics

References
AWS Documentation – Data Lake Architecture
https://docs.aws.amazon.com/whitepapers/latest/aws-serverless-data-analytics-pipeline/logical-architecture-of-modern-data-lake-centric-analytics-platforms.html


AWS Glue Getting Started Guide
 https://www.datacamp.com/tutorial/aws-glue


AWS Redshift Serverless User Guide
 https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-serverless.html


AWS QuickSight User Guide
 https://docs.aws.amazon.com/quicksight/latest/user/welcome.html


Kaggle Web Server Access Log Dataset
 https://www.kaggle.com/datasets/eliasdabbas/web-server-access-logs



Screenshots
Initial raw logs schema-





ETL Job Pipeline-







ETL Job Successfully created-





Crawler created Data Catalog-








Table created in redshift warehouse-





Data uploaded into table-








Table rows displayed-





Visualization on Quicksight-

