---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---
### Week 5 Objectives:

* Implement identity management, registration, and user authentication using Amazon Cognito.
* Integrate JWT Token authentication to secure API Gateway endpoints.
* Build an Event-Driven Architecture utilizing Amazon SQS, Amazon SNS, and Amazon EventBridge to decouple system components.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Learn Amazon Cognito and the differences between User Pools and Identity Pools<br>- Create and configure a Cognito User Pool, setting up password policies and MFA<br>- Customize default hosted login UI and user verification emails | 05/18/2026 | 05/18/2026 | <https://000081.awsstudygroup.com/> |
| Tue | - Create a Cognito Identity Pool to grant temporary AWS credentials for S3/DynamoDB<br>- Integrate the Cognito SDK into a Frontend React application for sign-up and login flows<br>- Fetch and manage JWT Tokens (ID, Access, Refresh Tokens) on the client side | 05/19/2026 | 05/19/2026 | <https://000081.awsstudygroup.com/> |
| Wed | - Integrate Cognito Authorizers into API Gateway to secure HTTP/REST API endpoints<br>- Write a Lambda function to decode and verify JWT claims from request headers<br>- Test API authorization using Postman by passing the Authorization header | 05/20/2026 | 05/20/2026 | <https://000081.awsstudygroup.com/> |
| Thu | - Explore Event-Driven Architecture concepts and Amazon SQS message queuing<br>- Launch a Standard Queue and a FIFO Queue, understanding Visibility Timeouts<br>- Write Lambda code to send messages to the queue and configure Lambda triggers for consumer processing | 05/21/2026 | 05/21/2026 | <https://000077.awsstudygroup.com/> |
| Fri | - Learn Amazon SNS and the Publish/Subscribe (Pub/Sub) messaging model<br>- Create an SNS Topic, subscribing an SQS queue and an email address to receive notifications<br>- Study Amazon EventBridge, creating Scheduled Rules to trigger Lambda functions periodically | 05/22/2026 | 05/22/2026 | <https://000077.awsstudygroup.com/> |

### Week 5 Achievements:

* **Secure User Identity Management with Amazon Cognito:**
  * Successfully initialized a Cognito User Pool for centralized user database management with MFA options.
  * Integrated authentication flows into the React Frontend, securely managing JWT tokens under LocalStorage/SessionStorage.
  * Enforced authorization rules across API Gateway endpoints using Cognito Authorizers.

* **Decoupled Messaging and Event-Driven Orchestration:**
  * Leveraged Amazon SQS to act as a buffer for long-running workflows, improving system scalability and responsiveness.
  * Mastered the differences between Standard Queues (high throughput, best-effort ordering) and FIFO Queues (guaranteed ordering and deduplication).
  * Implemented SNS Pub/Sub patterns to fan out events from a single publisher to multiple subscribers simultaneously.
  * Created EventBridge Scheduled Rules to automate recurring administrative tasks (such as log cleanups and daily backups) via cron syntax.
