---
title: "Week 1 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Week 1 Objectives:

* Get acquainted with FCAJ unit and study the overview of core AWS services.
* Setup AWS account and configure basic security mechanisms like IAM and MFA.
* Research and deploy VPC network infrastructure, EC2 virtual servers, and RDS relational databases.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Get acquainted with FCAJ unit, rules, and regulations.<br>- Learn core AWS services (Compute, Storage, Network, DB) and setup AWS Free Tier account.<br>- Configure MFA and AWS Budgets for cost control. | 04/20/2026 | 04/20/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Tue | - Research IAM Users, Groups, and Roles.<br>- Create Admin User and Admin Group with AdministratorAccess policy.<br>- Practice switching roles from Operator to Admin and implement least privilege access. | 04/21/2026 | 04/21/2026 | <https://000002.awsstudygroup.com/> |
| Wed | - Learn VPC basics: CIDR, Subnets (Public/Private), Internet Gateway, and NAT Gateway.<br>- Build Multi-AZ VPC network, configure Security Groups, Route Tables, and Network ACLs.<br>- Configure VPC Flow Logs and AWS Site-to-Site VPN. | 04/22/2026 | 04/22/2026 | <https://000003.awsstudygroup.com/> |
| Thu | - Research Amazon EC2, AMI, Instance Types, and EBS volumes.<br>- Deploy Node.js application and MySQL database on both Linux (Amazon Linux 2023) and Windows Server 2025.<br>- Configure PM2 process manager and Nginx as a Reverse Proxy. | 04/23/2026 | 04/23/2026 | <https://000004.awsstudygroup.com/> |
| Fri | - Learn Amazon RDS architecture.<br>- Launch RDS database instance, setup subnet groups, and configure security groups for secure EC2 connection.<br>- Deploy application with RDS backend and practice backup/restore scenarios. | 04/24/2026 | 04/24/2026 | <https://000005.awsstudygroup.com/> |

### Week 1 Achievements:

* **Account Management & Security (IAM)**: Enabled MFA for root account, applied the principle of least privilege using IAM Groups/Roles, and verified secure Switch Role operations.
* **Networking (VPC)**: Created a secure Multi-AZ isolated network environment, controlled traffic with Security Groups (Stateful) and Network ACLs (Stateless), and monitored traffic with VPC Flow Logs.
* **Virtual Compute (EC2)**: Successfully deployed Node.js application on both Linux and Windows Server platforms, optimized with PM2 and Nginx Reverse Proxy.
* **Relational Database (RDS)**: Connected EC2 application server to RDS database securely in private subnets and managed automated backup schedules.
