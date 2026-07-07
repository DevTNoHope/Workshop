---
title: "Week 9 Worklog"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Deploy DynamoDB databases consisting of 8 tables using On-demand capacity and Global Secondary Indexes (GSIs).
* Develop and deploy core Lambda Functions managing authentication, question lookups, interview sessions, and answer submissions.
* Write AI evaluation Lambda logic, configure application environment variables, and establish SQS message triggers.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Provision 8 DynamoDB tables: `users`, `questions`, `sessions`, `answers`, `history`, `topics`, `quiz-attempts`, and `gamification`.<br>- Configure GSIs: `category-index`, `userId-index`, `sessionId-index`, and `xp-index` for subkey querying. | 06/15/2026 | 06/15/2026 | ITCoach Manual |
| Tue | - Write and deploy `itcoach-auth-handler` to manage user profiles.<br>- Write `itcoach-question-handler` to fetch essay questions filtered by specialty (Frontend, Backend, DevOps...) and topics. | 06/16/2026 | 06/16/2026 | ITCoach Manual |
| Wed | - Build `itcoach-session-handler` to initialize Mock Interview sessions, matching question banks by level/duration.<br>- Build `itcoach-answer-handler` to save records and generate S3 Presigned URLs for client voice uploads. | 06/17/2026 | 06/17/2026 | ITCoach Manual |
| Thu | - Develop `itcoach-ai-processor` for heavy tasks: OpenAI STT (transcribe audio), OpenAI GPT (evaluate responses), and Polly TTS (vocalize responses).<br>- Configure environment variables for S3 buckets, table names, and OpenAI keys. | 06/18/2026 | 06/18/2026 | ITCoach Manual |
| Fri | - Write secondary helper Lambda functions: `itcoach-result-handler` (dashboard stats), `itcoach-quiz-handler` (spaced repetition SM-2 engine), and `itcoach-gamification-handler` (leaderboard rankings).<br>- Attach SQS queue trigger to `itcoach-ai-processor` Lambda. | 06/19/2026 | 06/19/2026 | ITCoach Manual |

### Week 9 Achievements:

* **Database Provisioning (DynamoDB)**: Deployed 8 On-demand tables successfully and verified low-latency index querying for dashboard statistics and leaderboard displays.
* **Serverless Backend Logic**: Deployed 8 Python 3.12 Lambda handlers using custom execution roles with fine-tuned execution timeouts and memory settings.
* **Asynchronous Integration**: Successfully configured secure credentials via environment variables and bound SQS triggers to invoke AI processing queues when client audios are uploaded.
