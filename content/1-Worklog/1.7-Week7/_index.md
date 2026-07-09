---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---


# Week 7 Worklog

## Week 7 Objectives

In week 7, the main goal was to explore AWS database services: **Amazon RDS** and **Amazon DynamoDB**. These are two important services for storing, managing, and querying data in a system. Amazon RDS fits relational databases such as MySQL, PostgreSQL, MariaDB, Oracle, and SQL Server, while DynamoDB is a fully managed NoSQL database service on AWS. This content belongs to the **Explore / AWS Service Exploration** group, where the AWS Study Group introduces RDS and DynamoDB as foundational services when learning AWS. ([Cloud Journey][1])

Key topics for the week include:

* Getting an overview of databases on AWS.
* Exploring **Amazon RDS** and how to create a relational database.
* Exploring backup, snapshot, restore, Multi-AZ, and Read Replica in RDS.
* Exploring **Amazon DynamoDB** and the NoSQL database model.
* Exploring AWS Backup for backing up and restoring data.
* Comparing RDS and DynamoDB by use case.

---

## Tasks to be carried out this week

| No. | Task                                                                                                                                            | Start Date | Completion Date | Reference Material                                                                                                                                                                                                                                                                                                                                                                       |
| --- | --- | --- | --- | --- |
| **1** | Get an overview of databases on AWS, distinguish relational and NoSQL databases, and decide when to use RDS vs DynamoDB.                        | 06/01/2026 | 06/01/2026 | [https://cloudjourney.awsstudygroup.com/1-explore/](https://cloudjourney.awsstudygroup.com/1-explore/) <br> [https://000005.awsstudygroup.com/](https://000005.awsstudygroup.com/) <br> [https://000053.awsstudygroup.com/](https://000053.awsstudygroup.com/)                                                                                                                                                         |
| **2** | Explore Amazon RDS and concepts such as DB Instance, DB Engine, endpoint, storage, security group, and how applications connect to the database. | 06/02/2026 | 06/02/2026 | [https://000005.awsstudygroup.com/](https://000005.awsstudygroup.com/) <br> [https://000005.awsstudygroup.com/1-introduce/](https://000005.awsstudygroup.com/1-introduce/)                                                                                                                                                                                                             |
| **3** | Explore backup, DB Snapshot, restore, Multi-AZ, and Read Replica in Amazon RDS to improve data safety and system availability.                  | 06/03/2026 | 06/03/2026 | [https://000005.awsstudygroup.com/1-introduce/](https://000005.awsstudygroup.com/1-introduce/)                                                                                                                                                                                                                                                           |
| **4** | Explore Amazon DynamoDB, the NoSQL model, Table, Item, Partition Key, Sort Key, Query, Scan, and how DynamoDB stores data.                      | 06/04/2026 | 06/04/2026 | [https://000053.awsstudygroup.com/](https://000053.awsstudygroup.com/) <br> [https://000053.awsstudygroup.com/1-introduction/](https://000053.awsstudygroup.com/1-introduction/) <br> [https://000055.awsstudygroup.com/3-create-single-page-app/3.1-create-dynamodb-table/](https://000055.awsstudygroup.com/3-create-single-page-app/3.1-create-dynamodb-table/) |
| **5** | Explore AWS Backup, backup vault, backup plan, resource assignment, and how to back up and restore resources like RDS Database, DynamoDB Table, EBS, and EFS. | 06/05/2026 | 06/05/2026 | [https://000013.awsstudygroup.com/](https://000013.awsstudygroup.com/) <br> [https://000013.awsstudygroup.com/1-introduce/](https://000013.awsstudygroup.com/1-introduce/) <br> [https://000039.awsstudygroup.com/1-lhol/1.4/1.4.1/](https://000039.awsstudygroup.com/1-lhol/1.4/1.4.1/)                                                                           |
| **6** | Consolidate knowledge, compare Amazon RDS and DynamoDB, and note cautions about security, backup, restore, cost, and cleaning up resources after practice. | 06/06/2026 | 06/06/2026 | [https://cloudjourney.awsstudygroup.com/1-explore/](https://cloudjourney.awsstudygroup.com/1-explore/) <br> [https://000005.awsstudygroup.com/](https://000005.awsstudygroup.com/) <br> [https://000053.awsstudygroup.com/](https://000053.awsstudygroup.com/) <br> [https://000013.awsstudygroup.com/](https://000013.awsstudygroup.com/)                   |

---

## Week 7 Achievements

### Overview

This week, I explored two popular database groups on AWS: **Amazon RDS** and **Amazon DynamoDB**. Amazon RDS supports deploying a managed relational database, while Amazon DynamoDB is a fully managed NoSQL service, suitable for systems needing flexible scaling and stable performance. ([000005.awsstudygroup.com][2])

### Knowledge gained

After completing week 7, I have understood:

* The role of databases in systems deployed on AWS.
* The difference between **Relational Database** and **NoSQL Database**.
* That **Amazon RDS** is used to deploy relational database engines such as MySQL, PostgreSQL, MariaDB, Oracle, or SQL Server.
* The basic RDS components: **DB Instance**, **DB Engine**, **Endpoint**, **Storage**, **Security Group**, and **Backup**.
* That a **DB Snapshot** in RDS backs up the database at a specific point in time and can be restored into a new DB Instance. ([000005.awsstudygroup.com][3])
* That **Multi-AZ** improves RDS availability, while **Read Replica** helps offload read queries from the database. ([000005.awsstudygroup.com][2])
* That **Amazon DynamoDB** is a fully managed NoSQL database where you can create tables, store items, and query data by key.
* That **AWS Backup** can centralize and automate backups of resources such as EBS, RDS, DynamoDB, and EFS. ([Aws Study Group][4])

### Practice

During the learning and practice process, I was able to:

* Access the Amazon RDS service on the AWS Management Console.
* Learn the process of creating an RDS Database.
* Learn how to choose the database engine, instance class, storage, and connection configuration.
* Learn how to use a Security Group to control connections to the database.
* Learn how to create a DB Snapshot and restore a database from a Snapshot.
* Explore Multi-AZ and Read Replica in RDS.
* Access the DynamoDB service on the AWS Management Console.
* Learn how to create a DynamoDB Table.
* Learn about Partition Key, Sort Key, Item, Attribute, Query, and Scan.
* Explore AWS Backup, Backup Vault, Backup Plan, and Resource Assignment.
* Note common errors when configuring databases: wrong Security Group, database not public, wrong endpoint, missing IAM permissions, or backup not configured.

---

## Comparison of Amazon RDS and DynamoDB

| Criteria              | Amazon RDS                                                      | Amazon DynamoDB                                      |
| --------------------- | --------------------------------------------------------------- | ---------------------------------------------------- |
| **Database type**     | Relational, SQL                                                 | NoSQL, Key-Value / Document                          |
| **Query method**      | SQL Query                                                       | Query / Scan by key                                  |
| **Use case**          | Systems needing tables, relations, transactions                | Systems needing high speed, flexible scaling        |
| **Infra management**  | AWS manages much, but DB Instance still needs configuration     | Fully managed by AWS, more serverless                |
| **Backup**            | Automated Backup, DB Snapshot                                   | On-demand Backup, Point-in-time Recovery, AWS Backup |
| **Example app**       | E-commerce site, order management, relational-data system      | Cart, session, log, fast-access data                |

---

## Week 7 Summary

**Week 7:** Explore Amazon RDS, DynamoDB, backup, restore, and database management on AWS. Understand the difference between relational and NoSQL databases, know how to choose the right database service, and understand the role of backup, snapshot, and restore in protecting system data.

[1]: https://cloudjourney.awsstudygroup.com/?utm_source=chatgpt.com "The First Cloud Journey"
[2]: https://000005.awsstudygroup.com/1-introduce/?utm_source=chatgpt.com "Introduction :: GETTING STARTED WITH AMAZON RDS"
[3]: https://000005.awsstudygroup.com/?utm_source=chatgpt.com "Amazon Relational Database Service (Amazon RDS)"
[4]: https://000013.awsstudygroup.com/1-introduce/?utm_source=chatgpt.com "Introduction :: DEPLOYING AWS BACKUP FOR THE SYSTEM"
