---
title: "Nhật ký công việc Tuần 12"
date: 2024-01-01
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu tuần 12:

* Đóng gói mã nguồn và triển khai trang web tĩnh Frontend lên hạ tầng CDN đám mây (S3 & CloudFront).
* Thiết lập hệ thống định tuyến phân giải tên miền chuyên nghiệp với Amazon Route 53.
* Cấu hình giám sát cảnh báo vận hành hệ thống (CloudWatch & SNS) và nghiệm thu, đánh giá kết quả thực tập.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Đóng gói mã nguồn Client (ReactJS) bằng lệnh `npm run build` tạo thư mục `/dist`.<br>- Tải toàn bộ dữ liệu tĩnh lên S3 bucket `itcoach-static-assets` và cấu hình chỉ số phân phối trên S3. | 06/07/2026 | 06/07/2026 | Hướng dẫn ITCoach |
| 3 | - Tạo Amazon CloudFront Distribution (`itcoach-distribution`) liên kết với S3 static assets.<br>- Thiết lập Default Root Object là `index.html`, tạo các Error Pages Custom (403/404 thành 200 /index.html) để hỗ trợ điều hướng React Router và thực hiện invalidation. | 07/07/2026 | 07/07/2026 | Hướng dẫn ITCoach |
| 4 | - Cấu hình Amazon Route 53: mua tên miền tùy chỉnh hoặc cấu hình Hosted Zone.<br>- Tạo Alias Record trỏ tên miền chính đến phân phối CloudFront, và tạo Record trỏ tên miền phụ API đến AWS API Gateway. | 08/07/2026 | 08/07/2026 | Hướng dẫn ITCoach |
| 5 | - Thiết lập hệ thống giám sát và cảnh báo: tạo Amazon SNS Topic (`itcoach-alerts`) gửi email cảnh báo.<br>- Thiết lập 3 cảnh báo trên CloudWatch: Lỗi Lambda AI (`itcoach-ai-errors`), lỗi 5xx trên API Gateway, và thông báo quá tải hàng đợi SQS. | 09/07/2026 | 09/07/2026 | Hướng dẫn ITCoach |
| 6 | - Tiến hành kiểm thử hộp đen toàn bộ hệ thống ITCoach từ đầu đến cuối.<br>- Rà soát mã nguồn, dọn dẹp tài nguyên thừa, tối ưu chi phí Serverless, hoàn thiện tài liệu dự án và tổng kết kết quả thực tập tại FCAJ. | 10/07/2026 | 10/07/2026 | Tài liệu nội bộ |

### Kết quả đạt được tuần 12:

* **Triển khai Frontend đám mây (CDN)**: Đóng gói thành công ứng dụng ReactJS, chạy phân phối ổn định qua CloudFront CDN có tốc độ tải trang nhanh và hỗ trợ React Router mượt mà.
* **Cấu hình Tên miền (Route 53)**: Thiết lập thành công tên miền tùy chỉnh trỏ về ứng dụng khách và API Gateway thông qua giao thức HTTPS bảo mật an toàn.
* **Giám sát vận hành (CloudWatch/SNS)**: Kích hoạt thành công hệ thống cảnh báo qua email, tự động phát hiện các sự cố bất thường (lỗi 5xx hoặc quá tải hàng đợi SQS) giúp xử lý sự cố kịp thời.
* **Nghiệm thu toàn diện**: Dự án ITCoach hoạt động ổn định trên môi trường AWS Serverless thực tế, đạt điểm đánh giá cao từ mentor, hoàn tất chương trình thực tập xuất sắc.
