---
title: "Week 8 Worklog"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:

* Initialize the ITCoach project: Conduct system analysis, define data flows, and design Serverless architecture on AWS.
* Establish S3 storage resources and configure IAM security credentials.
* Set up Amazon Cognito centralized authentication pools and deploy Amazon SQS messaging queues.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Research ITCoach project proposal: define target users, study objectives, quiz modules, and AI evaluation components.<br>- Perform system design analysis and draft the Serverless architecture integrating S3, Cognito, API Gateway, Lambda, SQS, DynamoDB, Polly, and OpenAI. | 06/08/2026 | 06/08/2026 | Internal Documents |
| Tue | - Create centralized IAM execution role (`itcoach-lambda-role`) for Lambda functions.<br>- Attach 6 required policies: `AWSLambdaBasicExecutionRole`, `AmazonDynamoDBFullAccess`, `AmazonS3FullAccess`, `AmazonSQSFullAccess`, `AmazonPollyFullAccess`, and `CloudWatchFullAccess`. | 06/09/2026 | 06/09/2026 | Internal Documents |
| Wed | - Initialize 2 S3 buckets: public website bucket `itcoach-static-assets` and private audio upload bucket `itcoach-audio-upload`.<br>- Configure CORS policies on the audio bucket to support GET, PUT, POST, and DELETE methods from client browsers. | 06/10/2026 | 06/10/2026 | Internal Documents |
| Thu | - Create Amazon Cognito User Pool for user profile authentication.<br>- Configure Single-Page Application (SPA) Client `itcoach-web-client` supporting email logins, mandate user `name` attribute, and save pool IDs. | 06/11/2026 | 06/11/2026 | Internal Documents |
| Fri | - Create message queue system (Amazon SQS) for async speech processing.<br>- Setup Dead Letter Queue (`itcoach-dlq`) and main queue (`itcoach-processing-queue`) with 300s visibility timeout and maximum receives limit of 3. | 06/12/2026 | 06/12/2026 | Internal Documents |

### Week 8 Achievements:

* **System Design**: Finalized technical plans for ITCoach, detailing asynchronous voice evaluations using cost-efficient AWS Serverless patterns.
* **Security & Storage**: Successfully created IAM execution credentials restricting Lambda permissions and provisioned browser-accessible storage boundaries via S3 CORS.
* **Authentication Pool (Cognito)**: Configured active Cognito User Pools, providing secure registration and validation workflows.
* **Message Queuing (SQS)**: Implemented reliable message passing schemas using SQS queues backed by fault-tolerant DLQ setups.
