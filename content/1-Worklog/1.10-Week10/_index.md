---
title: "Week 10 Worklog"
date: 2026-07-06
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---
### Week 10 Objectives:

* Develop Backend source code (8 AWS Lambda Functions) to handle core logic and integrate AI services (OpenAI API, Amazon Polly).
* Construct the basic Frontend user interface (Authentication, Quiz, Essay, and Audio Recording pages).

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Write Lambda Functions for the Quiz system (Quiz API: fetch questions, submit scores)<br>- Develop Lambda Functions to handle Authentication via Amazon Cognito | 06/22/2026 | 06/22/2026 | Node.js & AWS SDK |
| Tue | - Write 2 core Lambda Functions for Essays (Essay API) and starting new mock interview sessions (Mock Interview Session API)<br>- Setup database connection configurations to DynamoDB | 06/23/2026 | 06/23/2026 | DynamoDB DocumentClient |
| Wed | - Integrate OpenAI API into the Lambda Worker to automate grading and feedback generation for essays<br>- Integrate Amazon Polly (TTS) to generate question audios, save to S3, and sign Presigned URLs | 06/24/2026 | 06/24/2026 | OpenAI Docs & Amazon Polly Guide |
| Thu | - Build basic Frontend UI: Login/Register page (integrated Cognito SDK) and Quiz workspace layout (Quiz UI)<br>- Scaffold React component structures | 06/25/2026 | 06/25/2026 | React UI & Cognito SDK |
| Fri | - Develop Essay UI workspace with direct in-browser voice recording capabilities<br>- Perform local testing of Lambda APIs using AWS SAM / LocalStack | 06/26/2026 | 06/27/2026 | Web Audio API |

### Week 10 Achievements:

* **Completed Backend Development with 8 Lambda Functions:**
  * `auth-handler`: Handles user registration, login, and token-based authorization.
  * `quiz-get-questions`: Fetches categorized quiz questions from database.
  * `quiz-submit-answers`: Evaluates and persists user quiz answers.
  * `essay-get-questions`: Retrieves essay questions bank.
  * `essay-submit-answers`: Submits user essays and triggers evaluations.
  * `interview-session-start`: Initializes mock interview sessions and invokes Amazon Polly for speech generation.
  * `interview-audio-handler`: Handles user recording uploads to S3 via Presigned URLs.
  * `ai-evaluation-worker`: Background worker listening to SQS to process essays/audio through OpenAI API and updates DynamoDB.

* **Successfully Integrated AI & Voice Services:**
  * **Amazon Polly:** Generated high-quality `.mp3` audio files to simulate an interactive interviewer voice.
  * **OpenAI (GPT-4o):** Acted as a virtual IT Coach, analyzing technical vocabulary, grammar, and answering correctness, returning bilingual feedback (English & Vietnamese).

* **Constructed Basic Frontend UI Foundation:**
  * Finished Cognito-integrated Login/Register workflows.
  * Designed clean quiz page layouts with timers and interactive choices.
  * Successfully set up Web Audio API to record user answers from microphone.
