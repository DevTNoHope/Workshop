---
title: "Nhật ký công việc Tuần 4"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Triển khai các giải pháp kết nối mạng nâng cao (VPC Peering và AWS Transit Gateway).
* Tự động hóa tối ưu chi phí hạ tầng máy chủ ảo EC2 bằng AWS Lambda.
* Triển khai CI/CD pipeline sử dụng các dịch vụ Code-Suite nguyên bản của AWS và tích hợp giải pháp Hybrid Storage.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Nghiên cứu kiến trúc VPC Peering kết nối các mạng VPC khác nhau.<br>- Viết CloudFormation template triển khai hạ tầng mạng Multi-VPC tự động.<br>- Cấu hình định tuyến, cập nhật Security Groups và kiểm tra ping kết nối qua IP Private. | 11/05/2026 | 11/05/2026 | <https://000019.awsstudygroup.com/> |
| 3 | - Nghiên cứu AWS Transit Gateway thiết lập kết nối mạng hình sao (Hub-and-spoke).<br>- Tạo Transit Gateway, thiết lập attachments cho các VPC và định cấu hình route propagation tự động.<br>- Kiểm tra liên lạc xuyên suốt giữa các EC2 ở các VPC khác nhau. | 12/05/2026 | 12/05/2026 | <https://000020.awsstudygroup.com/> |
| 4 | - Nghiên cứu tối ưu chi phí EC2 bằng cách tự động tắt/bật instance ngoài giờ làm việc.<br>- Viết hàm AWS Lambda dừng/chạy instances dựa trên Resource Tags.<br>- Sử dụng Amazon EventBridge kích hoạt Lambda theo lịch biểu và SNS gửi thông báo kết quả. | 13/05/2026 | 13/05/2026 | <https://000022.awsstudygroup.com/> |
| 5 | - Triển khai quy trình CI/CD tự động bằng AWS CodeCommit, CodeBuild, CodeDeploy và CodePipeline.<br>- Cài đặt CodeDeploy Agent trên EC2, viết tệp cấu hình `buildspec.yml` và `appspec.yml`.<br>- Thiết lập pipeline 3 giai đoạn: Source -> Build -> Deploy tự động hóa cập nhật ứng dụng. | 14/05/2026 | 14/05/2026 | <https://000023.awsstudygroup.com/> |
| 6 | - Tìm hiểu AWS Storage Gateway kết nối lưu trữ on-premises với AWS Cloud.<br>- Triển khai File Gateway chạy trên EC2, cấu hình lưu trữ S3 backend.<br>- Ánh xạ (map) ổ đĩa mạng SMB/NFS trên máy trạm và kiểm tra đồng bộ hóa file tự động lên S3. | 15/05/2026 | 15/05/2026 | <https://000024.awsstudygroup.com/> |

### Kết quả đạt được tuần 4:

* **Kết nối đa VPC (Peering & Transit Gateway)**: Xây dựng thành công hạ tầng mạng doanh nghiệp phức tạp bằng CloudFormation. Kiểm soát định tuyến chéo thành công qua VPC Peering và Transit Gateway tập trung.
* **Tối ưu chi phí tự động**: Vận hành hệ thống dừng/bật máy chủ EC2 tự động trong giờ hành chính qua AWS Lambda và EventBridge Scheduler, giảm thiểu chi phí hao phí tài nguyên không cần thiết.
* **Pipeline AWS Code-Suite**: Làm chủ CI/CD nguyên bản của AWS, tự động kích hoạt tiến trình đóng gói và cập nhật phiên bản ứng dụng trên EC2 ngay khi có mã nguồn mới được push lên CodeCommit.
* **Lưu trữ đám mây lai (Storage Gateway)**: Triển khai ổ đĩa chia sẻ dùng chung an toàn kết hợp đồng bộ hóa dữ liệu trực tiếp lên Amazon S3, tối ưu hóa dung lượng lưu trữ cục bộ.
