---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---
### Week 3 Objectives:

* Learn AWS Database Services including Amazon RDS (Relational), Amazon DynamoDB (NoSQL), and Amazon ElastiCache (In-memory caching).
* Deploy, secure, and connect applications to an Amazon RDS MySQL instance.
* Design schemas and optimize query performance using Amazon DynamoDB.
* Integrate ElastiCache (Redis) to accelerate application responses and reduce primary database load.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Learn Amazon RDS (Relational Database Service) core concepts<br>- Differentiate Multi-AZ deployments (high availability) vs Read Replicas (read optimization)<br>- Set up DB Subnet Groups for secure database networking | 05/04/2026 | 05/04/2026 | <https://000005.awsstudygroup.com/> |
| Tue | - Launch a MySQL DB Instance on Amazon RDS<br>- Configure Security Group to restrict access only from specific app/EC2 instances<br>- Connect client/application and practice DDL/DML statements<br>- Configure Automated Backups and manual DB Snapshots | 05/05/2026 | 05/05/2026 | <https://000005.awsstudygroup.com/> |
| Wed | - Learn NoSQL database concepts and Amazon DynamoDB features<br>- Design Primary Key schemas: Partition Key vs Composite Key (Partition Key + Sort Key)<br>- Differentiate Read/Write Capacity Modes: Provisioned (with Auto Scaling) vs On-Demand | 05/06/2026 | 05/06/2026 | <https://000060.awsstudygroup.com/> |
| Thu | - Create a DynamoDB table and perform CRUD operations (PutItem, GetItem, UpdateItem, DeleteItem)<br>- Compare data retrieval methods: Query vs Scan and their cost implications<br>- Create and configure Global Secondary Indexes (GSI) and Local Secondary Indexes (LSI) | 05/07/2026 | 05/07/2026 | <https://000060.awsstudygroup.com/> |
| Fri | - Learn Amazon ElastiCache and in-memory caching solutions<br>- Compare features and use cases between Redis and Memcached<br>- Create an ElastiCache Redis cluster and configure secure connections<br>- Integrate caching into applications to optimize response times | 05/08/2026 | 05/08/2026 | <https://000061.awsstudygroup.com/> |

### Week 3 Achievements:

* **Relational Database Administration with Amazon RDS:**
  * Successfully initialized a MySQL database with a Multi-AZ architecture ready for production.
  * Secured the database using DB Subnet Groups and Security Groups to isolate it from the public internet.
  * Mastered automated backups and point-in-time recovery processes.

* **NoSQL Database Design & Operations with DynamoDB:**
  * Designed schemas applying best practices for Partition Keys and Sort Keys to distribute data evenly.
  * Understood DynamoDB pricing models and configured On-Demand capacity mode to optimize cost for unpredictable workloads.
  * Mastered Query operations for high-efficiency data fetching instead of using Scan.
  * Configured Global Secondary Indexes (GSI) to enable flexible search conditions.

* **Performance Optimization with ElastiCache:**
  * Set up an ElastiCache Redis cluster as a transient cache layer.
  * Achieved sub-millisecond response times for cached queries and significantly reduced CPU load on the primary database.
