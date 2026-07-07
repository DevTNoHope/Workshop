---
title: "Week 11 Work Log"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Develop interactive Mock Interview Rooms with real-time browser recording interfaces.
* Implement direct client S3 audio uploads using S3 Presigned URLs with SQS event notification.
* Integrate AI services: speech translation (OpenAI STT), grading evaluation (OpenAI GPT), and vocal synthesis (Amazon Polly).

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Design Mock Interview Room client setup (Specialty, Level, Duration config).<br>- Integrate browser MediaRecorder API to record user responses via local microphone. | 06/29/2026 | 06/29/2026 | ITCoach Manual |
| Tue | - Invoke S3 Presigned URL fetch from backend Lambda `itcoach-answer-handler`.<br>- Code frontend helper to upload recorded audio files (`.webm`/`.mp3`) to S3 `itcoach-audio-upload` bucket and trigger SQS. | 06/30/2026 | 06/30/2026 | ITCoach Manual |
| Wed | - Integrate OpenAI Whisper API in `itcoach-ai-processor` Lambda to transcribe S3 audios into text.<br>- Build GPT-4o evaluation engine checking responses against criteria database, grading scores, and listing missing points. | 07/01/2026 | 07/01/2026 | ITCoach Manual |
| Thu | - Configure Amazon Polly Text-to-Speech inside Lambda to synthesize GPT's comments and next questions into voice files.<br>- Upload Polly audios to S3, pass URLs to Client, and play them on the client interface. | 07/02/2026 | 07/02/2026 | ITCoach Manual |
| Fri | - Develop the Mock Interview Feedback Dashboard: display aggregate scores, skill breakdowns, sample responses, and study recommendations. | 07/03/2026 | 07/03/2026 | ITCoach Manual |

### Week 11 Achievements:

* **Voice Capture & Upload**: Successfully implemented client-side recording, securing audio ingestion directly into S3 private buckets using time-limited Presigned URLs.
* **Natural Language Analysis**: Embedded AI processing in Lambda to accurately convert spoken responses into text, score technical arguments, and verify mandatory points.
* **Vocal Feedback (Polly TTS)**: Integrated lifelike Polly artificial voices, serving next questions back to the client browser to simulate real interviewer interaction.
* **Detailed Feedback Dashboard**: Completed mock interview statistics dashboards, pointing out missing conceptual arguments and next study steps.
