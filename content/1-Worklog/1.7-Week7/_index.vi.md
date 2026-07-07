---
title: "Nhật ký công việc Tuần 7"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Quản lý giám sát hệ thống nâng cao với Amazon CloudWatch (Metric Expressions, Logs Insights).
* Triển khai hạ tầng dạng mã (IaC) sử dụng AWS CloudFormation và AWS Cloud Development Kit (CDK).
* Làm chủ hệ thống cơ sở dữ liệu NoSQL DynamoDB và xây dựng nền tảng phân tích báo cáo chi phí (Glue & Athena).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Triển khai giám sát CloudWatch nâng cao: sử dụng Search/Math expressions và Dynamic Labels.<br>- Cấu hình CloudWatch Logs, sử dụng Logs Insights viết câu lệnh SQL phân tích log và thiết lập Metric Filters kích hoạt Alarms tự động. | 01/06/2026 | 01/06/2026 | <https://000036.awsstudygroup.com/> |
| 3 | - Nghiên cứu nguyên lý Infrastructure as Code (IaC) với AWS CloudFormation.<br>- Viết template deploy EC2 nâng cao sử dụng Custom Resources (gọi Lambda), Mappings, StackSets đa vùng/đa tài khoản và chạy Drift Detection. | 02/06/2026 | 02/06/2026 | <https://000037.awsstudygroup.com/> |
| 4 | - Tìm hiểu AWS Cloud Development Kit (CDK) định nghĩa hạ tầng bằng mã ngôn ngữ lập trình.<br>- Triển khai CDK Stacks (VPC, S3, EC2), chạy cdk bootstrap/deploy trên Cloud9 và tích hợp User Data cài đặt ứng dụng tự động. | 03/06/2026 | 03/06/2026 | <https://000038.awsstudygroup.com/> |
| 5 | - Nghiên cứu cơ sở dữ liệu NoSQL Amazon DynamoDB: CLI, Console, nạp dữ liệu mẫu.<br>- Thực hành truy xuất dữ liệu nâng cao (Query vs Scan), cấu hình chỉ mục phụ GSI, thực hiện giao dịch Transactions và cấu hình PITR sao lưu tự động. | 04/06/2026 | 04/06/2026 | <https://000039.awsstudygroup.com/> |
| 6 | - Xây dựng nền tảng phân tích báo cáo chi phí CUR bằng AWS Glue và Amazon Athena.<br>- Tạo bảng trong Glue Data Catalog từ file Parquet trên S3 và viết các câu lệnh SQL tối ưu hóa chi phí (Top accounts/services, Tag-based, RI vs On-Demand). | 05/06/2026 | 05/06/2026 | <https://000040.awsstudygroup.com/> |

### Kết quả đạt được tuần 7:

* **Giám sát nâng cao (CloudWatch)**: Sử dụng thành thạo CloudWatch Logs Insights phân tích nhanh log hệ thống, thiết lập Metric Filters tự động đếm lỗi hệ thống và dựng Dashboards theo dõi tập trung.
* **Hạ tầng dạng mã (CloudFormation)**: Tạo thành công template triển khai hạ tầng tự động, tích hợp Custom Resource cấu hình sâu cho EC2 và sử dụng Drift Detection rà soát cấu hình sai lệch thực tế.
* **Định nghĩa hạ tầng bằng Code (CDK)**: Tận dụng sức mạnh ngôn ngữ lập trình (TypeScript) định nghĩa và cdk deploy các stack tài nguyên đám mây nhanh chóng, tự động hóa cấu hình máy chủ qua User Data.
* **Cơ sở dữ liệu NoSQL (DynamoDB)**: Thiết kế bảng DynamoDB tối ưu, cải tiến tốc độ truy vấn phi khóa chính qua Global Secondary Indexes (GSI), thực thi giao dịch ACID an toàn và cấu hình PITR bảo vệ dữ liệu.
* **Phân tích chi phí nâng cao (CUR)**: Xây dựng hoàn chỉnh nền tảng phân tích chi phí CUR bằng Athena, chạy các truy vấn SQL bóc tách chi phí chi tiết theo thẻ CostCenter, theo dõi hiệu quả mua Reserved Instances và Savings Plans.
