---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Study virtualization technology and practice virtual machine migration (VM Import/Export).
* Understand container technologies (Docker/Docker Compose) and container orchestration on Amazon ECS.
* Build automated CI/CD pipelines for containers and manage security compliance with AWS Security Hub.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Research VM Import/Export: export Ubuntu VM from VMware Workstation to S3.<br>- Configure IAM Roles and import S3 VM files to Custom AMIs.<br>- Launch EC2 instances from custom AMIs and verify connection. | 05/04/2026 | 05/04/2026 | <https://000014.awsstudygroup.com/> |
| Tue | - Learn Docker basics: Dockerfile, Images, Containers, and basic commands.<br>- Set up EC2 instances running Docker and manage multi-container apps with Docker Compose.<br>- Create Amazon ECR repositories, configure IAM permissions, and push Docker images. | 05/05/2026 | 05/05/2026 | <https://000015.awsstudygroup.com/> |
| Wed | - Study Amazon ECS architecture: Clusters, Task Definitions, and Services.<br>- Create an ECS Cluster (EC2 launch type) with Application Load Balancer and AWS Cloud Map integration.<br>- Practice ECS rolling updates and Blue/Green deployment strategies. | 05/06/2026 | 05/06/2026 | <https://000016.awsstudygroup.com/> |
| Thu | - Design container CI/CD pipeline on Amazon ECS.<br>- Configure GitLab code repository, write `.gitlab-ci.yml`, and integrate with AWS CodeBuild.<br>- Automate build, push image to ECR, and deploy update to ECS. | 05/07/2026 | 05/07/2026 | <https://000017.awsstudygroup.com/> |
| Fri | - Learn AWS Security Hub and cloud compliance standards (CIS AWS Foundations, PCI DSS).<br>- Enable Security Hub in the AWS account, analyze security findings, and configure AWS Config remediation. | 05/08/2026 | 05/08/2026 | <https://000018.awsstudygroup.com/> |

### Week 3 Achievements:

* **VM Migration (VM Import/Export)**: Successfully migrated on-premises virtual machines to AWS Custom AMIs and exported cloud resources back to local virtualization formats.
* **Containerization (Docker & ECR)**: Mastered writing optimized Dockerfiles, managing multi-container deployments using Docker Compose, and securely pushing images to ECR.
* **Orchestration (Amazon ECS)**: Deployed containerized workloads on ECS, configured container network settings, integrated ALB routing, and performed automated Blue/Green deployments.
* **CI/CD Automation**: Created an end-to-end deployment pipeline from GitLab CI to AWS ECR/ECS, ensuring code updates are automatically published to production.
* **Security Auditing (Security Hub)**: Setup centralized security score tracking, resolved misconfigured cloud resources, and analyzed automated remediation workflows.
