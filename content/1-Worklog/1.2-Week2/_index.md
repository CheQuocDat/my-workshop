---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---
### Week 2 Objectives:

* Start with Amazon VPC and AWS VPN Site-to-Site.
* Learn and practice creating VPC, Security Groups, VPN Connection.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Mon | - Learn VPC (Virtual Private Cloud) basics<br>- Understand CIDR blocks, Subnets (Public/Private)<br>- Learn about Internet Gateway and NAT Gateway<br>- Create VPC with multi-AZ architecture | 04/28/2026 | 04/28/2026 | <https://000003.awsstudygroup.com/> |
| Tue | - Learn Security Groups and Network ACLs<br>- Differentiate Stateful vs Stateless firewall<br>- Configure inbound/outbound rules<br>- Practice creating Security Groups for EC2 | 04/29/2026 | 04/29/2026 | <https://000003.awsstudygroup.com/> |
| Wed | - Learn Route Tables and routing<br>- Configure VPC Flow Logs<br>- Setup CloudWatch monitoring for VPC<br>- Use VPC Resource Map for visualization | 04/30/2026 | 04/30/2026 | <https://000003.awsstudygroup.com/> |
| Thu | - Learn AWS Site-to-Site VPN<br>- Create Virtual Private Gateway and Customer Gateway<br>- Configure VPN Connection<br>- Test VPN connectivity | 05/01/2026 | 05/01/2026 | <https://000003.awsstudygroup.com/> |
| Fri | - Learn AWS Transit Gateway<br>- Connect multiple VPCs via Transit Gateway<br>- Configure VPN with strongSwan<br>- Route traffic through Transit Gateway | 05/02/2026 | 05/02/2026 | <https://000003.awsstudygroup.com/> |

### Week 2 Achievements:

* Understood Amazon VPC (Virtual Private Cloud) architecture and network resource isolation on AWS:
  * CIDR notation and IP address planning
  * Multi-AZ deployment for high availability
  * Public Subnets with Internet Gateway (IGW) for Internet access
  * Private Subnets with NAT Gateway for outbound traffic
  * Route Tables and routing priority (longest prefix matching)
  * VPC peering and VPC endpoints

* Mastered Network Security with Security Groups and Network ACLs:
  * Security Groups - stateful firewall at EC2 instance level
  * Network ACLs - stateless firewall at subnet level
  * Configured inbound rules (SSH, HTTP, HTTPS) and outbound rules
  * Rule numbering and evaluation order
  * Security group chaining and references
  * Deny rules to blacklist IPs

* Deployed VPC Monitoring and Troubleshooting:
  * VPC Flow Logs to capture IP traffic information
  * Published logs to CloudWatch Logs or S3
  * Created CloudWatch dashboards to visualize VPC resources
  * Set up alarms for traffic anomalies
  * Analyzed traffic patterns and troubleshot connectivity
  * Identified security threats and unusual traffic
  * Used VPC Resource Map for visualization

* Connected on-premises with AWS via VPN Solutions:
  * Site-to-Site VPN with Virtual Private Gateway (VGW) and Customer Gateway (CGW)
  * Established IPsec VPN tunnel between on-premises and AWS VPC
  * Static routing vs Dynamic routing (BGP)
  * AWS Transit Gateway - hub-and-spoke architecture for multi-VPC connectivity
  * Transit Gateway attachments (VPC, VPN, Direct Connect)
  * Transit Gateway route tables
  * Configured strongSwan VPN (open-source IPsec) on Linux EC2 instance
  * VPN monitoring and troubleshooting
  * VPN high availability patterns
