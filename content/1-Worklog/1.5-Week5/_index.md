---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Deploy shared storage systems for Windows (Amazon FSx) and secure web workloads with AWS WAF firewalls.
* Establish metadata management with Resource Tagging and control access using attribute-based parameters (ABAC).
* Configure visualization platforms (Grafana) for tracking performance and implement IAM Permission Boundaries.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Launch Amazon FSx for Windows File Server in SSD/HDD Multi-AZ config.<br>- Map default shares, enable Data Deduplication, configure Shadow Copies, and configure quotas. | 05/18/2026 | 05/18/2026 | <https://000025.awsstudygroup.com/> |
| Tue | - Research AWS WAF mitigation for web vulnerability threats (OWASP Top 10).<br>- Deploy sample web application, configure Web ACL, and write custom rules to block SQLi and XSS. | 05/19/2026 | 05/19/2026 | <https://000026.awsstudygroup.com/> |
| Wed | - Build standard tagging schemes for cloud assets (Resource Tagging).<br>- Set up Resource Groups and apply IAM Policies checking resource tags dynamically (ABAC model). | 05/20/2026 | 05/20/2026 | <https://000027.awsstudygroup.com/><br><https://000028.awsstudygroup.com/> |
| Thu | - Install Grafana Server on a Linux EC2 instance.<br>- Assign CloudWatch integration IAM Roles, configure data sources, and build monitoring dashboards. | 05/21/2026 | 05/21/2026 | <https://000029.awsstudygroup.com/> |
| Fri | - Research IAM Permission Boundaries to mitigate privilege escalation risks.<br>- Design Restriction Policies setting maximum boundaries and test blocking out-of-scope tasks. | 05/22/2026 | 05/22/2026 | <https://000030.awsstudygroup.com/> |

### Week 5 Achievements:

* **Shared Windows Storage (FSx)**: Deployed highly available shared storage, optimized space with deduplication, and verified shadow copy user restore processes.
* **Web Security (WAF)**: Blocked simulated SQL Injection, XSS, and DDoS threats by associating Web ACL rules with public web endpoints.
* **Tag-based Access Control (ABAC)**: Enabled scale-friendly dynamic permissions, allowing control of instance cycles based on matching resource tags rather than hardcoded policies.
* **Performance Dashboards (Grafana)**: Integrated CloudWatch metrics into central Grafana displays, tracking infrastructure health metrics in real-time.
* **Authorization Boundaries**: Established strict limits on administrative privileges, containing potential user permission escalation vulnerabilities.
