---
title: "Nhật ký công việc Tuần 11"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Phát triển phòng phỏng vấn mô phỏng (Mock Interview Room) tương tác giọng nói thời gian thực.
* Xây dựng luồng tải tệp tin âm thanh lên S3 qua Presigned URL và gửi thông điệp xử lý đến SQS.
* Tích hợp AI thông minh: dịch giọng nói (OpenAI STT), đánh giá câu hỏi (OpenAI GPT) và sinh giọng nói nhân tạo (Amazon Polly).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Thiết kế giao diện Mock Interview Room: cho phép người dùng cấu hình buổi phỏng vấn (Chuyên ngành, Cấp độ, Thời lượng).<br>- Tích hợp MediaRecorder API trên trình duyệt để ghi âm giọng nói của người dùng trực tiếp qua microphone. | 29/06/2026 | 29/06/2026 | Hướng dẫn ITCoach |
| 3 | - Gọi API nộp bài để lấy Presigned URL từ Lambda `itcoach-answer-handler`.<br>- Triển khai hàm upload tệp ghi âm `.webm`/`.mp3` trực tiếp từ client lên S3 bucket `itcoach-audio-upload` và tự động gửi message kích hoạt vào SQS. | 30/06/2026 | 30/06/2026 | Hướng dẫn ITCoach |
| 4 | - Tích hợp API OpenAI Whisper trong Lambda `itcoach-ai-processor` để dịch file âm thanh từ S3 thành văn bản (Speech-to-Text).<br>- Sử dụng OpenAI GPT-4o đánh giá câu trả lời tự luận dựa trên tiêu chí đáp án chuẩn, tính toán điểm số và chỉ ra các ý còn thiếu. | 01/07/2026 | 01/07/2026 | Hướng dẫn ITCoach |
| 5 | - Tích hợp dịch vụ Amazon Polly trong Lambda để chuyển văn bản nhận xét/câu hỏi tiếp theo của AI thành giọng nói (Text-to-Speech).<br>- Lưu trữ file âm thanh của Polly tạo ra lên S3, trả về URL cho Client và phát phát giọng nói của AI trên giao diện phỏng vấn. | 02/07/2026 | 02/07/2026 | Hướng dẫn ITCoach |
| 6 | - Phát triển màn hình kết quả sau buổi phỏng vấn (Feedback Dashboard): hiển thị điểm tổng, điểm kỹ năng, các câu trả lời mẫu tham khảo và đề xuất các chủ đề kiến thức cần ôn tập tiếp theo. | 03/07/2026 | 03/07/2026 | Hướng dẫn ITCoach |

### Kết quả đạt được tuần 11:

* **Tương tác Giọng nói (Media & S3)**: Phát triển thành công module ghi âm trình duyệt, tải tệp tin âm thanh an toàn lên S3 thông qua Presigned URL mà không làm lộ credentials.
* **Xử lý Ngôn ngữ Tự nhiên (STT & GPT)**: Tích hợp thành công bộ vi xử lý AI dịch chuyển giọng nói chuẩn xác sang văn bản, chấm điểm và đánh giá chính xác các ý chuyên môn bắt buộc của câu hỏi tự luận.
* **Phản hồi bằng Giọng nói (Polly TTS)**: Triển khai thành công giọng nói nhân tạo của AI sinh động, phát lại trên client tạo cảm giác phỏng vấn thực tế với người hỏi bản ngữ.
* **Báo cáo Kết quả phỏng vấn**: Hoàn thiện trang thống kê kết quả chi tiết, giúp người học dễ dàng nhận ra điểm yếu kiến thức và cách cải thiện câu trả lời.
