---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:

* Deploy Application Load Balancing and Auto Scaling solutions.
* Monitor systems with Amazon CloudWatch and configure Hybrid DNS with Route 53 Resolver.
* Automate AWS administration tasks using AWS CLI and protect resources with AWS Backup.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Deploy Application Load Balancer (ALB) and Auto Scaling Group (ASG) in Multi-AZ environment.<br>- Create EC2 Launch Template and target groups.<br>- Configure scaling policies and verify health check failover. | 04/27/2026 | 04/27/2026 | <https://000006.awsstudygroup.com/> |
| Tue | - Research Amazon CloudWatch: Metrics, Logs, and Alarms.<br>- Create custom CloudWatch Dashboards and configure SNS notification alarms for CPU utilization. | 04/28/2026 | 04/28/2026 | <https://000008.awsstudygroup.com/> |
| Wed | - Set up Hybrid DNS between simulated on-premises Active Directory and Route 53.<br>- Configure Route 53 Inbound/Outbound Endpoints and Resolver Rules for bidirectional query routing. | 04/29/2026 | 04/29/2026 | <https://000010.awsstudygroup.com/> |
| Thu | - Install and configure AWS CLI v2.<br>- Manage AWS resources (S3, IAM, VPC, EC2, SNS) using CLI and write automation scripts using JMESPath query filters. | 04/30/2026 | 04/30/2026 | <https://000011.awsstudygroup.com/> |
| Fri | - Deploy AWS Backup for centralized protection of S3, EC2, and RDS.<br>- Configure backup plans, retention lifecycle policies, and verify restore operations. | 05/01/2026 | 05/01/2026 | <https://000013.awsstudygroup.com/> |

### Week 2 Achievements:

* **Auto Scaling & Load Balancing (ELB/ASG)**: Successfully built a scalable compute infrastructure driven by resource utilization metrics and optimized incoming traffic with Application Load Balancers.
* **System Monitoring (CloudWatch)**: Implemented consolidated performance tracking dashboards for compute and database layers, with real-time alerting using SNS.
* **Hybrid DNS (Route 53 Resolver)**: Integrated simulated on-premises Active Directory DNS resolution with AWS Private Hosted Zones seamlessly.
* **Command Line Management (AWS CLI)**: Gained proficiency in executing core resource operations and automating workflow scripts via AWS CLI querying.
* **Data Protection (AWS Backup)**: Created centralized backups for production assets (EC2 and databases) and validated recovery processes to ensure disaster preparedness.
