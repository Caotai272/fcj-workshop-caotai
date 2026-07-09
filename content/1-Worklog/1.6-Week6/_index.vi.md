---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---


# Worklog Tuần 6

## Mục tiêu tuần 6

Trong tuần 6, mục tiêu chính là tìm hiểu các dịch vụ lưu trữ dữ liệu trên AWS, bao gồm **Amazon S3, Amazon EBS và Amazon EFS**. Đây là các dịch vụ quan trọng trong việc lưu trữ file, dữ liệu ứng dụng, ổ đĩa cho máy chủ EC2 và hệ thống tệp dùng chung.

Nội dung tuần này thuộc nhóm **Explore / Khám phá dịch vụ AWS**, tập trung vào việc nhận biết các loại hình lưu trữ trên AWS và lựa chọn dịch vụ phù hợp theo từng nhu cầu sử dụng. Amazon S3 là dịch vụ lưu trữ đối tượng, Amazon EBS là lưu trữ dạng block dùng với EC2, còn Amazon EFS là hệ thống file serverless có thể chia sẻ dữ liệu cho các dịch vụ compute. ([AWS Documentation][1])

Các nội dung trọng tâm của tuần bao gồm:

* Tìm hiểu tổng quan về các loại lưu trữ trên AWS.
* Tìm hiểu **Amazon S3** để lưu trữ object, file tĩnh, tài liệu, hình ảnh và dữ liệu backup.
* Tìm hiểu **Amazon EBS** để cung cấp ổ đĩa lưu trữ cho EC2 Instance.
* Tìm hiểu **Amazon EFS** để tạo hệ thống tệp dùng chung cho nhiều tài nguyên AWS.
* So sánh S3, EBS và EFS theo mục đích sử dụng.
* Ghi chú các lưu ý về phân quyền, backup, bảo mật và chi phí lưu trữ.

---

## Các công việc cần triển khai trong tuần này

