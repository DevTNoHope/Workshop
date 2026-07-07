---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:

* Automate patch management (SSM) and right-size compute resources (Compute Optimizer).
* Implement encryption at rest (KMS) and analyze operational audit trails (CloudTrail & Athena).
* Analyze spending patterns with Cost Explorer and build real-time Data Lakes for big data ingestion.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Configure centralized node management with AWS Systems Manager (SSM).<br>- Attach SSM Core roles, use Patch Manager for scheduling OS updates, and run commands remotely. | 05/25/2026 | 05/25/2026 | <https://000031.awsstudygroup.com/> |
| Tue | - Install CloudWatch Agent on EC2 instances to collect memory metrics.<br>- Enable AWS Compute Optimizer to analyze performance workloads and recommend right-sizing changes. | 05/26/2026 | 05/26/2026 | <https://000032.awsstudygroup.com/> |
| Wed | - Encrypt S3 buckets at rest using Customer Managed Keys (CMK) in AWS KMS.<br>- Track API history via AWS CloudTrail, store logs on S3, and analyze logs with SQL queries in Athena. | 05/27/2026 | 05/27/2026 | <https://000033.awsstudygroup.com/> |
| Thu | - Evaluate spending efficiency in Cost Explorer following Well-Architected guidelines.<br>- Group usage costs by accounts and services, analyze Savings Plans/RI metrics, and review data transfer costs. | 05/28/2026 | 05/28/2026 | <https://000034.awsstudygroup.com/> |
| Fri | - Build a serverless Data Lake pipeline on AWS: S3, Kinesis Firehose, AWS Glue, Athena, and QuickSight.<br>- Ingest streaming data, generate Glue Catalogs, query data via SQL, and design QuickSight dashboards. | 05/29/2026 | 05/29/2026 | <https://000035.awsstudygroup.com/> |

### Week 6 Achievements:

* **Centralized Operations (SSM)**: Configured automated patch routines via Patch Manager and ran administrative scripts remotely using Run Command.
* **Compute Sizing (Compute Optimizer)**: Collected detailed memory indicators via CloudWatch Agent and evaluated workload capacity limits using Compute Optimizer to reduce waste.
* **Encryption & Logging Audit**: Secured S3 buckets using custom KMS keys, created organization-wide CloudTrail tracking, and built SQL databases in Athena for log queries.
* **Financial Analysis (Cost Explorer)**: Visualized cost variations, mapped account-level spending allocations, and calculated resource requirements for purchasing Savings Plans or Reserved Instances.
* **Serverless Data Lake Ingestion**: Created a stream ingestion pipeline parsing real-time logs, matching schemas automatically with Glue, and building visual dashboards in QuickSight.
