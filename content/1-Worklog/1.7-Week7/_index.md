---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---
### Week 7 Objectives:

* Build a serverless Data Lake architecture on AWS using Amazon S3 as the primary storage layer.
* Automate metadata cataloging and ETL (Extract, Transform, Load) jobs using AWS Glue.
* Query S3 data directly using SQL with Amazon Athena and visualize insights using Amazon QuickSight dashboards.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Learn Data Lake architecture and the lifecycle stages of big data (Ingest, Store, Process, Analyze)<br>- Configure tiered S3 Buckets representing: Raw, Processed, and Curated Zones<br>- Set up IAM roles and access permissions for analytics services | 06/01/2026 | 06/01/2026 | <https://000035.awsstudygroup.com/> |
| Tue | - Study AWS Glue components: Data Catalog, Crawlers, Connections, and Jobs<br>- Create and configure an AWS Glue Crawler to scan raw data stored in S3<br>- Verify crawl results and check generated schemas in the Glue Data Catalog | 06/02/2026 | 06/02/2026 | <https://000035.awsstudygroup.com/> |
| Wed | - Build an ETL (Extract, Transform, Load) Job in AWS Glue<br>- Configure data format conversion from row-oriented formats (like CSV/JSON) to columnar formats (Parquet)<br>- Apply S3 data partitioning to accelerate queries and reduce operational costs | 06/03/2026 | 06/03/2026 | <https://000070.awsstudygroup.com/> |
| Thu | - Learn Amazon Athena serverless query engine capabilities<br>- Configure S3 query output location requirements<br>- Write standard SQL queries to perform analysis directly on S3 data cataloged in Glue | 06/04/2026 | 06/04/2026 | <https://000106.awsstudygroup.com/> |
| Fri | - Register and set up the Amazon QuickSight environment<br>- Configure data source connections to Amazon Athena and import datasets into SPICE storage<br>- Design interactive visualization charts and publish secure business dashboards | 06/05/2026 | 06/05/2026 | <https://000073.awsstudygroup.com/> |

### Week 7 Achievements:

* **Built a Serverless Data Lake:**
  * Implemented a structured multi-tiered S3 storage design adhering to enterprise big data standards.
  * Leveraged S3's low-cost, high-durability storage architecture to manage scalable analytical data pools.

* **Automated Data Processing with AWS Glue:**
  * Successfully operated Glue Crawlers to discover heterogeneous schemas automatically and maintain a centralized Data Catalog.
  * Executed ETL transformation jobs to compress raw logs into partitioned Parquet files, decreasing query scan data sizes by up to 80%.

* **Data Analysis & Visualization:**
  * Executed SQL queries using Athena directly against S3 objects, obtaining analytical results quickly without maintaining database servers.
  * Designed and published multi-dimensional QuickSight business intelligence dashboards to help make data-driven decisions.
