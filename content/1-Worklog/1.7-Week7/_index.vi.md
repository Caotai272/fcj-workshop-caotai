---
title: "Worklog Tuần 7"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---


# Worklog Tuần 7

## Mục tiêu tuần 7

Trong tuần 7, mục tiêu chính là tìm hiểu các dịch vụ cơ sở dữ liệu trên AWS, gồm **Amazon RDS** và **Amazon DynamoDB**. Đây là hai dịch vụ quan trọng dùng để lưu trữ, quản lý và truy vấn dữ liệu trong hệ thống. Amazon RDS phù hợp với cơ sở dữ liệu quan hệ như MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, còn DynamoDB là dịch vụ cơ sở dữ liệu NoSQL được quản lý hoàn toàn trên AWS. Nội dung này nằm trong nhóm **Explore / Khám phá dịch vụ AWS**, trong đó AWS Study Group có đề cập đến RDS và DynamoDB như các dịch vụ nền tảng khi học AWS. ([Cloud Journey][1])

Các nội dung trọng tâm của tuần bao gồm:

* Tìm hiểu tổng quan về cơ sở dữ liệu trên AWS.
* Tìm hiểu **Amazon RDS** và cách tạo database quan hệ.
* Tìm hiểu backup, snapshot, restore, Multi-AZ và Read Replica trong RDS.
* Tìm hiểu **Amazon DynamoDB** và mô hình cơ sở dữ liệu NoSQL.
* Tìm hiểu AWS Backup để sao lưu và khôi phục dữ liệu.
* So sánh RDS và DynamoDB theo từng trường hợp sử dụng.

---

## Các công việc cần triển khai trong tuần này

