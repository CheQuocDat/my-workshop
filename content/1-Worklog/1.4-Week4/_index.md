---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---
### Week 4 Objectives:

* Explore serverless computing on AWS utilizing the core service AWS Lambda.
* Set up and manage secure API endpoints using Amazon API Gateway.
* Build and deploy serverless applications automatically with AWS SAM (Serverless Application Model).

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Learn Serverless architecture and Event-Driven execution patterns<br>- Introduce AWS Lambda, configuring Memory, Timeout, and IAM Execution Roles<br>- Write a basic Lambda function to process strings and JSON inputs | 05/11/2026 | 05/11/2026 | <https://000022.awsstudygroup.com/> |
| Tue | - Develop advanced Lambda functions interacting with S3 and DynamoDB via AWS SDK<br>- Configure Environment Variables for dynamic configuration management<br>- Test and debug Lambda functions using CloudWatch Logs | 05/12/2026 | 05/12/2026 | <https://000022.awsstudygroup.com/> |
| Wed | - Learn Amazon API Gateway concepts and service benefits<br>- Differentiate REST APIs vs HTTP APIs (high performance, low cost)<br>- Create an API and configure Resources and Methods (GET, POST, PUT, DELETE)<br>- Set up CORS (Cross-Origin Resource Sharing) to allow client integration | 05/13/2026 | 05/13/2026 | <https://000066.awsstudygroup.com/> |
| Thu | - Integrate API Gateway with Lambda using Lambda Proxy Integration<br>- Handle input parameters: Query String Parameters, Path Parameters, and Request Body<br>- Configure API Gateway Stages and deploy the API to Dev/Prod environments | 05/14/2026 | 05/14/2026 | <https://000066.awsstudygroup.com/> |
| Fri | - Install AWS SAM CLI in the local development environment<br>- Initialize a new SAM project and analyze the template.yaml configuration (AWS CloudFormation)<br>- Build and deploy the serverless application to AWS using the `sam deploy` command | 05/15/2026 | 05/15/2026 | <https://000080.awsstudygroup.com/> |

### Week 4 Achievements:

* **Serverless Programming with AWS Lambda:**
  * Understood event-driven mechanisms and how Lambda automatically scales based on requests.
  * Optimized Memory settings to balance execution speed and costs.
  * Mastered reading and debugging application issues using CloudWatch Logs.

* **API Gateway Design & Deployment:**
  * Deployed a functional HTTP API Gateway as the entry point for client requests.
  * Successfully configured CORS rules to block cross-site vulnerabilities.
  * Utilized Lambda Proxy Integration to forward request headers, path parameters, and query parameters directly to Lambda.

* **Automation with AWS SAM:**
  * Defined infrastructure (Lambda, API Gateway, DynamoDB) as code in `template.yaml`.
  * Standardized environments across local testing and cloud deployments with automated CI/CD-like workflows.
