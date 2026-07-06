---
title: "Week 1 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---
### Week 1 Objectives:

* Managing Access Control with AWS IAM (Identity and Access Management).
* Learn and practice creating Users, Groups, Roles and Switch Role.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Get acquainted with FCAJ members<br>- Read and note internship unit rules and regulations<br>- Learn about AWS and service types (Compute, Storage, Networking, Database) | 04/20/2026 | 04/20/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Tue | - Create AWS Free Tier account<br>- Complete 5 tasks to get $100 AWS Credit<br>- Set up MFA (Multi-Factor Authentication)<br>- Learn AWS Budgets for cost management | 04/21/2026 | 04/21/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Wed | - Learn about IAM Users and Groups<br>- Create IAM Admin User and Admin Group<br>- Attach AdministratorAccess policy to Admin Group<br>- Login with IAM Admin User | 04/22/2026 | 04/22/2026 | <https://000002.awsstudygroup.com/> |
| Thu | - Learn about IAM Roles and usage<br>- Create IAM Roles (AdminRole, S3Role)<br>- Create Operator User and attach policy for role switching | 04/23/2026 | 04/23/2026 | <https://000002.awsstudygroup.com/> |
| Fri | - Practice Switch Role from Operator User to Admin Role<br>- Check S3 access with S3Role<br>- Apply principle of least privilege | 04/24/2026 | 04/24/2026 | <https://000002.awsstudygroup.com/> |

### Week 1 Achievements:

* Successfully integrated with First Cloud AI Journey team and understood internship unit rules and regulations.

* Understood what AWS is and mastered the basic service groups:
  * Compute (EC2, Lambda, ECS, EKS)
  * Storage (S3, EBS, EFS, Glacier)
  * Networking (VPC, Route53, CloudFront, Direct Connect)
  * Database (RDS, DynamoDB, Aurora, Redshift)
  * Security & Identity (IAM, KMS, WAF, Shield)

* Successfully created and configured AWS Free Tier account:
  * Completed 5 tasks to receive $100 AWS Credit
  * Set up MFA (Multi-Factor Authentication) for root account
  * Configured AWS Budgets with cost alert thresholds

* Mastered access management with AWS IAM (Identity and Access Management):
  * Understood difference between IAM Users (long-term credentials) and IAM Roles (temporary permissions)
  * Created Admin Group with AdministratorAccess policy
  * Created IAM Admin User and added to Admin Group
  * Created AdminRole with full admin permissions and S3Role with Read/Write S3 access
  * Created Operator User and configured policy to allow role switching
  * Successfully practiced Switch Role from Operator User to Admin Role
  * Logged into AWS Console with IAM User instead of root account

* Applied IAM Best Practices:
  * Principle of least privilege
  * Use Roles for temporary access instead of shared credentials
  * Enable MFA for critical IAM Users
  * Monitor access activities via AWS CloudTrail
  * Avoid using root account for daily tasks
