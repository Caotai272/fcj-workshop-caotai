---
title: "Worklog Tuần 5"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---


# Worklog Tuần 5

## Mục tiêu tuần 5

Trong tuần 5, mục tiêu chính là tìm hiểu các công cụ kiểm thử bảo mật ứng dụng và hệ thống gồm **HCL AppScan, Nessus và Burp Suite**. Đây là các công cụ thường được sử dụng để hỗ trợ phát hiện lỗ hổng bảo mật, đánh giá rủi ro và kiểm tra mức độ an toàn của ứng dụng hoặc hệ thống trong phạm vi được phép.

HCL AppScan hỗ trợ các hình thức kiểm thử bảo mật ứng dụng như DAST, SAST, IAST và kiểm tra thành phần mã nguồn mở; Nessus là công cụ đánh giá lỗ hổng hệ thống; Burp Suite là bộ công cụ kiểm thử bảo mật ứng dụng web do PortSwigger phát triển. ([HCL SW Blogs][1])

Các nội dung trọng tâm của tuần bao gồm:

* Tìm hiểu tổng quan về kiểm thử bảo mật ứng dụng và hệ thống.
* Tìm hiểu vai trò của **HCL AppScan** trong kiểm thử bảo mật ứng dụng.
* Tìm hiểu vai trò của **Nessus** trong quét và đánh giá lỗ hổng hệ thống.
* Tìm hiểu vai trò của **Burp Suite** trong phân tích request/response và kiểm thử ứng dụng web.
* Tham khảo OWASP Web Security Testing Guide để nắm quy trình kiểm thử bảo mật web cơ bản.
* Ghi chú nguyên tắc chỉ kiểm thử trên hệ thống được cấp quyền, môi trường lab hoặc ứng dụng demo.

---

## Các công việc cần triển khai trong tuần này

