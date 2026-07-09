---
title: "Worklog Tuần 4"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---


# Worklog Tuần 4

## Mục tiêu tuần 4

Trong tuần 4, mục tiêu chính là tìm hiểu dịch vụ **Amazon Elastic Compute Cloud - EC2** và các thành phần liên quan khi triển khai máy chủ ảo trên AWS. Nội dung tuần này thuộc nhóm **Explore / Khám phá dịch vụ AWS**, trong đó AWS Study Group có đề cập đến triển khai và tối ưu dịch vụ tính toán, bao gồm EC2, Auto Scaling và các thành phần hỗ trợ vận hành ứng dụng. ([Cloud Journey][1])

Các nội dung trọng tâm của tuần bao gồm:

* Tìm hiểu tổng quan về Amazon EC2.
* Tìm hiểu AMI, Instance Type, Key Pair và Security Group.
* Thực hành khởi tạo Linux EC2 Instance.
* Tìm hiểu cách kết nối vào EC2 bằng SSH.
* Tìm hiểu cách thay đổi cấu hình EC2 Instance.
* Tìm hiểu Elastic Load Balancer và Auto Scaling Group.
* Ghi chú các lỗi thường gặp khi triển khai EC2.

---

## Các công việc cần triển khai trong tuần này

| Thứ tự | Công việc thực hiện                                                                                                          | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| --- | --- | --- | --- | --- |
| **1**  | Tìm hiểu tổng quan về Amazon EC2, vai trò của EC2 trong việc tạo máy chủ ảo và triển khai ứng dụng trên AWS.                 | 11/05/2026 | 11/05/2026 | [https://cloudjourney.awsstudygroup.com/vi/1-explore/](https://cloudjourney.awsstudygroup.com/vi/1-explore/) <br> [https://000004.awsstudygroup.com/vi/](https://000004.awsstudygroup.com/vi/) <br> [https://000004.awsstudygroup.com/vi/1-introduce/](https://000004.awsstudygroup.com/vi/1-introduce/)                                                                                                                                                                                                             |
| **2**  | Tìm hiểu AMI, Instance Type, Key Pair, EBS và Security Group khi khởi tạo EC2 Instance.                                      | 12/05/2026 | 12/05/2026 | [https://000004.awsstudygroup.com/vi/1-introduce/](https://000004.awsstudygroup.com/vi/1-introduce/) <br> [https://000004.awsstudygroup.com/vi/2-prerequiste/2.3-createsecuritygrouplinux/](https://000004.awsstudygroup.com/vi/2-prerequiste/2.3-createsecuritygrouplinux/)                                                                                                                                                                                                                                         |
| **3**  | Thực hành tạo Linux EC2 Instance, chọn Amazon Linux 2023 AMI, cấu hình Key Pair, VPC, Subnet và Security Group.              | 13/05/2026 | 13/05/2026 | [https://000004.awsstudygroup.com/vi/4-launchlinuxinstance/](https://000004.awsstudygroup.com/vi/4-launchlinuxinstance/) <br> [https://000004.awsstudygroup.com/vi/4-launchlinuxinstance/4.1-createlinuxinstance/](https://000004.awsstudygroup.com/vi/4-launchlinuxinstance/4.1-createlinuxinstance/)                                                                                                                                                                                                               |
| **4**  | Tìm hiểu cách kết nối vào Linux EC2 Instance bằng SSH, kiểm tra trạng thái instance và xử lý lỗi kết nối thường gặp.         | 14/05/2026 | 14/05/2026 | [https://000004.awsstudygroup.com/vi/4-launchlinuxinstance/4.2-connectlinuxinstance/](https://000004.awsstudygroup.com/vi/4-launchlinuxinstance/4.2-connectlinuxinstance/) <br> [https://000004.awsstudygroup.com/vi/5-amazonec2basic/5.1-changeconfigureec2/](https://000004.awsstudygroup.com/vi/5-amazonec2basic/5.1-changeconfigureec2/)                                                                                                                                                                         |
| **5**  | Tìm hiểu Load Balancer, Auto Scaling Group, EBS Snapshot và dọn dẹp tài nguyên sau khi thực hành để tránh phát sinh chi phí. | 15/05/2026 | 15/05/2026 | [https://000006.awsstudygroup.com/vi/](https://000006.awsstudygroup.com/vi/) <br> [https://000006.awsstudygroup.com/vi/4-setup-load-balancer/](https://000006.awsstudygroup.com/vi/4-setup-load-balancer/) <br> [https://000006.awsstudygroup.com/vi/6-create-auto-scaling-group/](https://000006.awsstudygroup.com/vi/6-create-auto-scaling-group/) <br> [https://000004.awsstudygroup.com/vi/5-amazonec2basic/5.2-createec2snapshot/](https://000004.awsstudygroup.com/vi/5-amazonec2basic/5.2-createec2snapshot/) |

---

## Kết quả đạt được tuần 4

### Tổng quan

Trong tuần này, tôi đã tìm hiểu về **Amazon EC2**, dịch vụ máy chủ ảo cốt lõi của AWS. Amazon EC2 cho phép khởi tạo máy chủ ảo nhanh chóng, lựa chọn cấu hình theo nhu cầu sử dụng và triển khai nhiều loại workload như website, ứng dụng, cơ sở dữ liệu hoặc backend service. ([Aws Study Group][2])

### Kiến thức đã học

Sau khi hoàn thành tuần 4, tôi đã nắm được:

* Hiểu được vai trò của **Amazon EC2** trong việc cung cấp tài nguyên tính toán trên AWS.
* Hiểu khái niệm **AMI - Amazon Machine Image**, dùng làm mẫu để khởi tạo EC2 Instance.
* Hiểu **Instance Type** ảnh hưởng đến CPU, RAM, network và storage của máy chủ ảo.
* Hiểu **Key Pair** dùng để xác thực khi kết nối vào EC2 Instance và cần bảo vệ private key cẩn thận. ([Aws Study Group][3])
* Biết cách cấu hình **Security Group** để kiểm soát lưu lượng truy cập vào và ra khỏi EC2 Instance.
* Hiểu vai trò của **EBS Snapshot** trong sao lưu dữ liệu và khôi phục hệ thống. ([Aws Study Group][4])
* Hiểu cơ bản về **Elastic Load Balancer** và **Auto Scaling Group** trong việc phân phối tải và tự động mở rộng số lượng instance. ([Aws Study Group][5])

### Thực hành

Trong quá trình học và thực hành, tôi đã thực hiện được các nội dung sau:

* Truy cập dịch vụ EC2 trên AWS Management Console.
* Tìm hiểu quy trình tạo EC2 Instance.
* Chọn Amazon Linux 2023 AMI khi khởi tạo máy chủ ảo.
* Cấu hình Instance Type, Key Pair, VPC, Subnet và Security Group.
* Thiết lập rule cho Security Group, bao gồm SSH, HTTP và HTTPS.
* Kết nối vào Linux EC2 Instance bằng SSH.
* Kiểm tra trạng thái hoạt động của instance.
* Tìm hiểu cách thay đổi cấu hình EC2 Instance Type khi cần nâng cấp tài nguyên.
* Tìm hiểu quy trình tạo EBS Snapshot để sao lưu dữ liệu.
* Tìm hiểu Load Balancer và Auto Scaling Group để tăng tính sẵn sàng, khả năng mở rộng và tối ưu vận hành hệ thống.
* Ghi chú các lỗi thường gặp như chưa mở port 22, sai key pair, instance chưa có public IP, chọn sai subnet hoặc security group chưa cho phép truy cập.

---

## Tóm tắt tuần 4

**Tuần 4:** Tìm hiểu EC2, AMI, Instance Type, Key Pair, Security Group, EBS Snapshot, Load Balancer và Auto Scaling. Nắm được cách khởi tạo máy chủ ảo, kết nối vào EC2 Instance, cấu hình bảo mật truy cập và tìm hiểu cơ chế mở rộng hệ thống trên AWS.

[1]: https://cloudjourney.awsstudygroup.com/vi/1-explore/ "Khám phá dịch vụ AWS :: Hành trình đầu tiên lên Mây"
[2]: https://000004.awsstudygroup.com/vi/1-introduce/ "Giới thiệu :: GIỚI THIỆU VỀ AMAZON EC2"
[3]: https://000004.awsstudygroup.com/vi/4-launchlinuxinstance/4.1-createlinuxinstance/ "Tạo Linux instance :: GIỚI THIỆU VỀ AMAZON EC2"
[4]: https://000004.awsstudygroup.com/vi/5-amazonec2basic/5.2-createec2snapshot/ "Tạo và quản lý EBS Snapshots :: GIỚI THIỆU VỀ AMAZON EC2"
[5]: https://000006.awsstudygroup.com/vi/ "Triển khai ứng dụng FCJ Management với Auto Scaling Group :: TRIỂN KHAI ỨNG DỤNG FCJ MANAGEMENT VỚI AUTO SCALING GROUP"
