---
title: "Nhật ký công việc Tuần 8"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Khởi tạo dự án ITCoach: Phân tích thiết kế hệ thống, xác định luồng dữ liệu và thiết kế kiến trúc Serverless trên AWS.
* Thiết lập các dịch vụ lưu trữ (S3) và phân quyền bảo mật hạ tầng (IAM Role).
* Cấu hình dịch vụ xác thực tập trung Amazon Cognito và thiết lập hàng đợi tin nhắn Amazon SQS.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Nghiên cứu đề xuất dự án ITCoach: xác định đối tượng người dùng, tính năng ôn tập kiến thức, thi trắc nghiệm và phỏng vấn tự luận có sự hỗ trợ của AI.<br>- Phân tích thiết kế hệ thống, vẽ sơ đồ kiến trúc Serverless tích hợp Cognito, API Gateway, Lambda, SQS, DynamoDB, S3, Polly và OpenAI. | 08/06/2026 | 08/06/2026 | Tài liệu nội bộ |
| 3 | - Thiết lập IAM Role dùng chung cho các Lambda Functions (`itcoach-lambda-role`).<br>- Tick chọn và đính kèm 6 chính sách quyền hạn (Policies): `AWSLambdaBasicExecutionRole`, `AmazonDynamoDBFullAccess`, `AmazonS3FullAccess`, `AmazonSQSFullAccess`, `AmazonPollyFullAccess`, và `CloudWatchFullAccess`. | 09/06/2026 | 09/06/2026 | Tài liệu nội bộ |
| 4 | - Khởi tạo 2 S3 buckets phục vụ lưu trữ: bucket static assets `itcoach-static-assets` (bật Public website hosting) và bucket private `itcoach-audio-upload` lưu trữ các tệp ghi âm giọng nói.<br>- Cấu hình chính sách CORS trên bucket audio cho phép các method GET/PUT/POST/DELETE từ frontend. | 10/06/2026 | 10/06/2026 | Tài liệu nội bộ |
| 5 | - Khởi tạo dịch vụ quản lý định danh và xác thực người dùng tập trung Amazon Cognito User Pool.<br>- Đăng ký SPA App Client (`itcoach-web-client`) hỗ trợ phương thức đăng nhập bằng Email, bật thuộc tính bắt buộc `name` và lưu thông tin User Pool ID, Client ID. | 11/06/2026 | 11/06/2026 | Tài liệu nội bộ |
| 6 | - Thiết lập hệ thống hàng đợi tin nhắn Amazon SQS xử lý tác vụ bất đồng bộ phân tích âm thanh bằng AI.<br>- Tạo Dead Letter Queue (`itcoach-dlq`) và Queue chính (`itcoach-processing-queue`) cấu hình Visibility Timeout 300s, liên kết DLQ với số lần thử tối đa bằng 3. | 12/06/2026 | 12/06/2026 | Tài liệu nội bộ |

### Kết quả đạt được tuần 8:

* **Thiết kế hệ thống**: Hoàn thành tài liệu phân tích hệ thống ITCoach, thiết lập luồng dữ liệu phỏng vấn tự luận/giọng nói sử dụng mô hình Serverless tối ưu chi phí.
* **Bảo mật & Lưu trữ**: Cấu hình thành công phân quyền IAM Role hạn chế đặc quyền tối thiểu cho Lambda, triển khai 2 S3 Buckets phân tách tĩnh/động đáp ứng yêu cầu CORS của trình duyệt.
* **Xác thực người dùng (Cognito)**: Cấu hình xong Cognito User Pool sẵn sàng cung cấp cơ chế đăng nhập/đăng ký người dùng an toàn.
* **Hàng đợi tin nhắn (SQS)**: Xây dựng thành công kiến trúc xử lý tác vụ bất đồng bộ an toàn bằng cặp Queue SQS chính và DLQ dự phòng, sẵn sàng nhận trigger từ Lambda.