| Thứ tự | Công việc thực hiện                                                                                                                                                          | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                                                                                                                                                                                                                                                                                             |
| --- | --- | --- | --- | --- |
| **1**  | Tìm hiểu tổng quan về kiểm thử bảo mật ứng dụng, đánh giá lỗ hổng và vai trò của security testing trong quá trình phát triển, triển khai hệ thống.                           | 18/05/2026 | 18/05/2026 | [https://owasp.org/www-project-web-security-testing-guide/](https://owasp.org/www-project-web-security-testing-guide/) <br> [https://cloudjourney.awsstudygroup.com/vi/3-optimize/](https://cloudjourney.awsstudygroup.com/vi/3-optimize/)                                                                                                                                                                                                 |
| **2**  | Tìm hiểu HCL AppScan, các chức năng kiểm thử bảo mật ứng dụng như quét ứng dụng web, kiểm tra mã nguồn và hỗ trợ phát hiện lỗ hổng trong quá trình phát triển phần mềm.      | 19/05/2026 | 19/05/2026 | [https://www.hcl-software.com/appscan/documentation-and-support](https://www.hcl-software.com/appscan/documentation-and-support) <br> [https://help.hcl-software.com/appscan/Welcome.html](https://help.hcl-software.com/appscan/Welcome.html)                                                                                                                                                                                             |
| **3**  | Tìm hiểu Nessus, vai trò của công cụ trong việc quét lỗ hổng hệ thống, kiểm tra cấu hình, phát hiện điểm yếu bảo mật trên máy chủ hoặc hạ tầng mạng trong phạm vi được phép. | 20/05/2026 | 20/05/2026 | [https://docs.tenable.com/Nessus.htm](https://docs.tenable.com/Nessus.htm) <br> [https://docs.tenable.com/](https://docs.tenable.com/)                                                                                                                                                                                                                                                                                                     |
| **4**  | Tìm hiểu Burp Suite, cách công cụ hỗ trợ kiểm thử ứng dụng web thông qua phân tích request/response, proxy, scanner và các chức năng phục vụ kiểm thử bảo mật web.           | 21/05/2026 | 21/05/2026 | [https://portswigger.net/burp](https://portswigger.net/burp) <br> [https://portswigger.net/burp/documentation](https://portswigger.net/burp/documentation)                                                                                                                                                                                                                                                                                 |
| **5**  | So sánh mục đích sử dụng của HCL AppScan, Nessus và Burp Suite; tổng hợp ưu điểm, phạm vi áp dụng và ghi chú nguyên tắc kiểm thử an toàn, hợp pháp.                          | 22/05/2026 | 22/05/2026 | [https://owasp.org/www-project-web-security-testing-guide/](https://owasp.org/www-project-web-security-testing-guide/) <br> [https://www.hcl-software.com/appscan/documentation-and-support](https://www.hcl-software.com/appscan/documentation-and-support) <br> [https://docs.tenable.com/Nessus.htm](https://docs.tenable.com/Nessus.htm) <br> [https://portswigger.net/burp/documentation](https://portswigger.net/burp/documentation) |

---

## Kết quả đạt được tuần 5

### Tổng quan

Trong tuần này, tôi đã tìm hiểu các công cụ kiểm thử bảo mật gồm **HCL AppScan, Nessus và Burp Suite**. Các công cụ này có phạm vi sử dụng khác nhau: AppScan tập trung vào kiểm thử bảo mật ứng dụng, Nessus tập trung vào đánh giá lỗ hổng hệ thống, còn Burp Suite hỗ trợ kiểm thử bảo mật ứng dụng web ở mức request/response và phân tích thủ công. ([HCL SW Blogs][1])

### Kiến thức đã học

Sau khi hoàn thành tuần 5, tôi đã nắm được:

* Hiểu vai trò của kiểm thử bảo mật trong quy trình phát triển và triển khai hệ thống.
* Hiểu **HCL AppScan** có thể hỗ trợ kiểm thử bảo mật ứng dụng thông qua các hình thức như DAST, SAST, IAST và kiểm tra thành phần mã nguồn mở. ([HCL SW Blogs][1])
* Hiểu **Nessus** được sử dụng để đánh giá lỗ hổng, kiểm tra cấu hình và hỗ trợ phát hiện điểm yếu trên hệ thống. ([docs.tenable.com][2])
* Hiểu **Burp Suite** là bộ công cụ hỗ trợ kiểm thử bảo mật ứng dụng web, bao gồm các chức năng liên quan đến proxy, scanner và phân tích luồng request/response. ([portswigger.net][3])
* Biết tham khảo **OWASP Web Security Testing Guide** như một tài liệu nền tảng khi tìm hiểu quy trình kiểm thử bảo mật ứng dụng web. ([OWASP Foundation][4])
* Nhận thức được việc kiểm thử bảo mật chỉ nên thực hiện trên hệ thống được cho phép, môi trường lab hoặc ứng dụng demo.

### Thực hành

Trong quá trình học và tìm hiểu, tôi đã thực hiện được các nội dung sau:

* Tìm hiểu khái niệm security testing, vulnerability assessment và web application security testing.
* Tìm hiểu giao diện, mục đích sử dụng và nhóm chức năng chính của HCL AppScan.
* Tìm hiểu Nessus và vai trò của công cụ trong việc quét lỗ hổng hệ thống.
* Tìm hiểu Burp Suite và cách công cụ hỗ trợ phân tích request/response trong ứng dụng web.
* Tham khảo OWASP Web Security Testing Guide để nắm các nhóm kiểm thử phổ biến.
* Lập bảng so sánh cơ bản giữa HCL AppScan, Nessus và Burp Suite.
* Ghi chú các lưu ý về phạm vi kiểm thử, quyền được phép kiểm thử và an toàn khi sử dụng công cụ bảo mật.

---

## Bảng so sánh công cụ

| Công cụ         | Mục đích chính                | Phạm vi sử dụng                                         |
| --------------- | ----------------------------- | ------------------------------------------------------- |
| **HCL AppScan** | Kiểm thử bảo mật ứng dụng     | Ứng dụng web, mã nguồn, runtime, thành phần mã nguồn mở |
| **Nessus**      | Đánh giá lỗ hổng hệ thống     | Máy chủ, thiết bị mạng, hệ điều hành, cấu hình dịch vụ  |
| **Burp Suite**  | Kiểm thử bảo mật ứng dụng web | Request/response, proxy, kiểm thử thủ công và scanner   |

---

## Tóm tắt tuần 5

**Tuần 5:** Tìm hiểu HCL AppScan, Nessus và Burp Suite để kiểm thử bảo mật ứng dụng và hệ thống. Nắm được mục đích sử dụng của từng công cụ, phạm vi áp dụng, cách tham khảo tài liệu kiểm thử bảo mật web theo OWASP và các nguyên tắc kiểm thử an toàn trong môi trường được cấp quyền.

[1]: https://www.hcl-software.com/appscan/documentation-and-support?utm_source=chatgpt.com "HCL AppScan Documentation and Support"
[2]: https://docs.tenable.com/Nessus.htm?utm_source=chatgpt.com "Tenable Nessus"
[3]: https://portswigger.net/burp/documentation?utm_source=chatgpt.com "Burp Suite documentation"
[4]: https://owasp.org/www-project-web-security-testing-guide/?utm_source=chatgpt.com "OWASP Web Security Testing Guide"
