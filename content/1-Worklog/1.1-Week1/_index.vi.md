---
title: "Nhật ký công việc Tuần 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Mục tiêu tuần 1:

* Làm quen với đơn vị thực tập FCAJ và tìm hiểu tổng quan các dịch vụ cốt lõi của AWS.
* Thiết lập tài khoản và các cơ chế bảo mật cơ bản như IAM và MFA.
* Nghiên cứu và triển khai hạ tầng mạng (VPC), máy chủ ảo (EC2) và cơ sở dữ liệu quan hệ (RDS).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Làm quen đơn vị thực tập FCAJ, nội quy và quy định.<br>- Tìm hiểu tổng quan dịch vụ AWS (Compute, Storage, Network, DB).<br>- Tạo tài khoản AWS Free Tier, thiết lập MFA và cấu hình AWS Budgets để quản lý chi phí. | 20/04/2026 | 20/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Nghiên cứu IAM Users, Groups và Roles.<br>- Tạo tài khoản Admin User và Admin Group với chính sách AdministratorAccess.<br>- Thực hành chuyển đổi Role (Switch Role) từ Operator sang Admin và cấu hình phân quyền tối thiểu. | 21/04/2026 | 21/04/2026 | <https://000002.awsstudygroup.com/> |
| 4 | - Tìm hiểu VPC cơ bản: CIDR, Subnets (Public/Private), Internet Gateway, NAT Gateway.<br>- Xây dựng kiến trúc mạng Multi-AZ, cấu hình Security Groups, Route Tables và Network ACLs.<br>- Thực hành cấu hình VPC Flow Logs và thiết lập AWS Site-to-Site VPN. | 22/04/2026 | 22/04/2026 | <https://000003.awsstudygroup.com/> |
| 5 | - Nghiên cứu Amazon EC2, AMI, Instance Types và EBS volumes.<br>- Triển khai ứng dụng Node.js và cài đặt MySQL trên cả hai môi trường Linux (Amazon Linux 2023) và Windows Server 2025.<br>- Cấu hình PM2 quản lý tiến trình và Nginx làm Reverse Proxy. | 23/04/2026 | 23/04/2026 | <https://000004.awsstudygroup.com/> |
| 6 | - Tìm hiểu cơ chế hoạt động của Amazon RDS.<br>- Khởi tạo RDS DB instance, cấu hình subnet groups và security groups kết nối an toàn với máy chủ EC2.<br>- Triển khai ứng dụng thực tế với backend RDS và thực hiện các kịch bản sao lưu/khôi phục dữ liệu. | 24/04/2026 | 24/04/2026 | <https://000005.awsstudygroup.com/> |

### Kết quả đạt được tuần 1:

* **Quản trị tài khoản & Bảo mật (IAM)**: Thiết lập thành công MFA bảo mật tài khoản root, áp dụng nguyên tắc đặc quyền tối thiểu (Least Privilege) qua việc phân tách quyền quản trị bằng IAM Roles, Groups và thực hành Switch Role an toàn.
* **Hạ tầng mạng (VPC)**: Thiết lập phân vùng mạng Multi-AZ cô lập và an toàn, kiểm soát lưu lượng truy cập qua Security Groups (Stateful) và Network ACLs (Stateless), giám sát network traffic bằng VPC Flow Logs.
* **Máy chủ ảo (EC2)**: Triển khai thành công ứng dụng Node.js trên cả Linux và Windows Server, tối ưu hóa quản lý ứng dụng qua PM2 và Nginx Reverse Proxy.
* **Cơ sở dữ liệu (RDS)**: Kết nối thành công máy chủ ứng dụng EC2 đến RDS Database, hiểu rõ cơ chế cô lập dữ liệu trong mạng Private Subnet và quản lý chu kỳ sao lưu dữ liệu.
