---
title: "Worklog Tuần 8"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---


# Worklog Tuần 8

## Mục tiêu tuần 8

Trong tuần 8, mục tiêu chính là tìm hiểu quy trình **dịch chuyển hệ thống lên AWS**, bao gồm dịch chuyển máy chủ ảo, dịch chuyển cơ sở dữ liệu và các bước kiểm tra sau khi migration. Nội dung này thuộc nhóm **Dịch chuyển lên AWS** trong AWS Cloud Journey, tập trung vào đánh giá workload, lập kế hoạch migration, dịch chuyển máy chủ/ứng dụng, dịch chuyển cơ sở dữ liệu, xác thực sau migration và chuẩn bị phương án rollback khi có sự cố. ([Cloud Journey][1])

Các nội dung trọng tâm của tuần bao gồm:

* Tìm hiểu tổng quan về cloud migration.
* Tìm hiểu các bước đánh giá và lập kế hoạch dịch chuyển hệ thống lên AWS.
* Tìm hiểu **AWS VM Import/Export** để chuyển máy ảo từ môi trường on-premise lên AWS.
* Tìm hiểu cách chuyển máy ảo thành **Amazon Machine Image - AMI** và triển khai thành **EC2 Instance**.
* Tìm hiểu **AWS Database Migration Service - DMS** và **Schema Conversion Tool - SCT** để dịch chuyển cơ sở dữ liệu.
* Tìm hiểu cách theo dõi, kiểm tra lỗi và dọn dẹp tài nguyên sau khi thực hành migration.

---

## Các công việc cần triển khai trong tuần này

