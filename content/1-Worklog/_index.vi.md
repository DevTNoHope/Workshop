---
title: "Nhật ký công việc"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

### 🚀 Tổng quan về Hành trình Thực tập & Học tập (Worklog)

Chào mừng bạn đến với trang nhật ký công việc của tôi trong suốt chương trình **First Cloud AI Journey (FCAJ)**. Đây là một tài liệu chi tiết, ghi nhận toàn bộ quá trình học tập, nghiên cứu và triển khai thực tế các công nghệ điện toán đám mây Amazon Web Services (AWS) kéo dài trong **12 tuần**.

Chương trình được thiết kế theo mô hình **hybrid** (kết hợp tự nghiên cứu từ xa và làm việc trực tiếp tại văn phòng trong các buổi thảo luận, cùng với việc tham gia các sự kiện công nghệ cộng đồng lớn như AWS Community Days). Toàn bộ lộ trình 12 tuần được chia làm 2 giai đoạn cốt lõi:

1. **Giai đoạn 1: Làm chủ hạ tầng AWS qua Chuỗi bài thực hành (Tuần 1 - Tuần 7)**
   * Hoàn thành 39 bài lab AWS thực tế (từ Lab 001 đến Lab 040, loại bỏ Lab 12 để tối ưu tài nguyên).
   * Nghiên cứu sâu từ hạ tầng cơ bản (VPC, EC2, RDS, IAM, S3) đến các dịch vụ nâng cao (CI/CD, Monitoring, Security, Cost Optimization, Container/ECS/EKS).
2. **Giai đoạn 2: Phát triển Dự án Luyện phỏng vấn ITCoach Serverless (Tuần 8 - Tuần 12)**
   * Lập kế hoạch, thiết kế kiến trúc hệ thống 3-tier Serverless.
   * Xây dựng và triển khai toàn bộ các dịch vụ đám mây AWS tích hợp AI (OpenAI API cho Whisper/GPT, Amazon Polly cho Text-to-Speech) để xây dựng ứng dụng mô phỏng phỏng vấn thực tế dành cho sinh viên IT.

---

### 📅 Lộ trình Chi tiết qua các Tuần

Dưới đây là liên kết dẫn tới nhật ký công việc chi tiết của từng tuần:

| Tuần | Chủ đề chính | Các nội dung triển khai chính | Chi tiết |
| :---: | :--- | :--- | :---: |
| **Tuần 1** | AWS Basics & Core Infrastructure | Thiết lập tài khoản AWS, quản lý quyền hạn IAM, cấu hình VPC mạng cơ bản, khởi chạy EC2 và RDS. | [Xem chi tiết](1.1-week1/) |
| **Tuần 2** | Scaling, DNS & Basic Automation | Triển khai Auto Scaling Group, Application Load Balancer, Route 53 và tự động hóa sao lưu với AWS Backup. | [Xem chi tiết](1.2-week2/) |
| **Tuần 3** | Virtualization & Container | Nghiên cứu Containerization, quản lý ứng dụng trên Docker, AWS ECS (Fargate) và thiết lập AWS EKS. | [Xem chi tiết](1.3-week3/) |
| **Tuần 4** | Advanced Networking & CI/CD | Cấu hình Transit Gateway, VPC Peering và thiết lập luồng tự động hóa CI/CD bằng AWS CodePipeline. | [Xem chi tiết](1.4-week4/) |
| **Tuần 5** | Security, Tagging & Permission | Triển khai bảo mật AWS KMS, AWS WAF, IAM Policy nâng cao và chiến lược gắn thẻ tài nguyên (Tagging). | [Xem chi tiết](1.5-week5/) |
| **Tuần 6** | Operations, Audit & Data Lake | Thiết lập hệ thống kiểm toán CloudTrail, giám sát EventBridge và xây dựng hệ thống lưu trữ Data Lake. | [Xem chi tiết](1.6-week6/) |
| **Tuần 7** | IaC, NoSQL & Cost Analysis | Viết mã nguồn hạ tầng CloudFormation, thiết lập DynamoDB và phân tích chi phí bằng Cost Explorer. | [Xem chi tiết](1.7-week7/) |
| **Tuần 8** | ITCoach: Architecture & Cloud Services | Phân tích yêu cầu hệ thống ITCoach, thiết lập các IAM Role bảo mật, cấu hình S3 Buckets, Cognito và SQS. | [Xem chi tiết](1.8-week8/) |
| **Tuần 9** | ITCoach: DynamoDB & Lambda Functions | Thiết kế lược đồ và chỉ mục (GSI/LSI) cho 8 bảng DynamoDB. Viết và tích hợp 8 hàm AWS Lambda. | [Xem chi tiết](1.9-week9/) |
| **Tuần 10** | ITCoach: API Gateway & Dashboard | Cấu hình REST API trên API Gateway tích hợp Cognito Authorizer. Xây dựng giao diện ReactJS Dashboard. | [Xem chi tiết](1.10-week10/) |
| **Tuần 11** | ITCoach: Audio, OpenAI & Polly | Lập trình ghi âm giọng nói, tải dữ liệu lên S3 qua Presigned URL, tích hợp OpenAI GPT/Whisper & Polly. | [Xem chi tiết](1.11-week11/) |
| **Tuần 12** | ITCoach: CloudFront, Route 53 & Test | Cấu hình CDN CloudFront cho frontend, ánh xạ tên miền Route 53, thiết lập CloudWatch Alarm và kiểm thử hệ thống. | [Xem chi tiết](1.12-week12/) |

---

> [!NOTE]
> Mọi báo cáo tuần đều được ghi nhận trực quan bao gồm các mục tiêu đề ra, các tác vụ cụ thể kèm ngày thực hiện thực tế, tài liệu tham khảo và các thành tựu thu hoạch được.
