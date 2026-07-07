---
title: "Week 10 Worklog"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Configure Amazon API Gateway, bind Cognito Authorizers, and deploy 8 operational REST endpoints.
* Bootstrap the Frontend client application using ReactJS & TypeScript and integrate Cognito identity SDKs.
* Develop Client Dashboards, Quiz evaluation components, and standard essay input interfaces.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Initialize REST API on Amazon API Gateway (`itcoach-api`).<br>- Configure Cognito Authorizer (`itcoach-cognito-auth`) linking it to the User Pool and set token source to the `Authorization` header. | 06/22/2026 | 06/22/2026 | ITCoach Manual |
| Tue | - Set up the 8 resources and methods (GET/POST) integrated with their respective Lambda handlers.<br>- Enable CORS for all resource endpoints and deploy the API to stage `prod` to copy invoke URL. | 06/23/2026 | 06/23/2026 | ITCoach Manual |
| Wed | - Initialize Client Frontend codebase using ReactJS, TypeScript, and TailwindCSS.<br>- Integrate AWS Cognito SDK to authenticate registrations, logins, and retrieve ID tokens for API headers. | 06/24/2026 | 06/24/2026 | ITCoach Manual |
| Thu | - Develop the personal student Dashboard: visualize progress stats, topic completion rates, study streaks, and gamified XP tables. | 06/25/2026 | 06/25/2026 | ITCoach Manual |
| Fri | - Develop the Quiz workspace supporting single/multi-select answers and point calculation.<br>- Create the basic Essay workspace providing text input editing and direct audio recording buttons. | 06/26/2026 | 06/26/2026 | ITCoach Manual |

### Week 10 Achievements:

* **API Gateway Routing**: Implemented centralized REST endpoints secured behind active Cognito Authorizers, protecting operational methods from unauthorized queries.
* **Frontend Infrastructure**: Set up a clean ReactJS + TypeScript template, linking Client login operations with AWS Cognito identity stores.
* **Study Modules**: Completed core client pages: interactive student dashboards, automated quiz scoring with XP rewards, and clean text/audio essay inputs.
