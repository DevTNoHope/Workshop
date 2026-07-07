---
title: "Nhật ký công việc Tuần 6"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Vận hành và quản lý máy chủ tập trung (SSM) và tối ưu hóa tài nguyên compute (Compute Optimizer).
* Triển khai mã hóa dữ liệu tĩnh (KMS) và kiểm toán hoạt động của tài khoản (CloudTrail & Athena).
* Phân tích chi phí chuyên sâu (Cost Explorer) và xây dựng kiến trúc Data Lake phục vụ phân tích dữ liệu lớn.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Quản trị máy chủ EC2 tập trung bằng AWS Systems Manager (SSM).<br>- Gán IAM Role SSM Core, sử dụng Patch Manager tự động vá lỗi hệ điều hành và Run Command thực thi script từ xa không cần mở cổng RDP/SSH. | 25/05/2026 | 25/05/2026 | <https://000031.awsstudygroup.com/> |
| 3 | - Thiết lập CloudWatch Agent trên EC2 thu thập memory metrics (% RAM).<br>- Cấu hình AWS Compute Optimizer phân tích tải hệ thống và trích xuất các đề xuất điều chỉnh kích thước máy chủ (Right-sizing) tối ưu. | 26/05/2026 | 26/05/2026 | <https://000032.awsstudygroup.com/> |
| 4 | - Tạo Customer Managed Key (CMK) trong AWS KMS để mã hóa dữ liệu tĩnh trên S3.<br>- Kích hoạt AWS CloudTrail ghi nhận lịch sử thao tác API, cấu hình lưu trữ log vào S3 và sử dụng Amazon Athena chạy truy vấn SQL kiểm toán dữ liệu log. | 27/05/2026 | 27/05/2026 | <https://000033.awsstudygroup.com/> |
| 5 | - Trực quan hóa chi phí theo AWS Well-Architected Framework bằng AWS Cost Explorer.<br>- Phân tích xu hướng chi phí theo Accounts/Services, đánh giá tỷ lệ sử dụng Savings Plans, Reserved Instances và phân tích chi phí truyền dữ liệu (Data Transfer). | 28/05/2026 | 28/05/2026 | <https://000034.awsstudygroup.com/> |
| 6 | - Xây dựng giải pháp Data Lake trên AWS: S3, Kinesis Firehose, AWS Glue, Athena và QuickSight.<br>- Cấu hình Firehose thu thập dữ liệu stream lưu vào S3, chạy Glue Crawler tạo catalog, phân tích bằng Athena và trực quan bằng QuickSight. | 29/05/2026 | 29/05/2026 | <https://000035.awsstudygroup.com/> |

### Kết quả đạt được tuần 6:

* **Quản trị hệ thống tập trung (SSM)**: Tự động hóa quét bản vá lỗi hệ điều hành trên máy chủ Windows qua Patch Manager, thực thi thành công lệnh shell từ xa qua Run Command.
* **Tối ưu hóa máy chủ (Right-sizing)**: Giám sát thành công dung lượng RAM của EC2 qua CloudWatch Agent, phân tích hiệu suất bằng Compute Optimizer để đưa ra các khuyến nghị nâng cấp/hạ cấp size máy chủ hợp lý.
* **Kiểm toán & Mã hóa dữ liệu**: Bảo mật dữ liệu S3 bằng mã hóa KMS CMK, ghi nhận toàn bộ hoạt động API thông qua CloudTrail và viết truy vấn SQL trên Athena để tìm kiếm dấu vết kiểm toán bảo mật nhanh chóng.
* **Quản lý chi phí (Cost Explorer)**: Hiểu rõ nguồn phát sinh chi phí truyền dữ liệu chéo vùng và tối ưu hóa kế hoạch mua Savings Plans hoặc Reserved Instances dựa trên báo cáo chi phí.
* **Hệ thống dữ liệu lớn (Data Lake)**: Xây dựng hoàn chỉnh luồng thu thập dữ liệu streaming thời gian thực (Kinesis), chuẩn hóa cấu hình bảng dữ liệu (Glue Crawler), truy vấn trực tiếp (Athena) và thiết kế bảng biểu phân tích bằng QuickSight.