| Thứ tự | Công việc thực hiện                                                                                                                                               | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                                                                                                                                                       |
| --- | --- | --- | --- | --- |
| **1**  | Tìm hiểu tổng quan về dịch chuyển lên AWS, các giai đoạn đánh giá workload, lập kế hoạch migration, xác thực sau migration và phương án rollback.                 | 08/06/2026 | 08/06/2026 | [https://cloudjourney.awsstudygroup.com/vi/2-migrate/](https://cloudjourney.awsstudygroup.com/vi/2-migrate/) <br> [https://cloudjourney.awsstudygroup.com/vi/](https://cloudjourney.awsstudygroup.com/vi/)                                                                                           |
| **2**  | Tìm hiểu AWS VM Import/Export, mục đích sử dụng, các yêu cầu chuẩn bị như AWS CLI, môi trường ảo hóa, S3 Bucket và IAM Role.                                      | 09/06/2026 | 09/06/2026 | [https://000014.awsstudygroup.com/vi/](https://000014.awsstudygroup.com/vi/) <br> [https://000014.awsstudygroup.com/vi/1-deploy-application-server/](https://000014.awsstudygroup.com/vi/1-deploy-application-server/)                                                                               |
| **3**  | Tìm hiểu quy trình import máy ảo vào AWS: export máy ảo từ môi trường on-premise, upload lên AWS, import thành AMI và khởi chạy EC2 Instance từ AMI đã import.    | 10/06/2026 | 10/06/2026 | [https://000014.awsstudygroup.com/vi/2-import-vm-to-aws/](https://000014.awsstudygroup.com/vi/2-import-vm-to-aws/) <br> [https://000014.awsstudygroup.com/vi/2-import-vm-to-aws/1-export-vm-from-virtual-env/](https://000014.awsstudygroup.com/vi/2-import-vm-to-aws/1-export-vm-from-virtual-env/) |
| **4**  | Tìm hiểu AWS Database Migration Service và Schema Conversion Tool, vai trò của từng công cụ trong quá trình chuyển đổi lược đồ và di chuyển dữ liệu.              | 11/06/2026 | 11/06/2026 | [https://000043.awsstudygroup.com/vi/](https://000043.awsstudygroup.com/vi/) <br> [https://cloudjourney.awsstudygroup.com/vi/2-migrate/](https://cloudjourney.awsstudygroup.com/vi/2-migrate/)                                                                                                       |
| **5**  | Tổng hợp kiến thức về migration, so sánh dịch chuyển máy chủ và dịch chuyển cơ sở dữ liệu; ghi chú lỗi thường gặp, cách theo dõi migration và dọn dẹp tài nguyên. | 12/06/2026 | 12/06/2026 | [https://000014.awsstudygroup.com/vi/](https://000014.awsstudygroup.com/vi/) <br> [https://000043.awsstudygroup.com/vi/](https://000043.awsstudygroup.com/vi/) <br> [https://cloudjourney.awsstudygroup.com/vi/2-migrate/](https://cloudjourney.awsstudygroup.com/vi/2-migrate/)                     |

---

## Kết quả đạt được tuần 8

### Tổng quan

Trong tuần này, tôi đã tìm hiểu quy trình dịch chuyển hệ thống từ môi trường truyền thống hoặc môi trường ảo hóa lên AWS. Nội dung tập trung vào hai nhóm chính là **dịch chuyển máy chủ ảo** bằng AWS VM Import/Export và **dịch chuyển cơ sở dữ liệu** bằng AWS DMS kết hợp AWS SCT.

### Kiến thức đã học

Sau khi hoàn thành tuần 8, tôi đã nắm được:

* Hiểu được mục đích của cloud migration là đưa workload, máy chủ, ứng dụng hoặc cơ sở dữ liệu từ môi trường hiện tại lên AWS.
* Hiểu quy trình cơ bản của migration gồm đánh giá hệ thống hiện tại, lập kế hoạch, chuẩn bị tài nguyên, thực hiện dịch chuyển, kiểm tra sau migration và dọn dẹp tài nguyên.
* Hiểu **AWS VM Import/Export** cho phép import máy ảo từ môi trường ảo hóa vào Amazon EC2 và cũng có thể export ngược lại. Công cụ này có thể dùng để chuyển ứng dụng từ on-premises lên EC2, sao lưu máy ảo hoặc tạo kho lưu trữ máy ảo phục vụ dự phòng/phục hồi. ([000014.awsstudygroup.com][2])
* Hiểu quy trình import máy ảo gồm chuẩn bị máy ảo, export từ môi trường on-premise, upload lên AWS, import thành AMI và khởi chạy EC2 Instance từ AMI đó. ([000014.awsstudygroup.com][3])
* Hiểu **AWS Schema Conversion Tool - SCT** hỗ trợ chuyển đổi schema của cơ sở dữ liệu nguồn sang định dạng tương thích với cơ sở dữ liệu đích, đặc biệt khi migration giữa hai hệ quản trị cơ sở dữ liệu khác nhau. ([000043.awsstudygroup.com][4])
* Hiểu **AWS Database Migration Service - DMS** hỗ trợ di chuyển dữ liệu từ cơ sở dữ liệu nguồn sang cơ sở dữ liệu đích, đồng thời có thể giúp giảm thời gian gián đoạn trong quá trình migration. ([000043.awsstudygroup.com][4])
* Biết tầm quan trọng của việc theo dõi log, kiểm tra trạng thái migration task và chuẩn bị phương án rollback khi quá trình dịch chuyển gặp lỗi.

### Thực hành

Trong quá trình học và tìm hiểu, tôi đã thực hiện được các nội dung sau:

* Tìm hiểu nhóm lộ trình **Dịch chuyển lên AWS** trên AWS Cloud Journey.
* Tìm hiểu vai trò của VM Import/Export trong việc chuyển máy ảo lên AWS.
* Tìm hiểu cách chuẩn bị máy ảo từ môi trường VMware Workstation.
* Tìm hiểu cách export máy ảo từ môi trường on-premise.
* Tìm hiểu cách upload máy ảo lên AWS và import thành AMI.
* Tìm hiểu cách khởi chạy EC2 Instance từ AMI đã import.
* Tìm hiểu AWS DMS, replication instance, source endpoint, target endpoint và migration task.
* Tìm hiểu AWS SCT trong quá trình chuyển đổi schema cơ sở dữ liệu.
* Ghi chú các lỗi thường gặp như thiếu quyền IAM, sai cấu hình S3 Bucket, lỗi định dạng máy ảo, lỗi kết nối database, sai security group hoặc migration task không chạy thành công.

---

## Bảng so sánh các công cụ migration

| Công cụ / dịch vụ        | Mục đích chính                                         | Trường hợp sử dụng                                                                                |
| ------------------------ | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
| **AWS VM Import/Export** | Dịch chuyển máy ảo lên AWS hoặc export máy ảo ra ngoài | Chuyển VM từ on-premise/VMware lên Amazon EC2                                                     |
| **AWS DMS**              | Di chuyển dữ liệu giữa các cơ sở dữ liệu               | Chuyển database từ on-premise, EC2 hoặc RDS sang database đích                                    |
| **AWS SCT**              | Chuyển đổi schema cơ sở dữ liệu                        | Migration giữa các hệ quản trị khác nhau như Oracle sang PostgreSQL, SQL Server sang MySQL/Aurora |

---

## Tóm tắt tuần 8

**Tuần 8:** Tìm hiểu Migration lên AWS với VM Import/Export, AWS DMS và Schema Conversion Tool. Nắm được quy trình dịch chuyển máy chủ ảo, chuyển đổi lược đồ cơ sở dữ liệu, di chuyển dữ liệu, theo dõi quá trình migration, xử lý lỗi và kiểm tra hệ thống sau khi dịch chuyển.

[1]: https://cloudjourney.awsstudygroup.com/vi/2-migrate/ "Dịch chuyển lên AWS :: Hành trình đầu tiên lên Mây"
[2]: https://000014.awsstudygroup.com/vi/ "AWS VM Import/Export :: VIRTUAL MACHINE (VM) IMPORT/EXPORT"
[3]: https://000014.awsstudygroup.com/vi/2-import-vm-to-aws/ "Import máy ảo vào AWS :: VIRTUAL MACHINE (VM) IMPORT/EXPORT"
[4]: https://000043.awsstudygroup.com/vi/ "Chuyển đổi lược đồ và di dời CSDL :: AWS Workshop - Di chuyển dữ liệu"
