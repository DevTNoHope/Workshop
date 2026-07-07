---
title: "Week 12 Work Log"
date: 2024-01-01
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Week 12 Objectives:

* Bundle and deploy Frontend client code onto cloud CDN distribution networks (S3 & CloudFront).
* Manage domain routing configurations and HTTPS certificates using Amazon Route 53.
* Setup automated system health monitoring alerts (CloudWatch & SNS) and compile final internship reports.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Compile ReactJS Client code into static assets folder using `npm run build`.<br>- Upload static bundles directly onto S3 bucket `itcoach-static-assets` and configure delivery settings. | 07/06/2026 | 07/06/2026 | ITCoach Manual |
| Tue | - Establish Amazon CloudFront CDN Distribution (`itcoach-distribution`) linking it to S3 static assets.<br>- Set default root object to `index.html`, add custom 403/404 error page responses rewriting to HTTP 200 `/index.html` for React Router routing, and execute cache invalidations. | 07/07/2026 | 07/07/2026 | ITCoach Manual |
| Wed | - Set up Amazon Route 53 domain hosting and custom domain DNS records.<br>- Create A-type Alias records directing primary domain to CloudFront CDN and API subdomains to AWS API Gateway endpoints. | 07/08/2026 | 07/08/2026 | ITCoach Manual |
| Thu | - Configure AWS system alerts: create Amazon SNS Topic (`itcoach-alerts`) and subscribe operator email accounts.<br>- Configure 3 CloudWatch alarms: Lambda execution failures (`itcoach-ai-errors`), API Gateway 5xx rates, and SQS visible messages backlog thresholds. | 07/09/2026 | 07/09/2026 | ITCoach Manual |
| Fri | - Run end-to-end black-box verification testing on the production-grade ITCoach application.<br>- Clean up staging cloud resources, optimize Serverless costs, write project documentation, and summarize internship results. | 07/10/2026 | 07/10/2026 | Internal Documents |

### Week 12 Achievements:

* **CDN Frontend Hosting**: Successfully bundled client codebase, deploying static bundles onto CloudFront CDN with responsive loading and full single-page routing support.
* **DNS Custom Routing**: Completed Route 53 configurations routing custom domain requests securely over HTTPS to CloudFront and API Gateway backends.
* **Proactive Monitoring**: Activated CloudWatch alert notifications to SNS topics, broadcasting email alerts when execution limits or queue visibility thresholds are exceeded.
* **Final Evaluation**: Successfully verified the serverless ITCoach system in production, concluding the internship program at FCAJ.
