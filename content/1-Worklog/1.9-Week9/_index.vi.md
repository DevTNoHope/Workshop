---
title: "Nhật ký công việc Tuần 9"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

* Triển khai hệ thống cơ sở dữ liệu DynamoDB gồm 8 bảng, cấu hình hiệu suất On-demand và thiết lập Global Secondary Indexes (GSI).
* Phát triển và triển khai nhóm Lambda Functions xử lý các API nghiệp vụ đăng nhập, quản lý câu hỏi, quản trị phiên phỏng vấn và nộp bài.
* Phát triển Lambda xử lý tác vụ thông minh (AI processing), cấu hình biến môi trường hệ thống và thiết lập SQS trigger.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Triển khai 8 bảng DynamoDB: `users`, `questions`, `sessions`, `answers`, `history`, `topics`, `quiz-attempts`, `gamification` ở chế độ On-demand.<br>- Cấu hình các chỉ mục phụ toàn cục (GSI): `category-index`, `userId-index`, `sessionId-index`, `xp-index` để tối ưu hóa hiệu suất truy vấn. | 15/06/2026 | 15/06/2026 | Hướng dẫn ITCoach |
| 3 | - Phát triển Lambda `itcoach-auth-handler` quản lý thông tin profile người dùng.<br>- Phát triển Lambda `itcoach-question-handler` truy xuất danh sách câu hỏi tự luận theo chuyên ngành (Frontend, Backend, DevOps...) và danh sách topics. | 16/06/2026 | 16/06/2026 | Hướng dẫn ITCoach |
| 4 | - Phát triển Lambda `itcoach-session-handler` khởi tạo phiên Mock Interview, tự động chọn câu hỏi từ ngân hàng dựa trên level/duration.<br>- Phát triển Lambda `itcoach-answer-handler` lưu thông tin câu trả lời và tạo Presigned URL upload file âm thanh lên S3. | 17/06/2026 | 17/06/2026 | Hướng dẫn ITCoach |
| 5 | - Phát triển Lambda xử lý tác vụ nặng `itcoach-ai-processor` tích hợp OpenAI STT dịch âm thanh, OpenAI GPT chấm điểm/nhận xét câu trả lời, và Polly TTS chuyển văn bản phản hồi thành giọng nói.<br>- Cấu hình biến môi trường: bucket S3, tên bảng DB, endpoint URL và API key. | 18/06/2026 | 18/06/2026 | Hướng dẫn ITCoach |
| 6 | - Phát triển các Lambda Functions phụ trợ còn lại: `itcoach-result-handler` (lịch sử, thống kê), `itcoach-quiz-handler` (làm quiz, thuật toán Spaced Repetition SM-2), và `itcoach-gamification-handler` (XP, streaks, leaderboard).<br>- Thiết lập SQS trigger liên kết SQS Queue với Lambda `itcoach-ai-processor`. | 19/06/2026 | 19/06/2026 | Hướng dẫn ITCoach |

### Kết quả đạt được tuần 9:

* **Hạ tầng Cơ sở dữ liệu (DynamoDB)**: Khởi tạo thành công 8 bảng DynamoDB hoạt động ổn định ở chế độ On-demand, cấu hình các chỉ mục GSI cho phép truy vấn nhanh dữ liệu phiên và bảng xếp hạng XP.
* **Logic Nghiệp vụ (Lambda)**: Triển khai thành công 8 Lambda functions bằng Python 3.12, gán đúng Custom Role và tối ưu hóa thời gian timeout, dung lượng RAM cho từng dịch vụ.
* **Tích hợp Tự động hóa**: Cấu hình thành công biến môi trường bảo mật độc lập, thiết lập trigger SQS kích hoạt Lambda AI xử lý bất đồng bộ các tệp tin âm thanh ghi âm hiệu quả.
