---
title: "Nhật ký công việc Tuần 10"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

* Thiết lập API Gateway tập trung, cấu hình xác thực Cognito Authorizer và triển khai 8 API Endpoints nghiệp vụ.
* Khởi tạo mã nguồn ứng dụng Client Frontend (ReactJS & TypeScript) và tích hợp các thư viện xác thực Cognito SDK.
* Phát triển giao diện Dashboard cá nhân theo dõi tiến độ học tập, giao diện trắc nghiệm ôn tập kiến thức (Quiz) và tự luận (Essay).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Khởi tạo API RESTful trên API Gateway (`itcoach-api`).<br>- Thiết lập Cognito Authorizer (`itcoach-cognito-auth`) liên kết với Cognito User Pool đã tạo và cấu hình Token source bằng header `Authorization`. | 22/06/2026 | 22/06/2026 | Hướng dẫn ITCoach |
| 3 | - Tạo cấu trúc 8 endpoints trên API Gateway, cấu hình các method (GET/POST) tích hợp với Lambda tương ứng.<br>- Kích hoạt CORS (Enable CORS) cho tất cả các resources và deploy API lên stage `prod`. | 23/06/2026 | 23/06/2026 | Hướng dẫn ITCoach |
| 4 | - Khởi tạo dự án Frontend bằng ReactJS và TypeScript.<br>- Tích hợp thư viện AWS Cognito SDK cấu hình đăng nhập, đăng ký và lấy ID token gửi kèm trong các request API. | 24/06/2026 | 24/06/2026 | Hướng dẫn ITCoach |
| 5 | - Phát triển giao diện Dashboard cá nhân hiển thị tiến độ học tập, tỷ lệ hoàn thành chủ đề, streak học tập liên tiếp và bảng xếp hạng thành tích người dùng (Bảng điểm XP). | 25/06/2026 | 25/06/2026 | Hướng dẫn ITCoach |
| 6 | - Phát triển giao diện trắc nghiệm ôn tập (Quiz) hỗ trợ chọn một/nhiều đáp án đúng.<br>- Phát triển giao diện làm bài tự luận (Essay) gồm khung soạn thảo câu trả lời văn bản và nút ghi âm câu trả lời trực tiếp. | 26/06/2026 | 26/06/2026 | Hướng dẫn ITCoach |

### Kết quả đạt được tuần 10:

* **Tích hợp API Gateway**: Cấu hình hoàn chỉnh cổng kết nối API tập trung được bảo mật an toàn bằng Cognito Authorizer, đảm bảo chỉ người dùng đã xác thực mới có quyền truy cập dữ liệu.
* **Cơ sở hạ tầng Frontend**: Thiết lập xong mã nguồn ReactJS + TypeScript sạch, kết nối xác thực người dùng hoạt động trơn tru từ Client đến AWS Cognito.
* **Module ôn luyện kiến thức**: Phát triển thành công các chức năng học tập cơ bản: giao diện Dashboard trực quan, làm bài trắc nghiệm tính điểm XP, và khung luyện tập tự luận cơ bản.
