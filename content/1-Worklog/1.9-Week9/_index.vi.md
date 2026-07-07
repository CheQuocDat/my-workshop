---
title: "Nhật ký công việc Tuần 9"
date: 2026-07-06
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---
### Mục tiêu tuần 9:

* Khởi động đồ án tốt nghiệp ITCoach (Hệ thống luyện phỏng vấn công nghệ với AI).
* Thiết kế kiến trúc Serverless trên AWS và phân công vai trò trong nhóm.
* Cấu hình cấu trúc thư mục codebase và bắt đầu thiết kế luồng xử lý ứng dụng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Họp nhóm thống nhất ý tưởng và phạm vi đồ án ITCoach<br>- Thiết kế cấu trúc cơ sở dữ liệu DynamoDB và các trường thông tin lưu trữ | 15/06/2026 | 15/06/2026 | Sách hướng dẫn & tài liệu AWS |
| 3 | - Vẽ sơ đồ kiến trúc hệ thống tổng thể (Web Serverless)<br>- Xác định các thành phần hạ tầng cần thiết trên AWS | 16/06/2026 | 16/06/2026 | AWS Architecture Center |
| 4 | - Phân công nhiệm vụ chi tiết: Bạn nhóm dựng hạ tầng (VPC, Cognito, S3, SQS, API Gateway, Route53, WAF), tôi thiết kế và phát triển Web App logic<br>- Xác định luồng API và cấu trúc dữ liệu gửi/nhận giữa Frontend và Backend | 17/06/2026 | 17/06/2026 | Sách hướng dẫn & tài liệu API |
| 5 | - Khởi tạo kho lưu trữ Git và phân chia các nhánh phát triển (Frontend, Backend, Infrastructure)<br>- Setup khung ứng dụng React/Vite ở local | 18/06/2026 | 18/06/2026 | Vite & React Guides |
| 6 | - Thiết kế cấu trúc chi tiết cho các Lambda Functions của Backend<br>- Viết tài liệu đặc tả kiến trúc phần mềm và luồng dữ liệu của đồ án | 19/06/2026 | 19/06/2026 | Dự án tài liệu nội bộ |

### Kết quả đạt được tuần 9:

* **Xác định mục tiêu đồ án tốt nghiệp:**
  * Thống nhất xây dựng ứng dụng ITCoach hỗ trợ người dùng ôn luyện kiến thức (Trắc nghiệm, Tự luận) và phỏng vấn giả lập (Mock Interview) với AI.
  * Thiết kế cấu trúc cơ sở dữ liệu trên Amazon DynamoDB bao gồm các bảng: `Users`, `Sessions`, `Questions`, `Answers`.

* **Hoàn thiện thiết kế kiến trúc hệ thống:**
  * Kiến trúc ứng dụng Web dạng Serverless hoàn chỉnh: Web client lưu trữ trên S3, phân phối qua CloudFront.
  * API giao tiếp qua Amazon API Gateway, xử lý logic bằng các AWS Lambda Functions.
  * Tích hợp AI (OpenAI API chấm điểm câu trả lời, Amazon Polly phát âm thanh câu hỏi).
  * Xử lý bất đồng bộ thông qua Amazon SQS hàng đợi.
  * Phân công vai trò rõ ràng: Thành viên cùng nhóm phụ trách dựng và cấu hình tài nguyên hạ tầng AWS (CloudFront, API Gateway, S3, Cognito, SQS, KMS, WAF). Bản thân tôi phụ trách phát triển ứng dụng Web (Frontend, Backend Lambda, AI Integration).

* **Thiết lập nền tảng codebase:**
  * Tạo repository Git chung, phân chia phân quyền và quy trình branch (main, develop, feature branches).
  * Khởi tạo thành công project Frontend với Vite + React + TypeScript và cấu trúc thư mục sạch.
  * Lập tài liệu mô tả 8 API tương ứng với 8 Lambda Functions sẽ viết ở Backend để thống nhất kết nối.
