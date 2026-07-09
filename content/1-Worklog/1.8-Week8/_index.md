---
title: "Week 8 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---


# Week 8 Worklog

## Week 8 Objectives

In week 8, the main goal was to explore the **system migration process to AWS**, including migrating virtual servers, migrating databases, and the post-migration validation steps. This content belongs to the **Migrate to AWS** group in the AWS Cloud Journey, focusing on workload assessment, migration planning, server/application migration, database migration, post-migration validation, and preparing a rollback plan for failures. ([Cloud Journey][1])

Key topics for the week include:

* Getting an overview of cloud migration.
* Exploring the assessment and planning steps for migrating systems to AWS.
* Exploring **AWS VM Import/Export** to move virtual machines from an on-premise environment to AWS.
* Learning how to convert a virtual machine into an **Amazon Machine Image - AMI** and deploy it as an **EC2 Instance**.
* Exploring **AWS Database Migration Service - DMS** and **Schema Conversion Tool - SCT** for database migration.
* Learning how to monitor, troubleshoot, and clean up resources after practicing migration.

---

## Tasks to be carried out this week

| No. | Task                                                                                                                                                  | Start Date | Completion Date | Reference Material                                                                                                                                                                                                                                                                                       |
| --- | --- | --- | --- | --- |
| **1** | Get an overview of migrating to AWS, the stages of workload assessment, migration planning, post-migration validation, and rollback plan.            | 06/08/2026 | 06/08/2026 | [https://cloudjourney.awsstudygroup.com/2-migrate/](https://cloudjourney.awsstudygroup.com/2-migrate/) <br> [https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)                                                                                                           |
| **2** | Explore AWS VM Import/Export, its purpose, and preparation requirements such as AWS CLI, virtualization environment, S3 Bucket, and IAM Role.        | 06/09/2026 | 06/09/2026 | [https://000014.awsstudygroup.com/](https://000014.awsstudygroup.com/) <br> [https://000014.awsstudygroup.com/1-deploy-application-server/](https://000014.awsstudygroup.com/1-deploy-application-server/)                                                                                             |
| **3** | Explore the VM import process: export the VM from on-premise, upload to AWS, import into an AMI, and launch an EC2 Instance from the imported AMI.   | 06/10/2026 | 06/10/2026 | [https://000014.awsstudygroup.com/2-import-vm-to-aws/](https://000014.awsstudygroup.com/2-import-vm-to-aws/) <br> [https://000014.awsstudygroup.com/2-import-vm-to-aws/1-export-vm-from-virtual-env/](https://000014.awsstudygroup.com/2-import-vm-to-aws/1-export-vm-from-virtual-env/)             |
| **4** | Explore AWS Database Migration Service and Schema Conversion Tool, and the role of each in schema conversion and data migration.                     | 06/11/2026 | 06/11/2026 | [https://000043.awsstudygroup.com/](https://000043.awsstudygroup.com/) <br> [https://cloudjourney.awsstudygroup.com/2-migrate/](https://cloudjourney.awsstudygroup.com/2-migrate/)                                                                                                                     |
| **5** | Consolidate migration knowledge, compare server vs database migration; note common errors, monitoring approaches, and resource cleanup.             | 06/12/2026 | 06/12/2026 | [https://000014.awsstudygroup.com/](https://000014.awsstudygroup.com/) <br> [https://000043.awsstudygroup.com/](https://000043.awsstudygroup.com/) <br> [https://cloudjourney.awsstudygroup.com/2-migrate/](https://cloudjourney.awsstudygroup.com/2-migrate/)                                       |

---

## Week 8 Achievements

### Overview

This week, I explored the process of migrating systems from traditional or virtualized environments to AWS. The content focused on two main groups: **virtual server migration** using AWS VM Import/Export and **database migration** using AWS DMS together with AWS SCT.

### Knowledge gained

After completing week 8, I have understood:

* The purpose of cloud migration is to bring workloads, servers, applications, or databases from the current environment to AWS.
* The basic migration process: assess the current system, plan, prepare resources, perform the migration, validate after migration, and clean up resources.
* That **AWS VM Import/Export** lets you import a virtual machine from a virtualization environment into Amazon EC2 and also export it back out. It can be used to move applications from on-premises to EC2, back up virtual machines, or build a VM repository for disaster recovery. ([000014.awsstudygroup.com][2])
* The VM import process: prepare the VM, export from on-premise, upload to AWS, import into an AMI, and launch an EC2 Instance from that AMI. ([000014.awsstudygroup.com][3])
* That **AWS Schema Conversion Tool - SCT** helps convert the source database schema into a format compatible with the target database, especially when migrating between two different database engines. ([000043.awsstudygroup.com][4])
* That **AWS Database Migration Service - DMS** helps migrate data from a source database to a target database and can reduce downtime during migration. ([000043.awsstudygroup.com][4])
* The importance of monitoring logs, checking migration task status, and preparing a rollback plan when the migration fails.

### Practice

During the learning and exploration process, I was able to:

* Explore the **Migrate to AWS** pathway on the AWS Cloud Journey.
* Learn the role of VM Import/Export in moving virtual machines to AWS.
* Learn how to prepare a VM from a VMware Workstation environment.
* Learn how to export a VM from an on-premise environment.
* Learn how to upload a VM to AWS and import it into an AMI.
* Learn how to launch an EC2 Instance from the imported AMI.
* Explore AWS DMS, replication instance, source endpoint, target endpoint, and migration task.
* Explore AWS SCT in the database schema conversion process.
* Note common errors such as missing IAM permissions, wrong S3 Bucket configuration, VM format errors, database connection errors, wrong security group, or migration task not running successfully.

---

## Migration Tools Comparison

| Tool / Service           | Main Purpose                                          | Use Case                                                                                         |
| ------------------------ | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| **AWS VM Import/Export** | Migrate VMs to AWS or export VMs out                  | Move VMs from on-premise/VMware to Amazon EC2                                                    |
| **AWS DMS**              | Move data between databases                           | Migrate database from on-premise, EC2, or RDS to a target database                                |
| **AWS SCT**              | Convert database schema                              | Migration between different engines, e.g. Oracle to PostgreSQL, SQL Server to MySQL/Aurora       |

---

## Week 8 Summary

**Week 8:** Explore Migration to AWS with VM Import/Export, AWS DMS, and Schema Conversion Tool. Understand the virtual server migration process, database schema conversion, data migration, monitoring the migration, handling errors, and validating the system after migration.

[1]: https://cloudjourney.awsstudygroup.com/2-migrate/ "Migrate to AWS :: The First Cloud Journey"
[2]: https://000014.awsstudygroup.com/ "AWS VM Import/Export :: VIRTUAL MACHINE (VM) IMPORT/EXPORT"
[3]: https://000014.awsstudygroup.com/2-import-vm-to-aws/ "Import VM to AWS :: VIRTUAL MACHINE (VM) IMPORT/EXPORT"
[4]: https://000043.awsstudygroup.com/ "Schema Conversion and Data Migration :: AWS Workshop - Data Migration"
