---
title: "Nhật ký công việc Tuần 5"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Triển khai hệ thống lưu trữ tập trung dùng chung cho Windows (Amazon FSx) và tường lửa bảo vệ ứng dụng (AWS WAF).
* Nghiên cứu chiến lược quản lý tài nguyên (Tagging, Resource Groups) và kiểm soát quyền truy cập dựa trên thuộc tính (ABAC).
* Thiết lập hệ thống giám sát đồ họa trực quan (Grafana) và bảo mật nâng cao với IAM Permission Boundary.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Triển khai Amazon FSx for Windows File Server SSD/HDD Multi-AZ.<br>- Ánh xạ thư mục chia sẻ mặc định lên client, kiểm tra hiệu năng, cấu hình Data Deduplication (chống trùng lặp) và Shadow Copies. | 18/05/2026 | 18/05/2026 | <https://000025.awsstudygroup.com/> |
| 3 | - Nghiên cứu tường lửa AWS WAF chống lại các mối đe dọa bảo mật phổ biến (OWASP Top 10).<br>- Triển khai ứng dụng web mẫu (OWASP Juice Shop), tạo Web ACL từ WAF console và thiết lập các rule ngăn chặn SQL Injection, XSS. | 19/05/2026 | 19/05/2026 | <https://000026.awsstudygroup.com/> |
| 4 | - Xây dựng chiến lược quản lý tài nguyên bằng Resource Tagging.<br>- Cấu hình Resource Groups phân loại tài nguyên và áp dụng IAM Policy kiểm soát truy cập dựa trên Tags (ABAC - Attribute-Based Access Control). | 20/05/2026 | 20/05/2026 | <https://000027.awsstudygroup.com/><br><https://000028.awsstudygroup.com/> |
| 5 | - Cài đặt Grafana Server trên máy chủ Linux EC2.<br>- Cấu hình IAM Role thu thập dữ liệu CloudWatch, thiết lập data source và xây dựng Dashboard hiển thị trực quan các số liệu tài nguyên. | 21/05/2026 | 21/05/2026 | <https://000029.awsstudygroup.com/> |
| 6 | - Nghiên cứu IAM Permission Boundary ngăn chặn leo thang đặc quyền (privilege escalation).<br>- Tạo Restriction Policy giới hạn quyền hạn cao nhất của người dùng và kiểm thử chặn các thao tác ngoài phạm vi cho phép. | 22/05/2026 | 22/05/2026 | <https://000030.awsstudygroup.com/> |

### Kết quả đạt được tuần 5:

* **Hệ thống lưu trữ Windows (FSx)**: Triển khai thành công hệ thống tệp tin FSx có tính khả dụng cao, tiết kiệm dung lượng qua Data Deduplication và kích hoạt Shadow Copies cho phép người dùng tự khôi phục file cũ.
* **Bảo vệ ứng dụng Web (WAF)**: Ngăn chặn thành công các đòn tấn công mô phỏng (SQLi, XSS, DDoS) bằng WAF Web ACL tích hợp các rule tùy chỉnh, tối ưu hóa bảo mật hệ thống.
* **Kiểm soát quyền bằng Tag (ABAC)**: Thiết lập phân quyền động linh hoạt, kiểm soát quyền vận hành tài nguyên (Start/Stop EC2) dựa trên tag đính kèm mà không cần chỉnh sửa IAM Policy.
* **Giám sát trực quan (Grafana)**: Kết nối thành công nguồn dữ liệu CloudWatch trích xuất số liệu hiệu năng tài nguyên thời gian thực hiển thị trên Dashboard Grafana trực quan.
* **Giới hạn quyền hạn (Permission Boundary)**: Thiết lập rào chắn bảo mật tối đa cho tài khoản người dùng, loại bỏ hoàn toàn nguy cơ tự nâng cấp quyền quản trị ngoài tầm kiểm soát của quản trị viên.
