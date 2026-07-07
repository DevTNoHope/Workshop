---
title: "Nhật ký công việc Tuần 3"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

* Nghiên cứu công nghệ ảo hóa và thực hành di chuyển máy ảo (VM Import/Export).
* Tìm hiểu công nghệ Container (Docker/Docker Compose) và quản lý container trên Amazon ECS.
* Thiết lập hệ thống tự động hóa CI/CD cho container và quản lý tuân thủ bảo mật với AWS Security Hub.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu VM Import/Export: Export máy ảo từ VMware Workstation (OVA/VMDK).<br>- Tải máy ảo lên Amazon S3, thiết lập IAM Role và thực hiện import thành AMI trên EC2.<br>- Khởi chạy instance từ Custom AMI và xác minh ứng dụng hoạt động chính xác. | 04/05/2026 | 04/05/2026 | <https://000014.awsstudygroup.com/> |
| 3 | - Tìm hiểu Docker cơ bản: Dockerfile, Images, Containers và các lệnh cơ bản.<br>- Khởi động EC2 cài đặt Docker, xây dựng ứng dụng multi-container bằng Docker Compose.<br>- Tạo kho lưu trữ Amazon ECR, cấu hình IAM truy cập và đẩy ảnh (Docker Image) lên ECR. | 05/05/2026 | 05/05/2026 | <https://000015.awsstudygroup.com/> |
| 4 | - Nghiên cứu dịch vụ quản lý container Amazon ECS: Clusters, Task Definitions và Services.<br>- Tạo ECS Cluster (EC2 launch type), thiết lập Application Load Balancer và đăng ký dịch vụ với AWS Cloud Map.<br>- Thực hành cập nhật Rolling Update và Blue/Green Deployment. | 06/05/2026 | 06/05/2026 | <https://000016.awsstudygroup.com/> |
| 5 | - Thiết kế CI/CD pipeline tự động hóa quy trình deploy container lên Amazon ECS.<br>- Cấu hình mã nguồn trên GitLab, viết tệp cấu hình `.gitlab-ci.yml` và tích hợp AWS CodeBuild.<br>- Tự động hóa build, push Docker image lên ECR và deploy ứng dụng lên ECS. | 07/05/2026 | 07/05/2026 | <https://000017.awsstudygroup.com/> |
| 6 | - Tìm hiểu AWS Security Hub và các tiêu chuẩn bảo mật đám mây (CIS AWS Foundations, PCI DSS).<br>- Kích hoạt Security Hub, phân tích các lỗ hổng (security findings), tạo custom insights và thiết lập cơ chế tự khắc phục lỗi bằng AWS Config. | 08/05/2026 | 08/05/2026 | <https://000018.awsstudygroup.com/> |

### Kết quả đạt được tuần 3:

* **Di chuyển máy ảo (VM Import/Export)**: Thực hiện thành công quy trình di chuyển máy ảo chạy hệ điều hành Ubuntu từ on-premises sang đám mây dưới dạng Custom AMI trên EC2, và ngược lại.
* **Đóng gói ứng dụng (Docker/ECR)**: Thành thạo các bước viết Dockerfile tối ưu, quản lý ứng dụng đa container bằng Docker Compose và đẩy ảnh lên Amazon Elastic Container Registry an toàn.
* **Quản lý Container (Amazon ECS)**: Triển khai thành công ứng dụng trên ECS Cluster, cấu hình mạng (awsvpc), tích hợp ALB định tuyến lưu lượng và thực hiện Blue/Green deployments thông qua CodeDeploy.
* **Tự động hóa CI/CD**: Xây dựng thành công pipeline CI/CD từ GitLab CI kết nối trực tiếp đến AWS ECR và ECS, giúp tự động hóa quy trình build và cập nhật ứng dụng ngay khi thay đổi code.
* **Kiểm toán bảo mật (Security Hub)**: Kích hoạt giám sát bảo mật tập trung cho toàn bộ tài khoản AWS, phát hiện sớm các lỗ hổng bảo mật cấu hình sai và nắm rõ cách cải thiện điểm số tuân thủ bảo mật hệ thống.