| Thứ tự | Công việc thực hiện                                                                                                                                     | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                                                                                                                                                                                                                                       |
| --- | --- | --- | --- | --- |
| **1**  | Tìm hiểu tổng quan về cơ sở dữ liệu trên AWS, phân biệt database quan hệ và NoSQL, xác định khi nào nên dùng RDS và khi nào nên dùng DynamoDB.          | 01/06/2026 | 01/06/2026 | [https://cloudjourney.awsstudygroup.com/vi/1-explore/](https://cloudjourney.awsstudygroup.com/vi/1-explore/) <br> [https://000005.awsstudygroup.com/vi/](https://000005.awsstudygroup.com/vi/) <br> [https://000053.awsstudygroup.com/vi/](https://000053.awsstudygroup.com/vi/)                                                                                                     |
| **2**  | Tìm hiểu Amazon RDS, các khái niệm DB Instance, DB Engine, endpoint, storage, security group và cách kết nối ứng dụng với database.                     | 02/06/2026 | 02/06/2026 | [https://000005.awsstudygroup.com/vi/](https://000005.awsstudygroup.com/vi/) <br> [https://000005.awsstudygroup.com/vi/1-introduce/](https://000005.awsstudygroup.com/vi/1-introduce/)                                                                                                                                                                                               |
| **3**  | Tìm hiểu backup, DB Snapshot, restore, Multi-AZ và Read Replica trong Amazon RDS để tăng độ an toàn dữ liệu và khả năng sẵn sàng của hệ thống.          | 03/06/2026 | 03/06/2026 | [https://000005.awsstudygroup.com/vi/1-introduce/](https://000005.awsstudygroup.com/vi/1-introduce/)                                                                                                                                                                                                                                                                                 |
| **4**  | Tìm hiểu Amazon DynamoDB, mô hình NoSQL, Table, Item, Partition Key, Sort Key, Query, Scan và cách DynamoDB lưu trữ dữ liệu.                            | 04/06/2026 | 04/06/2026 | [https://000053.awsstudygroup.com/vi/](https://000053.awsstudygroup.com/vi/) <br> [https://000053.awsstudygroup.com/vi/1-introduction/](https://000053.awsstudygroup.com/vi/1-introduction/) <br> [https://000055.awsstudygroup.com/vi/3-create-single-page-app/3.1-create-dynamodb-table/](https://000055.awsstudygroup.com/vi/3-create-single-page-app/3.1-create-dynamodb-table/) |
| **5**  | Tìm hiểu AWS Backup, backup vault, backup plan, resource assignment và cách sao lưu, khôi phục tài nguyên như RDS Database, DynamoDB Table, EBS và EFS. | 05/06/2026 | 05/06/2026 | [https://000013.awsstudygroup.com/vi/](https://000013.awsstudygroup.com/vi/) <br> [https://000013.awsstudygroup.com/vi/1-introduce/](https://000013.awsstudygroup.com/vi/1-introduce/) <br> [https://000039.awsstudygroup.com/vi/1-lhol/1.4/1.4.1/](https://000039.awsstudygroup.com/vi/1-lhol/1.4/1.4.1/)                                                                           |
| **6**  | Tổng hợp kiến thức, so sánh Amazon RDS và DynamoDB, ghi chú các lưu ý về bảo mật, backup, restore, chi phí và dọn dẹp tài nguyên sau khi thực hành.     | 06/06/2026 | 06/06/2026 | [https://cloudjourney.awsstudygroup.com/vi/1-explore/](https://cloudjourney.awsstudygroup.com/vi/1-explore/) <br> [https://000005.awsstudygroup.com/vi/](https://000005.awsstudygroup.com/vi/) <br> [https://000053.awsstudygroup.com/vi/](https://000053.awsstudygroup.com/vi/) <br> [https://000013.awsstudygroup.com/vi/](https://000013.awsstudygroup.com/vi/)                   |

---

## Kết quả đạt được tuần 7

### Tổng quan

Trong tuần này, tôi đã tìm hiểu hai nhóm cơ sở dữ liệu phổ biến trên AWS là **Amazon RDS** và **Amazon DynamoDB**. Amazon RDS hỗ trợ triển khai cơ sở dữ liệu quan hệ có quản lý, còn Amazon DynamoDB là dịch vụ NoSQL được quản lý hoàn toàn, phù hợp với hệ thống cần khả năng mở rộng linh hoạt và hiệu suất ổn định. ([000005.awsstudygroup.com][2])

### Kiến thức đã học

Sau khi hoàn thành tuần 7, tôi đã nắm được:

* Hiểu được vai trò của cơ sở dữ liệu trong hệ thống triển khai trên AWS.
* Phân biệt được **Relational Database** và **NoSQL Database**.
* Hiểu **Amazon RDS** dùng để triển khai các hệ quản trị cơ sở dữ liệu quan hệ như MySQL, PostgreSQL, MariaDB, Oracle hoặc SQL Server.
* Hiểu các thành phần cơ bản của RDS như **DB Instance**, **DB Engine**, **Endpoint**, **Storage**, **Security Group** và **Backup**.
* Hiểu **DB Snapshot** trong RDS dùng để sao lưu database ở một thời điểm xác định và có thể dùng để khôi phục thành DB Instance mới. ([000005.awsstudygroup.com][3])
* Hiểu **Multi-AZ** giúp tăng tính sẵn sàng cho RDS, còn **Read Replica** hỗ trợ giảm tải truy vấn đọc cho database. ([000005.awsstudygroup.com][2])
* Hiểu **Amazon DynamoDB** là cơ sở dữ liệu NoSQL được quản lý hoàn toàn, có thể tạo bảng, lưu item và truy vấn dữ liệu theo key.
* Hiểu **AWS Backup** có thể dùng để tập trung và tự động hóa việc sao lưu các tài nguyên như EBS, RDS, DynamoDB và EFS. ([Aws Study Group][4])

### Thực hành

Trong quá trình học và thực hành, tôi đã thực hiện được các nội dung sau:

* Truy cập dịch vụ Amazon RDS trên AWS Management Console.
* Tìm hiểu quy trình tạo RDS Database.
* Tìm hiểu cách chọn database engine, instance class, storage và cấu hình kết nối.
* Tìm hiểu cách dùng Security Group để kiểm soát kết nối đến database.
* Tìm hiểu cách tạo DB Snapshot và khôi phục database từ Snapshot.
* Tìm hiểu Multi-AZ và Read Replica trong RDS.
* Truy cập dịch vụ DynamoDB trên AWS Management Console.
* Tìm hiểu cách tạo DynamoDB Table.
* Tìm hiểu Partition Key, Sort Key, Item, Attribute, Query và Scan.
* Tìm hiểu AWS Backup, Backup Vault, Backup Plan và Resource Assignment.
* Ghi chú các lỗi thường gặp khi cấu hình database như sai Security Group, database không public, sai endpoint, thiếu quyền IAM hoặc chưa cấu hình backup.

---

## Bảng so sánh Amazon RDS và DynamoDB

| Tiêu chí               | Amazon RDS                                                      | Amazon DynamoDB                                      |
| ---------------------- | --------------------------------------------------------------- | ---------------------------------------------------- |
| **Loại cơ sở dữ liệu** | Quan hệ, SQL                                                    | NoSQL, Key-Value / Document                          |
| **Cách truy vấn**      | SQL Query                                                       | Query / Scan theo key                                |
| **Trường hợp sử dụng** | Hệ thống cần bảng, quan hệ, transaction                         | Hệ thống cần tốc độ cao, mở rộng linh hoạt           |
| **Quản lý hạ tầng**    | AWS quản lý nhiều phần, nhưng vẫn cần cấu hình DB Instance      | AWS quản lý hoàn toàn, serverless hơn                |
| **Backup**             | Automated Backup, DB Snapshot                                   | On-demand Backup, Point-in-time Recovery, AWS Backup |
| **Ví dụ ứng dụng**     | Website bán hàng, quản lý đơn hàng, hệ thống có dữ liệu quan hệ | Giỏ hàng, session, log, dữ liệu truy cập nhanh       |

---

## Tóm tắt tuần 7

**Tuần 7:** Tìm hiểu Amazon RDS, DynamoDB, backup, restore và quản lý cơ sở dữ liệu trên AWS. Nắm được sự khác nhau giữa cơ sở dữ liệu quan hệ và NoSQL, biết cách lựa chọn dịch vụ database phù hợp, đồng thời hiểu vai trò của backup, snapshot và restore trong việc bảo vệ dữ liệu hệ thống.

[1]: https://cloudjourney.awsstudygroup.com/vi/?utm_source=chatgpt.com "Hành trình đầu tiên lên Mây - The First Cloud Journey"
[2]: https://000005.awsstudygroup.com/vi/1-introduce/?utm_source=chatgpt.com "Giới thiệu :: BẮT ĐẦU VỚI AMAZON RDS"
[3]: https://000005.awsstudygroup.com/vi/?utm_source=chatgpt.com "Amazon Relational Database Service (Amazon RDS)"
[4]: https://000013.awsstudygroup.com/vi/1-introduce/?utm_source=chatgpt.com "Giới thiệu :: TRIỂN KHAI AWS BACKUP CHO HỆ THỐNG"
