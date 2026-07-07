---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---
### Week 6 Objectives:

* Deploy advanced security solutions on AWS to protect web applications from online threats using AWS WAF.
* Manage data encryption centrally with AWS KMS and secure sensitive configuration credentials using AWS Secrets Manager.
* Integrate intelligent threat detection via AWS GuardDuty and manage servers securely without SSH key dependencies using Systems Manager Session Manager.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Learn AWS WAF (Web Application Firewall) concepts: Web ACLs, Rules, and Rule Groups<br>- Create a Web ACL, associating it with a CloudFront Distribution or Application Load Balancer<br>- Configure basic rules to block SQL Injection, Cross-Site Scripting (XSS), and malicious IPs | 05/25/2026 | 05/25/2026 | <https://000026.awsstudygroup.com/> |
| Tue | - Study encryption mechanisms of AWS KMS (Key Management Service) and differentiate AWS Managed Keys vs Customer Managed Keys (CMK)<br>- Create a CMK, configuring its Key Policy to authorize administrators and users<br>- Practice encrypting and decrypting S3 Bucket and EBS Volume data using KMS keys | 05/26/2026 | 05/26/2026 | <https://000033.awsstudygroup.com/> |
| Wed | - Research secrets management using AWS Secrets Manager<br>- Create and store sensitive database connection credentials (username, password, endpoint)<br>- Write Lambda code calling Secrets Manager APIs to fetch credentials dynamically at runtime<br>- Configure automatic credentials rotation policies | 05/27/2026 | 05/27/2026 | <https://000096.awsstudygroup.com/> |
| Thu | - Enable AWS GuardDuty for continuous security monitoring of the AWS account<br>- Learn how GuardDuty analyzes VPC Flow Logs, DNS Logs, and CloudTrail Events<br>- Simulate security threat scenarios to analyze GuardDuty alerts (Findings) | 05/28/2026 | 05/28/2026 | <https://000098.awsstudygroup.com/> |
| Fri | - Learn AWS Systems Manager (SSM) and its Session Manager capability<br>- Configure an IAM instance profile for an EC2 instance with AWS Systems Manager Agent (SSM Agent) enabled<br>- Connect to the EC2 terminal securely via AWS Console without opening port 22 or managing SSH Key pairs | 05/29/2026 | 05/29/2026 | <https://000058.awsstudygroup.com/> |

### Week 6 Achievements:

* **Enhanced Application Security with AWS WAF:**
  * Protected application deployments successfully against OWASP Top 10 vulnerabilities.
  * Configured rate-based rules to mitigate basic Distributed Denial of Service (DDoS) attempts.

* **Centralized Encryption Key Management via KMS:**
  * Enforced encryption at rest policies across vital S3 storage buckets and EBS volumes.
  * Controlled key access boundaries securely using Key Policies combined with IAM policies.

* **Secure Credentials Lifecycle Management via Secrets Manager:**
  * Cleaned up database credentials from application source code files, eliminating hardcoded variables.
  * Configured automatic secrets rotation to regularly refresh database credentials without downtime.

* **Proactive Security Audits and Host Access Governance:**
  * Utilized GuardDuty to discover compromised credentials, anomalous user patterns, or unauthorized activities early.
  * Adopted Session Manager for host access, completely removing the attack surface of open port 22 and the operational overhead of PEM files.
