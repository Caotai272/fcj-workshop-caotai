---
title: "Worklog Tuần 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---


# Worklog Tuần 3

## Mục tiêu tuần 3

Trong tuần 3, mục tiêu chính là tìm hiểu về **Amazon Virtual Private Cloud - Amazon VPC** và các thành phần mạng cơ bản trên AWS. Đây là dịch vụ dùng để xây dựng môi trường mạng riêng, giúp triển khai các tài nguyên AWS như EC2, database hoặc các dịch vụ backend trong một hệ thống mạng có kiểm soát.

Nội dung tuần này thuộc nhóm **Explore / Khám phá dịch vụ AWS**, trong đó AWS Study Group có đề cập đến kiến trúc mạng với VPC và các mẫu thiết kế hạ tầng mạng trên AWS. ([cloudjourney.awsstudygroup.com][1]) Workshop Amazon VPC cũng tập trung vào việc thiết kế, triển khai và quản lý môi trường mạng riêng trên AWS Cloud. ([000003.awsstudygroup.com][2])

Các nội dung trọng tâm của tuần bao gồm:

* Tìm hiểu tổng quan về Amazon VPC.
* Tìm hiểu Subnet, Route Table, Internet Gateway và NAT Gateway.
* Phân biệt Public Subnet và Private Subnet.
* Tìm hiểu Security Group và Network ACL.
* Thực hành tạo VPC, Subnet, Internet Gateway, Route Table và Security Group.
* Ghi chú các lỗi thường gặp khi cấu hình mạng trên AWS.

---

## Các công việc cần triển khai trong tuần này

