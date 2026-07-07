---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---
### Week 2 Objectives:

* Understand AWS Hosting & Storage services including Amazon S3, Amazon CloudFront, and Amazon Route 53.
* Deploy and host a secure static website on Amazon S3.
* Configure Amazon CloudFront CDN to optimize performance and reduce global latency.
* Manage DNS and custom domain routing using Amazon Route 53 with ACM SSL/TLS certificates.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Learn Amazon S3 (Simple Storage Service) basics<br>- Differentiate S3 Storage Classes (Standard, IA, Glacier)<br>- Study access control mechanisms: IAM Policies, Bucket Policies, and ACLs<br>- Set up default encryption configurations (SSE-S3, SSE-KMS) | 04/27/2026 | 04/27/2026 | <https://000057.awsstudygroup.com/> |
| Tue | - Enable S3 Static Website Hosting<br>- Upload static website assets and configure index/error documents (index.html, error.html)<br>- Setup public-read Bucket Policy securely<br>- Learn and configure CORS (Cross-Origin Resource Sharing) | 04/28/2026 | 04/28/2026 | <https://000057.awsstudygroup.com/> |
| Wed | - Learn Amazon CloudFront concepts including Edge Locations and Regional Edge Caches<br>- Create a CloudFront Distribution pointing to the S3 Bucket origin<br>- Configure Origin Access Control (OAC) to block direct public access to S3<br>- Set Cache Behaviors, TTLs, and auto-compression | 04/29/2026 | 04/29/2026 | <https://000094.awsstudygroup.com/> |
| Thu | - Learn Amazon Route 53 and DNS routing methods<br>- Create a Hosted Zone for a custom domain<br>- Configure basic DNS records (A, AAAA, CNAME, MX, TXT)<br>- Set up Routing Alias records pointing to the CloudFront Distribution | 04/30/2026 | 04/30/2026 | <https://000010.awsstudygroup.com/> |
| Fri | - Request free SSL/TLS certificates via AWS Certificate Manager (ACM)<br>- Perform domain ownership validation using DNS Validation<br>- Bind the ACM certificate to the CloudFront Distribution<br>- Configure HTTPS security policies and automatic HTTP-to-HTTPS redirect | 05/01/2026 | 05/01/2026 | <https://000094.awsstudygroup.com/> |

### Week 2 Achievements:

* **Mastered Amazon S3 Storage:**
  * Gained a solid understanding of Object Storage and storage classes to optimize cost.
  * Configured Lifecycle Policies to automatically transition or expire objects.
  * Mastered Bucket Policies and OAC to restrict S3 access only via CloudFront.

* **Successfully Deployed Static Website:**
  * Configured S3 Static Website Hosting to serve pages quickly and reliably.
  * Resolved CORS issues to allow safe cross-origin API calls.

* **Optimized Application Performance via CloudFront CDN:**
  * Established global content delivery network to serve static assets with low latency.
  * Understood Cache Keys, TTL, and Cache Invalidation mechanisms for immediate updates.

* **Managed DNS & Domain Security:**
  * Administered DNS Route 53 and mapped records accurately.
  * Successfully integrated HTTPS using ACM SSL/TLS certificates, ensuring end-user security and SEO compliance.
