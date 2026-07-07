---
title: "Nhật ký công việc Tuần 8"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu tuần 8:

* Nghiên cứu quy trình xây dựng, huấn luyện và triển khai mô hình Trí tuệ nhân tạo/Học máy (AI/ML) sử dụng Amazon SageMaker.
* Tìm hiểu và tích hợp các dịch vụ AI ứng dụng có sẵn trên AWS như Amazon Polly (chuyển văn bản thành giọng nói), Amazon Rekognition (phân tích thị giác máy tính) và Amazon Lex (xây dựng giao diện trò chuyện hội thoại).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu các khái niệm cơ bản về AI/ML trên AWS và quy trình xây dựng mô hình<br>- Khởi tạo môi trường Amazon SageMaker Notebook Instance<br>- Làm quen với giao diện Jupyter Notebook, cấu hình môi trường IAM Role cần thiết | 08/06/2026 | 08/06/2026 | <https://000200.awsstudygroup.com/vi/> |
| 3 | - Chuẩn bị và tiền xử lý tập dữ liệu mẫu trong Jupyter Notebook<br>- Lựa chọn thuật toán tích hợp sẵn của SageMaker (như XGBoost hoặc Linear Learner)<br>- Thiết lập và chạy một SageMaker Training Job để huấn luyện mô hình | 09/06/2026 | 09/06/2026 | <https://000200.awsstudygroup.com/vi/> |
| 4 | - Triển khai mô hình đã huấn luyện thành một SageMaker Real-Time Endpoint<br>- Thực hiện kiểm thử dự đoán dữ liệu (Inference) gửi tới Endpoint từ Jupyter Notebook<br>- Viết hàm Lambda gọi SageMaker Endpoint để trả về kết quả dự đoán cho ứng dụng | 10/06/2026 | 10/06/2026 | <https://000200.awsstudygroup.com/vi/> |
| 5 | - Tìm hiểu Amazon Polly để chuyển đổi văn bản sang giọng nói nhân tạo tự nhiên<br>- Nghiên cứu Amazon Rekognition để phát hiện đối tượng, văn bản và phân tích khuôn mặt trong ảnh<br>- Viết code Python tích hợp Polly và Rekognition bằng thư viện Boto3 | 11/06/2026 | 11/06/2026 | <https://cloudjourney.awsstudygroup.com/vi/7-aimlservice/> |
| 6 | - Nghiên cứu Amazon Lex để xây dựng các Chatbot thông minh sử dụng công nghệ NLU (Natural Language Understanding)<br>- Thiết kế các Intents, Utterances và Slots cho một ứng dụng Chatbot đơn giản<br>- Thực hiện test và deploy chatbot trực tiếp trên AWS Console | 12/06/2026 | 12/06/2026 | <https://cloudjourney.awsstudygroup.com/vi/7-aimlservice/> |

### Kết quả đạt được tuần 8:

* **Làm chủ quy trình ML trên Amazon SageMaker:**
  * Hiểu rõ toàn bộ vòng đời xây dựng mô hình ML: Thu thập dữ liệu, Tiền xử lý, Huấn luyện, Đánh giá và Triển khai Endpoint.
  * Cấu hình và chạy thành công các SageMaker Training Jobs, biết cách kiểm tra log huấn luyện qua CloudWatch.
  * Thiết lập thành công Endpoint có khả năng co giãn tự động để phục vụ các yêu cầu dự đoán trực tiếp.

* **Ứng dụng các dịch vụ AI thông minh của AWS:**
  * Tích hợp thành công Amazon Polly để chuyển hóa văn bản thành file âm thanh chất lượng cao, phục vụ trực tiếp cho tính năng phát âm câu hỏi phỏng vấn giả lập.
  * Ứng dụng Rekognition để trích xuất thông tin chữ viết và cảm xúc khuôn mặt từ hình ảnh đầu vào.
  * Xây dựng thành công Chatbot tương tác tự động bằng Amazon Lex, hiểu cách xử lý hội thoại dựa trên ý định (Intents) của người dùng.