| Thứ tự | Công việc thực hiện                                                                                                                      | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| --- | --- | --- | --- | --- |
| **1**  | Tìm hiểu tổng quan về nhóm dịch vụ lưu trữ trên AWS, phân biệt object storage, block storage và file storage.                            | 25/05/2026 | 25/05/2026 | [https://cloudjourney.awsstudygroup.com/vi/1-explore/](https://cloudjourney.awsstudygroup.com/vi/1-explore/) <br> [https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) <br> [https://docs.aws.amazon.com/ebs/latest/userguide/what-is-ebs.html](https://docs.aws.amazon.com/ebs/latest/userguide/what-is-ebs.html) <br> [https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) |
| **2**  | Tìm hiểu Amazon S3, cách tạo bucket, upload object, quản lý object, phân quyền truy cập, versioning và static website hosting.           | 26/05/2026 | 26/05/2026 | [https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) <br> [https://docs.aws.amazon.com/AmazonS3/latest/userguide/GetStartedWithS3.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/GetStartedWithS3.html) <br> [https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingObjects.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingObjects.html)                                                                 |
| **3**  | Tìm hiểu Amazon EBS, EBS Volume, Snapshot, cách gắn volume vào EC2 Instance và vai trò của EBS trong lưu trữ dữ liệu cho máy chủ ảo.     | 27/05/2026 | 27/05/2026 | [https://docs.aws.amazon.com/ebs/latest/userguide/what-is-ebs.html](https://docs.aws.amazon.com/ebs/latest/userguide/what-is-ebs.html) <br> [https://docs.aws.amazon.com/ebs/latest/userguide/ebs-volume-types.html](https://docs.aws.amazon.com/ebs/latest/userguide/ebs-volume-types.html) <br> [https://000004.awsstudygroup.com/vi/5-amazonec2basic/5.2-createec2snapshot/](https://000004.awsstudygroup.com/vi/5-amazonec2basic/5.2-createec2snapshot/)                                                                     |
| **4**  | Tìm hiểu Amazon EFS, hệ thống file dùng chung, khả năng chia sẻ dữ liệu giữa nhiều tài nguyên compute; tổng hợp và so sánh S3, EBS, EFS. | 28/05/2026 | 28/05/2026 | [https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) <br> [https://aws.amazon.com/vi/efs/](https://aws.amazon.com/vi/efs/) <br> [https://000013.awsstudygroup.com/vi/1-introduce/](https://000013.awsstudygroup.com/vi/1-introduce/)                                                                                                                                                                                                                             |

---

## Kết quả đạt được tuần 6

### Tổng quan

Trong tuần này, tôi đã tìm hiểu các dịch vụ lưu trữ phổ biến trên AWS gồm **Amazon S3, Amazon EBS và Amazon EFS**. Mỗi dịch vụ có mục đích sử dụng khác nhau: S3 phù hợp lưu trữ object như file, ảnh, tài liệu; EBS phù hợp làm ổ đĩa cho EC2 Instance; EFS phù hợp khi cần một hệ thống file dùng chung có thể mở rộng linh hoạt. ([AWS Documentation][2])

### Kiến thức đã học

Sau khi hoàn thành tuần 6, tôi đã nắm được:

* Hiểu được sự khác nhau giữa **object storage**, **block storage** và **file storage**.
* Hiểu **Amazon S3** dùng để lưu trữ object trong bucket, phù hợp với file tĩnh, hình ảnh, tài liệu, backup và dữ liệu ứng dụng.
* Hiểu cách Amazon S3 quản lý dữ liệu thông qua **bucket**, **object**, **key**, **metadata** và quyền truy cập.
* Hiểu **Amazon EBS** cung cấp block storage có thể gắn vào EC2 Instance để sử dụng như ổ đĩa lưu trữ.
* Hiểu **EBS Snapshot** dùng để sao lưu dữ liệu từ EBS Volume và hỗ trợ khôi phục khi cần.
* Hiểu **Amazon EFS** là hệ thống tệp có thể mở rộng linh hoạt, phù hợp khi nhiều tài nguyên compute cần truy cập chung một hệ thống file.
* Biết được AWS Backup có thể hỗ trợ sao lưu nhiều tài nguyên như EBS Volumes, RDS Databases, DynamoDB Tables và EFS File Systems. ([000013.awsstudygroup.com][3])

### Thực hành

Trong quá trình học và thực hành, tôi đã thực hiện được các nội dung sau:

* Tìm hiểu giao diện quản lý Amazon S3 trên AWS Management Console.
* Tìm hiểu cách tạo S3 bucket và upload object.
* Tìm hiểu cách cấu hình quyền truy cập cho bucket và object.
* Tìm hiểu S3 Versioning để lưu nhiều phiên bản của object.
* Tìm hiểu cách sử dụng S3 cho static website hosting.
* Tìm hiểu EBS Volume khi khởi tạo hoặc sử dụng EC2 Instance.
* Tìm hiểu cách tạo EBS Snapshot để sao lưu dữ liệu.
* Tìm hiểu Amazon EFS và trường hợp dùng file storage dùng chung.
* Lập bảng so sánh cơ bản giữa S3, EBS và EFS.
* Ghi chú các lưu ý về bảo mật, phân quyền truy cập và dọn dẹp tài nguyên để tránh phát sinh chi phí.

---

## Bảng so sánh S3, EBS và EFS

| Dịch vụ        | Loại lưu trữ   | Mục đích sử dụng chính                                 |
| -------------- | -------------- | ------------------------------------------------------ |
| **Amazon S3**  | Object Storage | Lưu file, ảnh, video, tài liệu, backup, static website |
| **Amazon EBS** | Block Storage  | Làm ổ đĩa lưu trữ cho EC2 Instance                     |
| **Amazon EFS** | File Storage   | Hệ thống file dùng chung cho nhiều tài nguyên compute  |

---

## Tóm tắt tuần 6

**Tuần 6:** Tìm hiểu Amazon S3, EBS, EFS và các hình thức lưu trữ dữ liệu trên AWS. Nắm được sự khác nhau giữa object storage, block storage và file storage; biết cách lựa chọn dịch vụ lưu trữ phù hợp theo từng nhu cầu triển khai hệ thống.

[1]: https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html?utm_source=chatgpt.com "What is Amazon S3? - Amazon Simple Storage Service"
[2]: https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingObjects.html?utm_source=chatgpt.com "Amazon S3 objects overview"
[3]: https://000013.awsstudygroup.com/vi/1-introduce/?utm_source=chatgpt.com "Giới thiệu :: TRIỂN KHAI AWS BACKUP CHO HỆ THỐNG"