| Thứ tự | Công việc thực hiện                                                                                                                       | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| --- | --- | --- | --- | --- |
| **1**  | Tìm hiểu tổng quan về Amazon VPC, vai trò của VPC trong việc tạo môi trường mạng riêng trên AWS Cloud.                                    | 04/05/2026 | 04/05/2026 | [https://cloudjourney.awsstudygroup.com/vi/1-explore/](https://cloudjourney.awsstudygroup.com/vi/1-explore/) <br> [https://000003.awsstudygroup.com/vi/](https://000003.awsstudygroup.com/vi/) <br> [https://000003.awsstudygroup.com/vi/1-introduce/](https://000003.awsstudygroup.com/vi/1-introduce/)                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **2**  | Tìm hiểu Subnet và Route Table, phân biệt Public Subnet, Private Subnet và cách định tuyến lưu lượng trong VPC.                           | 05/05/2026 | 05/05/2026 | [https://000003.awsstudygroup.com/vi/1-introduce/1.1-subnets/](https://000003.awsstudygroup.com/vi/1-introduce/1.1-subnets/) <br> [https://000003.awsstudygroup.com/vi/1-introduce/1.2-routetable/](https://000003.awsstudygroup.com/vi/1-introduce/1.2-routetable/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **3**  | Tìm hiểu Internet Gateway và NAT Gateway, vai trò của từng thành phần trong việc kết nối tài nguyên AWS với Internet.                     | 06/05/2026 | 06/05/2026 | [https://000003.awsstudygroup.com/vi/1-introduce/1.3-internetgateway/](https://000003.awsstudygroup.com/vi/1-introduce/1.3-internetgateway/) <br> [https://000003.awsstudygroup.com/vi/1-introduce/1.4-natgateway/](https://000003.awsstudygroup.com/vi/1-introduce/1.4-natgateway/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **4**  | Tìm hiểu tường lửa trong VPC, Security Group và Network ACL để kiểm soát lưu lượng truy cập vào/ra tài nguyên AWS.                        | 07/05/2026 | 07/05/2026 | [https://000003.awsstudygroup.com/vi/2-firewallinvpc/](https://000003.awsstudygroup.com/vi/2-firewallinvpc/) <br> [https://000003.awsstudygroup.com/vi/2-firewallinvpc/2.1-securitygroup/](https://000003.awsstudygroup.com/vi/2-firewallinvpc/2.1-securitygroup/) <br> [https://000003.awsstudygroup.com/vi/2-firewallinvpc/2.2-networkacls/](https://000003.awsstudygroup.com/vi/2-firewallinvpc/2.2-networkacls/)                                                                                                                                                                                                                                                                                                                                           |
| **5**  | Thực hành tạo VPC, Subnet, Internet Gateway, Route Table và Security Group; kiểm tra lại mô hình mạng và ghi chú lỗi cấu hình thường gặp. | 08/05/2026 | 08/05/2026 | [https://000003.awsstudygroup.com/vi/3-prerequisite/3.1-createvpc/](https://000003.awsstudygroup.com/vi/3-prerequisite/3.1-createvpc/) <br> [https://000003.awsstudygroup.com/vi/3-prerequisite/3.2-createsubnet/](https://000003.awsstudygroup.com/vi/3-prerequisite/3.2-createsubnet/) <br> [https://000003.awsstudygroup.com/vi/3-prerequisite/3.3-createigw/](https://000003.awsstudygroup.com/vi/3-prerequisite/3.3-createigw/) <br> [https://000003.awsstudygroup.com/vi/3-prerequisite/3.4-createroutetable/](https://000003.awsstudygroup.com/vi/3-prerequisite/3.4-createroutetable/) <br> [https://000003.awsstudygroup.com/vi/3-prerequisite/3.5-createsecuritygroup/](https://000003.awsstudygroup.com/vi/3-prerequisite/3.5-createsecuritygroup/) |

---

## Kết quả đạt được tuần 3

### Tổng quan

Trong tuần này, tôi đã tìm hiểu về **Amazon VPC** và các thành phần mạng quan trọng khi triển khai hệ thống trên AWS. Amazon VPC cho phép tạo một môi trường mạng ảo riêng biệt trong AWS Cloud, có thể tùy chỉnh dải địa chỉ IP, phân chia subnet và cấu hình định tuyến theo nhu cầu triển khai hệ thống. ([000003.awsstudygroup.com][3])

### Kiến thức đã học

Sau khi hoàn thành tuần 3, tôi đã nắm được:

* Hiểu được vai trò của **Amazon VPC** trong kiến trúc hạ tầng AWS.
* Biết cách phân biệt **Public Subnet** và **Private Subnet**.
* Hiểu vai trò của **Route Table** trong việc điều hướng lưu lượng mạng.
* Hiểu **Internet Gateway** dùng để cho phép tài nguyên trong public subnet kết nối Internet.
* Hiểu **NAT Gateway** giúp tài nguyên trong private subnet truy cập Internet theo chiều đi ra.
* Hiểu sự khác nhau giữa **Security Group** và **Network ACL**.
* Nắm được quy trình cơ bản để tạo VPC, subnet, route table, internet gateway và security group.

### Thực hành

Trong quá trình học và thực hành, tôi đã thực hiện được các nội dung sau:

* Truy cập dịch vụ VPC trên AWS Management Console.
* Tìm hiểu cấu trúc một VPC cơ bản.
* Thực hành tạo VPC với dải CIDR phù hợp.
* Tạo public subnet và private subnet.
* Tạo Internet Gateway và gắn vào VPC.
* Cấu hình Route Table cho public subnet.
* Tạo Security Group để kiểm soát truy cập.
* Ghi chú các lỗi thường gặp như thiếu route ra Internet, chưa gắn Internet Gateway, cấu hình sai Security Group hoặc chưa mở port cần thiết.

---

## Tóm tắt tuần 3

**Tuần 3:** Tìm hiểu VPC, Subnet, Route Table, Internet Gateway, NAT Gateway, Security Group và Network ACL. Nắm được cách xây dựng mô hình mạng cơ bản trên AWS, phân chia public/private subnet và kiểm soát lưu lượng truy cập bằng các thành phần bảo mật mạng.

[1]: https://cloudjourney.awsstudygroup.com/vi/1-explore/ "Khám phá dịch vụ AWS :: Hành trình đầu tiên lên Mây"
[2]: https://000003.awsstudygroup.com/vi/ "Bắt đầu với Amazon Virtual Private Cloud (VPC) và AWS Site-to-Site VPN :: Bắt đầu với Amazon VPC và AWS VPN Site to Site"
[3]: https://000003.awsstudygroup.com/vi/1-introduce/ "Giới thiệu :: Bắt đầu với Amazon VPC và AWS VPN Site to Site"
