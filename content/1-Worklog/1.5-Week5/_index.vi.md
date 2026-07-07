---
title: "Nhật ký công việc Tuần 5"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---
### Mục tiêu tuần 5:

* Triển khai hệ thống quản lý danh tính, đăng ký và xác thực người dùng sử dụng Amazon Cognito.
* Tích hợp cơ chế xác thực JWT Token để bảo vệ an toàn các cổng kết nối API Gateway.
* Xây dựng kiến trúc hướng sự kiện (Event-Driven Architecture) sử dụng Amazon SQS, Amazon SNS và Amazon EventBridge để tách rời (decouple) các thành phần hệ thống.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu Amazon Cognito và các thành phần User Pools vs Identity Pools<br>- Tạo và cấu hình Cognito User Pool, thiết lập chính sách mật khẩu và xác thực MFA<br>- Tùy chỉnh giao diện đăng nhập mặc định và email xác nhận người dùng | 18/05/2026 | 18/05/2026 | <https://000081.awsstudygroup.com/vi/> |
| 3 | - Tạo Cognito Identity Pool để cấp quyền truy cập tạm thời cho tài nguyên AWS (như S3, DynamoDB)<br>- Tích hợp SDK Cognito vào ứng dụng Frontend React để thực hiện đăng ký và đăng nhập<br>- Lấy và quản lý các JWT Tokens (ID Token, Access Token, Refresh Token) ở client | 19/05/2026 | 19/05/2026 | <https://000081.awsstudygroup.com/vi/> |
| 4 | - Tích hợp Cognito Authorizer vào API Gateway để bảo mật HTTP/REST API endpoints<br>- Cấu hình Lambda Function giải mã và kiểm tra thông tin JWT Token trong request header<br>- Kiểm tra phân quyền truy cập API bằng Postman với Authorization header | 20/05/2026 | 20/05/2026 | <https://000081.awsstudygroup.com/vi/> |
| 5 | - Tìm hiểu kiến trúc Event-Driven và hàng đợi tin nhắn Amazon SQS<br>- Khởi tạo Standard Queue và FIFO Queue (First-In-First-Out), hiểu về Visibility Timeout<br>- Viết ứng dụng Lambda gửi tin nhắn vào queue và cấu hình Lambda Trigger xử lý tin nhắn | 21/05/2026 | 21/05/2026 | <https://000077.awsstudygroup.com/vi/> |
| 6 | - Tìm hiểu Amazon SNS và mô hình gửi nhận tin nhắn dạng Publish/Subscribe (Pub/Sub)<br>- Tạo SNS Topic, cấu hình SQS và Email nhận thông báo từ Topic<br>- Nghiên cứu Amazon EventBridge, thiết lập Scheduled Rule để tự động kích hoạt Lambda | 22/05/2026 | 22/05/2026 | <https://000077.awsstudygroup.com/vi/> |

### Kết quả đạt được tuần 5:

* **Quản lý định danh người dùng an toàn với Amazon Cognito:**
  * Thiết lập thành công Cognito User Pool quản lý cơ sở dữ liệu người dùng tập trung, hỗ trợ đăng nhập qua MFA.
  * Tích hợp thành công luồng Authentication vào Frontend, quản lý lưu trữ JWT Token an toàn dưới LocalStorage/SessionStorage.
  * Bảo vệ tuyệt đối các endpoint API Gateway thông qua cơ chế Cognito Authorizer (chỉ có token hợp lệ mới được đi qua).

* **Xây dựng hệ thống tin nhắn và sự kiện bất đồng bộ:**
  * Làm chủ Amazon SQS để làm đệm trung gian cho các tác vụ xử lý mất nhiều thời gian, giúp tăng khả năng chịu tải của ứng dụng.
  * Phân biệt rõ Standard Queue (xử lý nhanh, không đảm bảo thứ tự) và FIFO Queue (đảm bảo thứ tự tuyệt đối và không trùng lặp tin nhắn).
  * Vận dụng SNS Pub/Sub để phát tán sự kiện từ một nguồn đến nhiều subscriber khác nhau (SQS, Lambda, Email) cùng một lúc.
  * Tạo các quy tắc EventBridge tự động chạy các tác vụ định kỳ (như dọn dẹp log, backup hàng đêm) theo định dạng cron-job.
