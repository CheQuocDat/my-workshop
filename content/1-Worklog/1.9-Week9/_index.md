---
title: "Week 9 Worklog"
date: 2026-07-06
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---
### Week 9 Objectives:

* Kickoff the graduate project ITCoach (AI-powered IT Interview & Training Platform).
* Design the Serverless architecture on AWS and allocate team roles.
* Set up the codebase repository and start design workflows.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Team meeting to align on project scope and ideas for ITCoach<br>- Design Amazon DynamoDB database schemas and tables | 06/15/2026 | 06/15/2026 | AWS Documentation |
| Tue | - Draw the global Serverless system architecture diagram<br>- Identify necessary AWS infrastructure components | 06/16/2026 | 06/16/2026 | AWS Architecture Center |
| Wed | - Allocate detailed tasks: Teammate builds AWS infrastructure (VPC, Cognito, S3, SQS, API Gateway, Route53, WAF); I design and develop Web App logic<br>- Define API endpoints and JSON request/response formats | 06/17/2026 | 06/17/2026 | API Design Best Practices |
| Thu | - Initialize Git repository and setup branch workflows (main, develop, features)<br>- Scaffold React/Vite web application locally | 06/18/2026 | 06/18/2026 | Vite & React Guides |
| Fri | - Design detailed code architecture for 8 Backend Lambda Functions<br>- Document software architecture specifications and data flow | 06/19/2026 | 06/19/2026 | Project Internal Docs |

### Week 9 Achievements:

* **Defined Graduate Project Objectives:**
  * Agreed on building ITCoach, an application supporting users to practice knowledge (Quizzes, Essays) and simulated mock interviews with AI.
  * Designed DynamoDB tables: `Users`, `Sessions`, `Questions`, `Answers`.

* **Completed System Architecture Design:**
  * Designed a complete serverless web application architecture: Client hosted on S3 and distributed via CloudFront.
  * APIs communicated through Amazon API Gateway, processing logic handled by AWS Lambda.
  * Integrated AI services: OpenAI API for answer grading, Amazon Polly for audio generation.
  * Asynchronous background tasks processed via Amazon SQS.
  * Role allocation established: My teammate was responsible for setting up and configuring the AWS infrastructure (CloudFront, API Gateway, S3, Cognito, SQS, KMS, WAF). I was in charge of developing the Web application (Frontend, Backend Lambda, AI Integration).

* **Set up Project Codebase:**
  * Created shared Git repository, configured branch rules and workflows.
  * Successfully initialized the Frontend React project with Vite + React + TypeScript.
  * Documented specifications for the 8 Backend Lambda Functions to ensure seamless API integration.
