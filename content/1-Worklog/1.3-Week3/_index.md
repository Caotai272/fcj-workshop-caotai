---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---


# Week 3 Worklog

## Week 3 Objectives

In week 3, the main goal was to explore **Amazon Virtual Private Cloud - Amazon VPC** and the basic networking components on AWS. This service is used to build a private network environment, helping deploy AWS resources such as EC2, databases, or backend services within a controlled network system.

This week's content belongs to the **Explore / AWS Service Exploration** group, where the AWS Study Group covers VPC network architecture and AWS network infrastructure design patterns. ([cloudjourney.awsstudygroup.com][1]) The Amazon VPC workshop also focuses on designing, deploying, and managing a private network environment on AWS Cloud. ([000003.awsstudygroup.com][2])

Key topics for the week include:

* Getting an overview of Amazon VPC.
* Exploring Subnet, Route Table, Internet Gateway, and NAT Gateway.
* Distinguishing Public Subnet and Private Subnet.
* Exploring Security Group and Network ACL.
* Practicing creating VPC, Subnet, Internet Gateway, Route Table, and Security Group.
* Noting common errors when configuring networking on AWS.

---

## Tasks to be carried out this week

| No. | Task                                                                                                                                          | Start Date | Completion Date | Reference Material                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| --- | --- | --- | --- | --- |
| **1** | Get an overview of Amazon VPC and its role in creating a private network environment on AWS Cloud.                                            | 05/04/2026 | 05/04/2026 | [https://cloudjourney.awsstudygroup.com/1-explore/](https://cloudjourney.awsstudygroup.com/1-explore/) <br> [https://000003.awsstudygroup.com/](https://000003.awsstudygroup.com/) <br> [https://000003.awsstudygroup.com/1-introduce/](https://000003.awsstudygroup.com/1-introduce/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **2** | Explore Subnet and Route Table, distinguish Public Subnet, Private Subnet, and how traffic is routed within the VPC.                          | 05/05/2026 | 05/05/2026 | [https://000003.awsstudygroup.com/1-introduce/1.1-subnets/](https://000003.awsstudygroup.com/1-introduce/1.1-subnets/) <br> [https://000003.awsstudygroup.com/1-introduce/1.2-routetable/](https://000003.awsstudygroup.com/1-introduce/1.2-routetable/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **3** | Explore Internet Gateway and NAT Gateway, and the role of each component in connecting AWS resources to the Internet.                         | 05/06/2026 | 05/06/2026 | [https://000003.awsstudygroup.com/1-introduce/1.3-internetgateway/](https://000003.awsstudygroup.com/1-introduce/1.3-internetgateway/) <br> [https://000003.awsstudygroup.com/1-introduce/1.4-natgateway/](https://000003.awsstudygroup.com/1-introduce/1.4-natgateway/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **4** | Explore the firewall in VPC, Security Group and Network ACL, to control inbound/outbound traffic to AWS resources.                            | 05/07/2026 | 05/07/2026 | [https://000003.awsstudygroup.com/2-firewallinvpc/](https://000003.awsstudygroup.com/2-firewallinvpc/) <br> [https://000003.awsstudygroup.com/2-firewallinvpc/2.1-securitygroup/](https://000003.awsstudygroup.com/2-firewallinvpc/2.1-securitygroup/) <br> [https://000003.awsstudygroup.com/2-firewallinvpc/2.2-networkacls/](https://000003.awsstudygroup.com/2-firewallinvpc/2.2-networkacls/)                                                                                                                                                                                                                                                                                                                                                               |
| **5** | Practice creating VPC, Subnet, Internet Gateway, Route Table, and Security Group; review the network model and note common configuration errors. | 05/08/2026 | 05/08/2026 | [https://000003.awsstudygroup.com/3-prerequisite/3.1-createvpc/](https://000003.awsstudygroup.com/3-prerequisite/3.1-createvpc/) <br> [https://000003.awsstudygroup.com/3-prerequisite/3.2-createsubnet/](https://000003.awsstudygroup.com/3-prerequisite/3.2-createsubnet/) <br> [https://000003.awsstudygroup.com/3-prerequisite/3.3-createigw/](https://000003.awsstudygroup.com/3-prerequisite/3.3-createigw/) <br> [https://000003.awsstudygroup.com/3-prerequisite/3.4-createroutetable/](https://000003.awsstudygroup.com/3-prerequisite/3.4-createroutetable/) <br> [https://000003.awsstudygroup.com/3-prerequisite/3.5-createsecuritygroup/](https://000003.awsstudygroup.com/3-prerequisite/3.5-createsecuritygroup/) |

---

## Week 3 Achievements

### Overview

This week, I explored **Amazon VPC** and the key networking components when deploying systems on AWS. Amazon VPC lets you create an isolated virtual network environment in AWS Cloud, where you can customize the IP address range, divide subnets, and configure routing according to your deployment needs. ([000003.awsstudygroup.com][3])

### Knowledge gained

After completing week 3, I have understood:

* The role of **Amazon VPC** in AWS infrastructure architecture.
* How to distinguish **Public Subnet** and **Private Subnet**.
* The role of the **Route Table** in directing network traffic.
* That the **Internet Gateway** lets resources in the public subnet connect to the Internet.
* That the **NAT Gateway** lets resources in the private subnet access the Internet outbound.
* The difference between **Security Group** and **Network ACL**.
* The basic process to create a VPC, subnet, route table, internet gateway, and security group.

### Practice

During the learning and practice process, I was able to:

* Access the VPC service on the AWS Management Console.
* Explore the structure of a basic VPC.
* Practice creating a VPC with an appropriate CIDR range.
* Create a public subnet and a private subnet.
* Create an Internet Gateway and attach it to the VPC.
* Configure the Route Table for the public subnet.
* Create a Security Group to control access.
* Note common errors such as missing route to the Internet, unattached Internet Gateway, misconfigured Security Group, or unopened required ports.

---

## Week 3 Summary

**Week 3:** Explore VPC, Subnet, Route Table, Internet Gateway, NAT Gateway, Security Group, and Network ACL. Understand how to build a basic network model on AWS, divide public/private subnets, and control traffic with network security components.

[1]: https://cloudjourney.awsstudygroup.com/1-explore/ "Explore AWS Services :: First Journey to the Cloud"
[2]: https://000003.awsstudygroup.com/ "Getting Started with Amazon Virtual Private Cloud (VPC) and AWS Site-to-Site VPN :: Getting Started with Amazon VPC and AWS VPN Site to Site"
[3]: https://000003.awsstudygroup.com/1-introduce/ "Introduction :: Getting Started with Amazon VPC and AWS VPN Site to Site"
