---
title: "Week 12 Worklog"
date: 2026-07-06
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---
### Week 12 Objectives:

* End-to-end (E2E) integration, testing, and debugging.
* Import question bank data (Frontend, Backend, Cloud).
* Deploy the application to the AWS Production environment and deliver the final Demo.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Integrate my Frontend codebase with the AWS Infrastructure (CloudFront, WAF, API Gateway, S3) established by my teammate | 07/06/2026 | 07/06/2026 | AWS Integration Guide |
| Tue | - Perform End-to-End Testing: Register account -> Complete Quiz -> Write Essay & record answer -> AI evaluates -> Score displays on Dashboard | 07/07/2026 | 07/07/2026 | E2E Testing Strategies |
| Wed | - Populate the question bank with real-world questions (focusing on Frontend, Backend, DevOps, and AWS Cloud) | 07/08/2026 | 07/08/2026 | Internal Question Bank |
| Thu | - Debug issues (CORS, Lambda latency, audio format bugs on Safari/Chrome)<br>- Assist the team in deploying the app to the Production environment | 07/09/2026 | 07/09/2026 | Debugging & Deploy checklists |
| Fri | - Record a demo video showcasing the working ITCoach system<br>- Finalize the 12-week internship report and prepare the final presentation | 07/10/2026 | 07/10/2026 | Final Presentation Slides |

### Week 12 Achievements:

* **Successful System Integration and E2E Testing:**
  * Fully integrated the ITCoach platform: React Client securely connects to CloudFront protected by AWS WAF; API Gateway receives HTTP traffic and routes to appropriate AWS Lambda handlers.
  * E2E workflow succeeded: User registers -> takes quiz -> records speech for mock interview -> SQS triggers AI evaluation worker -> OpenAI evaluates -> dashboard updates.

* **High-Quality Question Bank Ingestion:**
  * Imported over 100 categorized questions covering Frontend, Backend, DevOps, and AWS Cloud architectures.

* **Production Deployment on AWS:**
  * App is live on custom domain with secure HTTPS.
  * Optimized Lambda Performance: Configured Provisioned Concurrency for core Lambda API handlers to eliminate cold starts, dropping latency from 5s to under 1s.
  * Solved Safari recording compatibility issues by outputting standard WAV files.

* **Completed Internship Program:**
  * Recorded demo video of the ITCoach product.
  * Prepared the final 12-week internship report, comprehensively demonstrating the learning phase (Weeks 1-8) and project development phase (Weeks 9-12).
