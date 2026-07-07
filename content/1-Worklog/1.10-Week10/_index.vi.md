---
title: "Nhật ký công việc Tuần 10"
date: 2026-07-06
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---
### Mục tiêu tuần 10:

* Phát triển mã nguồn Backend (8 AWS Lambda Functions) xử lý logic và tích hợp các dịch vụ AI (OpenAI API, Amazon Polly).
* Xây dựng giao diện Frontend cơ bản (Trang Authentication, làm trắc nghiệm, viết tự luận và ghi âm).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Viết mã nguồn Lambda Functions cho hệ thống Trắc nghiệm (Quiz API: lấy câu hỏi, gửi kết quả)<br>- Lập trình Lambda Functions xử lý Authentication qua Amazon Cognito | 22/06/2026 | 22/06/2026 | Node.js & AWS SDK documentation |
| 3 | - Xây dựng 2 Lambda Functions cốt lõi xử lý Tự luận (Essay API) và tạo phiên phỏng vấn mới (Mock Interview Session API)<br>- Thiết lập cấu hình kết nối database DynamoDB từ các Lambda | 23/06/2026 | 23/06/2026 | DynamoDB DocumentClient Guide |
| 4 | - Tích hợp OpenAI API vào Lambda Worker để tự động chấm điểm và đánh giá chi tiết bài làm tự luận của sinh viên<br>- Tích hợp Amazon Polly (Text-to-Speech) để chuyển đổi câu hỏi phỏng vấn thành audio, lưu trữ vào S3 và sinh Presigned URL | 24/06/2026 | 24/06/2026 | OpenAI API Docs & Amazon Polly Guide |
| 5 | - Phát triển giao diện Frontend cơ bản: Trang Đăng nhập/Đăng ký (tích hợp Cognito SDK) và trang làm bài trắc nghiệm (Quiz UI)<br>- Thiết kế cấu trúc các component giao diện React | 25/06/2026 | 25/06/2026 | React UI & Cognito Auth Integration |
| 6 | - Phát triển giao diện viết bài tự luận (Essay UI) tích hợp trình ghi âm câu trả lời trực tiếp trên trình duyệt<br>- Kiểm thử cục bộ (local testing) các API Lambda bằng AWS SAM / LocalStack | 26/06/2026 | 27/06/2026 | Web Audio API Docs |

### Kết quả đạt được tuần 10:

* **Hoàn thành phát triển logic Backend với 8 Lambda Functions:**
  * `auth-handler`: Quản lý đăng ký, đăng nhập và phân quyền bằng JWT Token.
  * `quiz-get-questions`: Lấy danh sách câu hỏi trắc nghiệm theo chủ đề.
  * `quiz-submit-answers`: Lưu trữ và tính điểm bài trắc nghiệm của người dùng.
  * `essay-get-questions`: Lấy ngân hàng câu hỏi tự luận.
  * `essay-submit-answers`: Tiếp nhận bài làm tự luận và kích hoạt tiến trình chấm điểm.
  * `interview-session-start`: Khởi tạo phiên phỏng vấn và gọi Amazon Polly để sinh giọng nói câu hỏi.
  * `interview-audio-handler`: Xử lý lưu trữ file ghi âm câu trả lời lên Amazon S3 qua Presigned URL.
  * `ai-evaluation-worker`: Lambda chạy ngầm lắng nghe SQS để gửi nội dung bài làm tự luận/âm thanh qua OpenAI API phân tích và cập nhật điểm số vào DynamoDB.

* **Tích hợp thành công AI & Dịch vụ Giọng nói:**
  * **Amazon Polly:** Tự động sinh ra file âm thanh `.mp3` chất lượng cao mô phỏng người phỏng vấn thật.
  * **OpenAI (GPT-4o):** Đóng vai trò là một IT Coach ảo, phân tích ngữ pháp, từ vựng kỹ thuật và độ chính xác của câu trả lời, đưa ra phản hồi bằng cả tiếng Anh và tiếng Việt.

* **Xây dựng khung giao diện Frontend cơ bản:**
  * Hoàn thiện luồng đăng nhập, đăng ký và lấy token xác thực (Cognito JWT).
  * Xây dựng giao diện trắc nghiệm thân thiện với đồng hồ đếm ngược và chọn câu trả lời trực quan.
  * Tích hợp thành công Web Audio API trên trình duyệt để ghi âm trực tiếp giọng nói của người dùng và sẵn sàng gửi lên S3.
