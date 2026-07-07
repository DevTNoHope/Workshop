---
title: "Nhật ký công việc Tuần 2"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Triển khai giải pháp cân bằng tải và tự động mở rộng tài nguyên (ELB & Auto Scaling).
* Sử dụng dịch vụ Amazon CloudWatch để giám sát hệ thống và Route 53 Resolver cho Hybrid DNS.
* Tự động hóa thao tác vận hành với AWS CLI và thiết lập bảo vệ dữ liệu với AWS Backup.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Triển khai Auto Scaling kết hợp Application Load Balancer (ALB) trong môi trường Multi-AZ.<br>- Tạo Launch Template cho EC2 và cấu hình Target Groups.<br>- Cấu hình chính sách mở rộng tự động (Scaling Policies) và kiểm tra khả năng chịu lỗi (Failover). | 27/04/2026 | 27/04/2026 | <https://000006.awsstudygroup.com/> |
| 3 | - Nghiên cứu dịch vụ Amazon CloudWatch: Metrics, Logs và Alarms.<br>- Thiết lập bảng điều khiển (Dashboards) trực quan hóa thông tin giám sát và cấu hình cảnh báo SNS khi quá tải hệ thống. | 28/04/2026 | 28/04/2026 | <https://000008.awsstudygroup.com/> |
| 4 | - Thiết lập Hybrid DNS tích hợp hệ thống phân giải DNS on-premises và AWS Route 53.<br>- Tạo Route 53 Inbound/Outbound Endpoints và định cấu hình Resolver Rules để phân giải DNS hai chiều. | 29/04/2026 | 29/04/2026 | <https://000010.awsstudygroup.com/> |
| 5 | - Cài đặt và cấu hình AWS CLI v2 trên máy trạm.<br>- Thực hành quản trị tài nguyên (S3, IAM, VPC, EC2, SNS) qua dòng lệnh và viết scripts tự động hóa các tác vụ quản trị cơ bản. | 30/04/2026 | 30/04/2026 | <https://000011.awsstudygroup.com/> |
| 6 | - Triển khai AWS Backup bảo vệ dữ liệu trên S3, EC2 và RDS.<br>- Thiết lập Backup Plans, quy định thời gian lưu trữ (Retention Policies) và kiểm tra kịch bản khôi phục (Restore). | 01/05/2026 | 01/05/2026 | <https://000013.awsstudygroup.com/> |

### Kết quả đạt được tuần 2:

* **Tự động mở rộng & Cân bằng tải (ELB/ASG)**: Xây dựng thành công hệ thống tự động co giãn tài nguyên theo tải thực tế dựa trên Launch Template, tối ưu hóa lưu lượng truy cập qua Application Load Balancer.
* **Giám sát hệ thống (CloudWatch)**: Dựng dashboard giám sát hiệu năng tập trung cho EC2/RDS, kích hoạt cảnh báo tự động gửi email qua SNS khi tài nguyên đạt ngưỡng giới hạn.
* **Hybrid DNS (Route 53 Resolver)**: Kết nối thành công hệ thống phân giải tên miền giữa môi trường mô phỏng On-Premises (Microsoft Active Directory AD) và AWS Private Hosted Zones.
* **Quản trị qua dòng lệnh (AWS CLI)**: Thành thạo các lệnh quản lý tài nguyên cốt lõi, sử dụng bộ lọc truy vấn nâng cao (JMESPath) để kết xuất dữ liệu và tối ưu vận hành bằng kịch bản tự động.
* **Bảo vệ dữ liệu (AWS Backup)**: Cấu hình tập trung lịch trình sao lưu dữ liệu cho EC2/RDS, kiểm tra quy trình khôi phục dữ liệu hoạt động chính xác đảm bảo an toàn hệ thống.
