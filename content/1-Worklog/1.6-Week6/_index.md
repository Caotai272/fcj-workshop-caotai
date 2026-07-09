---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---


# Week 6 Worklog

## Week 6 Objectives

In week 6, the main goal was to explore AWS data storage services: **Amazon S3, Amazon EBS, and Amazon EFS**. These are important services for storing files, application data, disks for EC2 servers, and shared file systems.

This week's content belongs to the **Explore / AWS Service Exploration** group, focusing on recognizing the types of storage on AWS and choosing the right service for each use case. Amazon S3 is object storage, Amazon EBS is block storage used with EC2, and Amazon EFS is a serverless file system that can share data across compute services. ([AWS Documentation][1])

Key topics for the week include:

* Getting an overview of storage types on AWS.
* Exploring **Amazon S3** for storing objects, static files, documents, images, and backup data.
* Exploring **Amazon EBS** for providing storage volumes for EC2 Instances.
* Exploring **Amazon EFS** for building a shared file system for multiple AWS resources.
* Comparing S3, EBS, and EFS by purpose.
* Noting cautions about permissions, backup, security, and storage cost.

---

## Tasks to be carried out this week

| No. | Task                                                                                                                                                     | Start Date | Completion Date | Reference Material                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| --- | --- | --- | --- | --- |
| **1** | Get an overview of the AWS storage service group, distinguishing object storage, block storage, and file storage.                                      | 05/25/2026 | 05/25/2026 | [https://cloudjourney.awsstudygroup.com/1-explore/](https://cloudjourney.awsstudygroup.com/1-explore/) <br> [https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) <br> [https://docs.aws.amazon.com/ebs/latest/userguide/what-is-ebs.html](https://docs.aws.amazon.com/ebs/latest/userguide/what-is-ebs.html) <br> [https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html)                                                                                                                                                                                       |
| **2** | Explore Amazon S3: creating a bucket, uploading objects, managing objects, configuring access, versioning, and static website hosting.                 | 05/26/2026 | 05/26/2026 | [https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) <br> [https://docs.aws.amazon.com/AmazonS3/latest/userguide/GetStartedWithS3.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/GetStartedWithS3.html) <br> [https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingObjects.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingObjects.html)                                                                                                                                                                                                        |
| **3** | Explore Amazon EBS, EBS Volume, Snapshot, how to attach a volume to an EC2 Instance, and EBS's role in storing data for virtual servers.               | 05/27/2026 | 05/27/2026 | [https://docs.aws.amazon.com/ebs/latest/userguide/what-is-ebs.html](https://docs.aws.amazon.com/ebs/latest/userguide/what-is-ebs.html) <br> [https://docs.aws.amazon.com/ebs/latest/userguide/ebs-volume-types.html](https://docs.aws.amazon.com/ebs/latest/userguide/ebs-volume-types.html) <br> [https://000004.awsstudygroup.com/5-amazonec2basic/5.2-createec2snapshot/](https://000004.awsstudygroup.com/5-amazonec2basic/5.2-createec2snapshot/)                                                                                                                                                                                                                         |
| **4** | Explore Amazon EFS, the shared file system, its ability to share data across compute resources; consolidate and compare S3, EBS, and EFS.              | 05/28/2026 | 05/28/2026 | [https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) <br> [https://aws.amazon.com/efs/](https://aws.amazon.com/efs/) <br> [https://000013.awsstudygroup.com/1-introduce/](https://000013.awsstudygroup.com/1-introduce/)                                                                                                                                                                                                                                                                                                                                                                                                        |

---

## Week 6 Achievements

### Overview

This week, I explored popular AWS storage services: **Amazon S3, Amazon EBS, and Amazon EFS**. Each service has a different purpose: S3 fits object storage such as files, images, and documents; EBS fits as a disk for EC2 Instances; EFS fits when a flexibly scalable shared file system is needed. ([AWS Documentation][2])

### Knowledge gained

After completing week 6, I have understood:

* The difference between **object storage**, **block storage**, and **file storage**.
* That **Amazon S3** stores objects in a bucket, suitable for static files, images, documents, backups, and application data.
* How Amazon S3 manages data through **bucket**, **object**, **key**, **metadata**, and access permissions.
* That **Amazon EBS** provides block storage that can be attached to an EC2 Instance as a storage disk.
* That an **EBS Snapshot** backs up data from an EBS Volume and supports recovery when needed.
* That **Amazon EFS** is a flexibly scalable file system, suitable when multiple compute resources need to access a shared file system.
* That AWS Backup can back up many resources such as EBS Volumes, RDS Databases, DynamoDB Tables, and EFS File Systems. ([000013.awsstudygroup.com][3])

### Practice

During the learning and practice process, I was able to:

* Explore the Amazon S3 management interface on the AWS Management Console.
* Learn how to create an S3 bucket and upload objects.
* Learn how to configure access permissions for a bucket and its objects.
* Explore S3 Versioning to keep multiple versions of an object.
* Learn how to use S3 for static website hosting.
* Explore the EBS Volume when launching or using an EC2 Instance.
* Learn how to create an EBS Snapshot to back up data.
* Explore Amazon EFS and use cases for shared file storage.
* Build a basic comparison table between S3, EBS, and EFS.
* Note cautions about security, access permissions, and cleaning up resources to avoid unexpected costs.

---

## Comparison of S3, EBS, and EFS

| Service        | Storage Type  | Main Purpose                                            |
| -------------- | ------------- | ------------------------------------------------------- |
| **Amazon S3**  | Object Storage | Store files, images, videos, documents, backups, static websites |
| **Amazon EBS** | Block Storage | Storage disk for EC2 Instances                          |
| **Amazon EFS** | File Storage  | Shared file system for multiple compute resources      |

---

## Week 6 Summary

**Week 6:** Explore Amazon S3, EBS, EFS, and AWS data storage forms. Understand the difference between object storage, block storage, and file storage; know how to choose the right storage service for each system deployment need.

[1]: https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html?utm_source=chatgpt.com "What is Amazon S3? - Amazon Simple Storage Service"
[2]: https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingObjects.html?utm_source=chatgpt.com "Amazon S3 objects overview"
[3]: https://000013.awsstudygroup.com/1-introduce/?utm_source=chatgpt.com "Introduction :: DEPLOYING AWS BACKUP FOR THE SYSTEM"
