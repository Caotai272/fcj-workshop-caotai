---
title: "Worklog Tuần 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---


## Mục tiêu tuần 2

Trong tuần 2, mục tiêu chính là tìm hiểu dịch vụ **AWS Identity and Access Management - IAM**. Đây là dịch vụ dùng để quản lý danh tính, phân quyền truy cập và kiểm soát người dùng khi làm việc với tài nguyên AWS. IAM hỗ trợ quản lý **User, Group, Role và Policy**, đồng thời giúp áp dụng nguyên tắc phân quyền tối thiểu trong hệ thống. ([000002.awsstudygroup.com][1])

Nội dung trọng tâm của tuần bao gồm:

* Tìm hiểu tổng quan về AWS IAM.
* Tìm hiểu IAM User, IAM Group, IAM Role và IAM Policy.
* Thực hành tạo Group và User quản trị.
* Tìm hiểu cách gán quyền thông qua Policy.
* Tìm hiểu cách sử dụng IAM Role để cấp quyền truy cập tạm thời.
* Ghi chú các lưu ý bảo mật khi sử dụng IAM.

---

## Các công việc cần triển khai trong tuần này

| Thứ tự | Công việc thực hiện                                                                                                                        | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                           |
| --- | --- | --- | --- | --- |
| **1**  | Tìm hiểu tổng quan về AWS IAM, vai trò của IAM trong việc quản lý danh tính, xác thực và phân quyền truy cập tài nguyên AWS.               | 27/04/2026 | 27/04/2026 | [https://000002.awsstudygroup.com/vi/](https://000002.awsstudygroup.com/vi/)                                                             |
| **2**  | Tìm hiểu các thành phần chính của IAM gồm IAM User, IAM Group, IAM Role và IAM Policy.                                                     | 28/04/2026 | 28/04/2026 | [https://000002.awsstudygroup.com/vi/1-introduction/](https://000002.awsstudygroup.com/vi/1-introduction/)                               |
| **3**  | Tìm hiểu IAM Policy, cách Policy định nghĩa quyền truy cập và cách gán Policy cho User, Group hoặc Role.                                   | 29/04/2026 | 29/04/2026 | [https://000002.awsstudygroup.com/vi/1-introduction/1.2-iam-policy/](https://000002.awsstudygroup.com/vi/1-introduction/1.2-iam-policy/) |
| **4**  | Thực hành tạo IAM Group và IAM User, gán quyền quản trị cho Group và đăng nhập bằng IAM User.                                              | 30/04/2026 | 30/04/2026 | [https://000002.awsstudygroup.com/vi/2-create-admin-user-and-group/](https://000002.awsstudygroup.com/vi/2-create-admin-user-and-group/) |
| **5**  | Tìm hiểu IAM Role, cách cấp quyền tạm thời cho dịch vụ AWS hoặc người dùng khác, đồng thời ghi chú các nguyên tắc bảo mật khi sử dụng IAM. | 01/05/2026 | 01/05/2026 | [https://000002.awsstudygroup.com/vi/3-aws-role/](https://000002.awsstudygroup.com/vi/3-aws-role/)                                       |

---

## Kết quả đạt được tuần 2

### Tổng quan

Trong tuần này, tôi đã tìm hiểu dịch vụ **AWS IAM** và nắm được vai trò của IAM trong việc quản lý quyền truy cập trên AWS. IAM cho phép kiểm soát chi tiết ai được phép truy cập tài nguyên nào và được thực hiện hành động gì trên hệ thống AWS. ([Amazon Web Services, Inc.][2])

### Kiến thức đã học

Sau khi hoàn thành tuần 2, tôi đã nắm được:

* Hiểu được vai trò của IAM trong việc quản lý danh tính và quyền truy cập.
* Phân biệt được **IAM User**, **IAM Group**, **IAM Role** và **IAM Policy**.
* Hiểu được IAM Policy là tài liệu định nghĩa quyền truy cập chi tiết và có thể được gán cho User, Group hoặc Role. ([000002.awsstudygroup.com][3])
* Hiểu được IAM Role dùng để cấp quyền truy cập tạm thời cho User, dịch vụ AWS, tài khoản AWS khác hoặc ứng dụng bên ngoài. ([000002.awsstudygroup.com][4])
* Nắm được nguyên tắc **least privilege**, tức là chỉ cấp quyền cần thiết cho người dùng hoặc dịch vụ.
* Biết được vì sao không nên sử dụng tài khoản root cho các công việc hằng ngày.

### Thực hành

Trong quá trình học và thực hành, tôi đã thực hiện được các nội dung sau:

* Truy cập dịch vụ IAM trên AWS Management Console.
* Tìm hiểu cách tạo IAM Group.
* Tìm hiểu cách tạo IAM User.
* Gán Policy phù hợp cho IAM Group.
* Đăng nhập thử bằng IAM User.
* Tìm hiểu cách tạo IAM Role và trường hợp sử dụng Role cho các dịch vụ AWS.
* Ghi chú các lỗi thường gặp khi phân quyền sai hoặc thiếu Policy.

---

## Tóm tắt tuần 2

**Tuần 2:** Tìm hiểu IAM, quản lý User, Group, Role, Policy và phân quyền truy cập trên AWS. Nắm được cách IAM hỗ trợ xác thực, ủy quyền và kiểm soát quyền truy cập tài nguyên AWS theo nguyên tắc bảo mật tối thiểu.

[1]: https://000002.awsstudygroup.com/vi/?utm_source=chatgpt.com "Quản trị quyền truy cập với AWS IAM (Identity and Access ..."
[2]: https://aws.amazon.com/vi/iam/?utm_source=chatgpt.com "Quản lý danh tính và truy cập (IAM) trong AWS"
[3]: https://000002.awsstudygroup.com/vi/1-introduction/1.2-iam-policy/?utm_source=chatgpt.com "AWS Identity and Access Management (IAM) Policy"
[4]: https://000002.awsstudygroup.com/vi/1-introduction/1.3-iam-role/?utm_source=chatgpt.com "AWS Identity and Access Management (IAM) Role"
