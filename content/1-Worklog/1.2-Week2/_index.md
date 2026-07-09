---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---


## Week 2 Objectives

In week 2, the main goal was to explore the **AWS Identity and Access Management - IAM** service. This service is used to manage identities, control access, and govern users when working with AWS resources. IAM helps manage **Users, Groups, Roles, and Policies**, and supports applying the principle of least privilege across the system. ([000002.awsstudygroup.com][1])

Key topics for the week include:

* Getting an overview of AWS IAM.
* Exploring IAM User, IAM Group, IAM Role, and IAM Policy.
* Practicing creating an admin Group and User.
* Learning how to grant permissions through Policies.
* Learning how to use IAM Role to grant temporary access.
* Noting security best practices when using IAM.

---

## Tasks to be carried out this week

| No. | Task                                                                                                                                                       | Start Date | Completion Date | Reference Material                                                                                                                |
| --- | --- | --- | --- | --- |
| **1** | Get an overview of AWS IAM and its role in managing identities, authentication, and access control for AWS resources.                                     | 04/27/2026 | 04/27/2026 | [https://000002.awsstudygroup.com/](https://000002.awsstudygroup.com/)                                                           |
| **2** | Explore the main IAM components: IAM User, IAM Group, IAM Role, and IAM Policy.                                                                            | 04/28/2026 | 04/28/2026 | [https://000002.awsstudygroup.com/1-introduction/](https://000002.awsstudygroup.com/1-introduction/)                             |
| **3** | Explore IAM Policy, how a Policy defines access permissions, and how to attach Policies to Users, Groups, or Roles.                                        | 04/29/2026 | 04/29/2026 | [https://000002.awsstudygroup.com/1-introduction/1.2-iam-policy/](https://000002.awsstudygroup.com/1-introduction/1.2-iam-policy/) |
| **4** | Practice creating an IAM Group and IAM User, assigning admin permissions to the Group, and signing in as the IAM User.                                      | 04/30/2026 | 04/30/2026 | [https://000002.awsstudygroup.com/2-create-admin-user-and-group/](https://000002.awsstudygroup.com/2-create-admin-user-and-group/) |
| **5** | Explore IAM Role, how to grant temporary permissions to AWS services or other users, and note security principles when using IAM.                          | 05/01/2026 | 05/01/2026 | [https://000002.awsstudygroup.com/3-aws-role/](https://000002.awsstudygroup.com/3-aws-role/)                                     |

---

## Week 2 Achievements

### Overview

This week, I explored the **AWS IAM** service and understood its role in managing access on AWS. IAM enables fine-grained control over who can access which resources and what actions they can perform on the AWS system. ([Amazon Web Services, Inc.][2])

### Knowledge gained

After completing week 2, I have understood:

* The role of IAM in managing identities and access control.
* The difference between **IAM User**, **IAM Group**, **IAM Role**, and **IAM Policy**.
* That an IAM Policy is a document defining detailed access permissions and can be attached to a User, Group, or Role. ([000002.awsstudygroup.com][3])
* That an IAM Role is used to grant temporary access to a User, an AWS service, another AWS account, or an external application. ([000002.awsstudygroup.com][4])
* The **least privilege** principle, meaning only the permissions necessary for a user or service should be granted.
* Why the root account should not be used for day-to-day tasks.

### Practice

During the learning and practice process, I was able to:

* Access the IAM service on the AWS Management Console.
* Learn how to create an IAM Group.
* Learn how to create an IAM User.
* Assign an appropriate Policy to the IAM Group.
* Try signing in as the IAM User.
* Learn how to create an IAM Role and use cases for Roles with AWS services.
* Note common errors from incorrect or missing Policies when assigning permissions.

---

## Week 2 Summary

**Week 2:** Explore IAM, manage Users, Groups, Roles, Policies, and access control on AWS. Understand how IAM supports authentication, authorization, and access control for AWS resources following the principle of least privilege security.

[1]: https://000002.awsstudygroup.com/?utm_source=chatgpt.com "Managing Access with AWS IAM (Identity and Access ..."
[2]: https://aws.amazon.com/iam/?utm_source=chatgpt.com "AWS Identity and Access Management (IAM)"
[3]: https://000002.awsstudygroup.com/1-introduction/1.2-iam-policy/?utm_source=chatgpt.com "AWS Identity and Access Management (IAM) Policy"
[4]: https://000002.awsstudygroup.com/1-introduction/1.3-iam-role/?utm_source=chatgpt.com "AWS Identity and Access Management (IAM) Role"
