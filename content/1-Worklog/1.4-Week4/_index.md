---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Implement advanced multi-VPC networking solutions (VPC Peering and AWS Transit Gateway).
* Automate cost optimization for EC2 virtual servers using serverless AWS Lambda triggers.
* Build automated CI/CD pipelines using native AWS developer tools and integrate hybrid cloud storage solutions.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Research VPC Peering connections for cross-VPC networking.<br>- Write CloudFormation templates to deploy Multi-VPC infrastructure automatically.<br>- Configure routing tables, update Security Groups, and verify private IP connections. | 05/11/2026 | 05/11/2026 | <https://000019.awsstudygroup.com/> |
| Tue | - Research AWS Transit Gateway architecture for hub-and-spoke networking.<br>- Create Transit Gateway, attach target VPCs, and configure route table propagation.<br>- Verify end-to-end communication between EC2 instances across VPC boundaries. | 05/12/2026 | 05/12/2026 | <https://000020.awsstudygroup.com/> |
| Wed | - Investigate EC2 cost optimization by stopping idle instances outside business hours.<br>- Write AWS Lambda functions to stop/start EC2 instances filtering by Resource Tags.<br>- Configure Amazon EventBridge triggers and SNS notification systems. | 05/13/2026 | 05/13/2026 | <https://000022.awsstudygroup.com/> |
| Thu | - Build a CI/CD pipeline using AWS CodeCommit, CodeBuild, CodeDeploy, and CodePipeline.<br>- Install CodeDeploy Agent on EC2 targets, write `buildspec.yml` and `appspec.yml` configurations.<br>- Assemble 3-stage pipeline: Source -> Build -> Deploy. | 05/14/2026 | 05/14/2026 | <https://000023.awsstudygroup.com/> |
| Fri | - Learn about AWS Storage Gateway to link on-premises and cloud data stores.<br>- Deploy a File Gateway appliance on EC2 with Amazon S3 storage backend.<br>- Mount SMB/NFS network shares on client computers and verify automatic synchronization. | 05/15/2026 | 05/15/2026 | <https://000024.awsstudygroup.com/> |

### Week 4 Achievements:

* **Cross-VPC Routing (Peering & Transit Gateway)**: Built secure multi-tier networking topologies using CloudFormation. Successfully routed data across network boundaries using peering connections and central Transit Gateway hubs.
* **Automated Cost Optimization**: Scheduled automated shutdown rules for computing resources outside business hours via Lambda, generating operational savings.
* **AWS Developer Suite Pipelines**: Set up native AWS developer pipelines, triggering automated compile-test-deploy operations on target instances upon code delivery.
* **Hybrid Storage Deployment**: Connected storage volumes seamlessly with S3 backends, providing local caches with secure cloud durability.
