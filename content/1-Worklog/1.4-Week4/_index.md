---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---


# Week 4 Worklog

## Week 4 Objectives

In week 4, the main goal was to explore the **Amazon Elastic Compute Cloud - EC2** service and its related components when deploying virtual servers on AWS. This week's content belongs to the **Explore / AWS Service Exploration** group, where the AWS Study Group covers deploying and optimizing compute services, including EC2, Auto Scaling, and supporting components for application operations. ([Cloud Journey][1])

Key topics for the week include:

* Getting an overview of Amazon EC2.
* Exploring AMI, Instance Type, Key Pair, and Security Group.
* Practicing launching a Linux EC2 Instance.
* Learning how to connect to EC2 via SSH.
* Learning how to change EC2 Instance configuration.
* Exploring Elastic Load Balancer and Auto Scaling Group.
* Noting common errors when deploying EC2.

---

## Tasks to be carried out this week

| No. | Task                                                                                                                                           | Start Date | Completion Date | Reference Material                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| --- | --- | --- | --- | --- |
| **1** | Get an overview of Amazon EC2 and its role in creating virtual servers and deploying applications on AWS.                                    | 05/11/2026 | 05/11/2026 | [https://cloudjourney.awsstudygroup.com/1-explore/](https://cloudjourney.awsstudygroup.com/1-explore/) <br> [https://000004.awsstudygroup.com/](https://000004.awsstudygroup.com/) <br> [https://000004.awsstudygroup.com/1-introduce/](https://000004.awsstudygroup.com/1-introduce/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **2** | Explore AMI, Instance Type, Key Pair, EBS, and Security Group when launching an EC2 Instance.                                                | 05/12/2026 | 05/12/2026 | [https://000004.awsstudygroup.com/1-introduce/](https://000004.awsstudygroup.com/1-introduce/) <br> [https://000004.awsstudygroup.com/2-prerequiste/2.3-createsecuritygrouplinux/](https://000004.awsstudygroup.com/2-prerequiste/2.3-createsecuritygrouplinux/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **3** | Practice creating a Linux EC2 Instance, choosing Amazon Linux 2023 AMI, and configuring Key Pair, VPC, Subnet, and Security Group.            | 05/13/2026 | 05/13/2026 | [https://000004.awsstudygroup.com/4-launchlinuxinstance/](https://000004.awsstudygroup.com/4-launchlinuxinstance/) <br> [https://000004.awsstudygroup.com/4-launchlinuxinstance/4.1-createlinuxinstance/](https://000004.awsstudygroup.com/4-launchlinuxinstance/4.1-createlinuxinstance/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **4** | Learn how to connect to a Linux EC2 Instance via SSH, check instance status, and handle common connection errors.                            | 05/14/2026 | 05/14/2026 | [https://000004.awsstudygroup.com/4-launchlinuxinstance/4.2-connectlinuxinstance/](https://000004.awsstudygroup.com/4-launchlinuxinstance/4.2-connectlinuxinstance/) <br> [https://000004.awsstudygroup.com/5-amazonec2basic/5.1-changeconfigureec2/](https://000004.awsstudygroup.com/5-amazonec2basic/5.1-changeconfigureec2/)                                                                                                                                                                                                                                                                                                                                                                                                       |
| **5** | Explore Load Balancer, Auto Scaling Group, EBS Snapshot, and clean up resources after practice to avoid unexpected costs.                    | 05/15/2026 | 05/15/2026 | [https://000006.awsstudygroup.com/](https://000006.awsstudygroup.com/) <br> [https://000006.awsstudygroup.com/4-setup-load-balancer/](https://000006.awsstudygroup.com/4-setup-load-balancer/) <br> [https://000006.awsstudygroup.com/6-create-auto-scaling-group/](https://000006.awsstudygroup.com/6-create-auto-scaling-group/) <br> [https://000004.awsstudygroup.com/5-amazonec2basic/5.2-createec2snapshot/](https://000004.awsstudygroup.com/5-amazonec2basic/5.2-createec2snapshot/)                                                                                                                                                                                                                                                       |

---

## Week 4 Achievements

### Overview

This week, I explored **Amazon EC2**, the core virtual server service of AWS. Amazon EC2 lets you launch virtual servers quickly, choose a configuration to fit your needs, and deploy many types of workloads such as websites, applications, databases, or backend services. ([Aws Study Group][2])

### Knowledge gained

After completing week 4, I have understood:

* The role of **Amazon EC2** in providing compute resources on AWS.
* The concept of **AMI - Amazon Machine Image**, used as a template to launch an EC2 Instance.
* That **Instance Type** affects the CPU, RAM, network, and storage of the virtual server.
* That **Key Pair** is used to authenticate when connecting to an EC2 Instance, and the private key must be protected carefully. ([Aws Study Group][3])
* How to configure a **Security Group** to control inbound and outbound traffic to the EC2 Instance.
* The role of **EBS Snapshot** in backing up data and recovering the system. ([Aws Study Group][4])
* The basics of **Elastic Load Balancer** and **Auto Scaling Group** in distributing load and automatically scaling the number of instances. ([Aws Study Group][5])

### Practice

During the learning and practice process, I was able to:

* Access the EC2 service on the AWS Management Console.
* Learn the EC2 Instance creation process.
* Choose Amazon Linux 2023 AMI when launching a virtual server.
* Configure Instance Type, Key Pair, VPC, Subnet, and Security Group.
* Set up Security Group rules, including SSH, HTTP, and HTTPS.
* Connect to the Linux EC2 Instance via SSH.
* Check the operational status of the instance.
* Learn how to change the EC2 Instance Type to upgrade resources when needed.
* Learn the EBS Snapshot creation process to back up data.
* Explore Load Balancer and Auto Scaling Group to improve availability, scalability, and operational efficiency.
* Note common errors such as unopened port 22, wrong key pair, instance without a public IP, wrong subnet, or a security group that does not allow access.

---

## Week 4 Summary

**Week 4:** Explore EC2, AMI, Instance Type, Key Pair, Security Group, EBS Snapshot, Load Balancer, and Auto Scaling. Understand how to launch a virtual server, connect to an EC2 Instance, configure access security, and explore the system scaling mechanism on AWS.

[1]: https://cloudjourney.awsstudygroup.com/1-explore/ "Explore AWS Services :: First Journey to the Cloud"
[2]: https://000004.awsstudygroup.com/1-introduce/ "Introduction :: INTRODUCTION TO AMAZON EC2"
[3]: https://000004.awsstudygroup.com/4-launchlinuxinstance/4.1-createlinuxinstance/ "Create Linux instance :: INTRODUCTION TO AMAZON EC2"
[4]: https://000004.awsstudygroup.com/5-amazonec2basic/5.2-createec2snapshot/ "Create and manage EBS Snapshots :: INTRODUCTION TO AMAZON EC2"
[5]: https://000006.awsstudygroup.com/ "Deploying FCJ Management application with Auto Scaling Group :: DEPLOYING FCJ MANAGEMENT APPLICATION WITH AUTO SCALING GROUP"
