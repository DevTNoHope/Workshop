---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:

* Implement advanced monitoring using Amazon CloudWatch (Logs Insights, Metric Expressions).
* Automate infrastructure provisioning with AWS CloudFormation and AWS Cloud Development Kit (CDK).
* Master DynamoDB NoSQL databases and build CUR report analysis platforms using AWS Glue and Athena.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Configure advanced CloudWatch metrics with search/math expressions and dynamic labels.<br>- Setup CloudWatch Logs, write analytical queries in Logs Insights, and build metric filters with alarms. | 06/01/2026 | 06/01/2026 | <https://000036.awsstudygroup.com/> |
| Tue | - Research Infrastructure as Code (IaC) architectures with AWS CloudFormation.<br>- Write stack templates with Custom Resources (Lambda triggers), Mappings, StackSets, and run Drift Detection. | 06/02/2026 | 06/02/2026 | <https://000037.awsstudygroup.com/> |
| Wed | - Investigate AWS Cloud Development Kit (CDK) to define cloud architecture using programming code.<br>- Build CDK Stacks (VPC, S3, EC2), run bootstrap/deploy commands, and configure EC2 User Data script. | 06/03/2026 | 06/03/2026 | <https://000038.awsstudygroup.com/> |
| Thu | - Learn DynamoDB NoSQL operations: tables creation, CLI queries, and Scans.<br>- Configure Global Secondary Indexes (GSI) for query optimization, run ACID Transactions, and enable PITR backups. | 06/04/2026 | 06/04/2026 | <https://000039.awsstudygroup.com/> |
| Fri | - Build a cost analysis querying engine for CUR reports using AWS Glue and Amazon Athena.<br>- Create Glue Catalog schema from S3 Parquet datasets and execute SQL optimization queries. | 06/05/2026 | 06/05/2026 | <https://000040.awsstudygroup.com/> |

### Week 7 Achievements:

* **Advanced Monitoring (CloudWatch)**: Utilized Logs Insights to query application log volumes, configured Metric Filters tracking system failures, and designed unified dashboards.
* **Declarative IaC (CloudFormation)**: Created robust templates to provision instances, integrated Lambda custom resources, and verified resource drifts using Drift Detection.
* **Imperative IaC (AWS CDK)**: Wrote structured infrastructure code using TypeScript, deployed cloud stacks on Cloud9, and bootstrapped instances using EC2 User Data.
* **NoSQL Database (DynamoDB)**: Implemented partition-key patterns, optimized queries using Global Secondary Indexes (GSI), and set up ACID transaction security with PITR continuous restore logs.
* **Cost Analysis (CUR via Athena)**: Created CUR SQL databases using Athena, extracted tag-allocated costs grouped by CostCenter, and compared Reserved Instance/Savings Plans billing efficiency against On-Demand.
