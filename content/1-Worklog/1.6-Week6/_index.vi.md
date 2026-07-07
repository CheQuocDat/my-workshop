---
title: "Nhật ký công việc Tuần 6"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu tuần 6:

* Triển khai các giải pháp bảo mật nâng cao trên AWS nhằm bảo vệ ứng dụng Web khỏi các mối đe dọa trực tuyến sử dụng AWS WAF.
* Quản lý mã hóa dữ liệu tập trung với AWS KMS và bảo mật thông tin nhạy cảm sử dụng AWS Secrets Manager.
* Tích hợp hệ thống phát hiện xâm nhập thông minh AWS GuardDuty và quản lý máy chủ an toàn không cần SSH thông qua Systems Manager Session Manager.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu AWS WAF (Web Application Firewall) và các khái niệm Web ACL, Rules, Rule Groups<br>- Khởi tạo Web ACL, liên kết với CloudFront Distribution hoặc Application Load Balancer<br>- Cấu hình các rules cơ bản ngăn chặn SQL Injection, Cross-Site Scripting (XSS) và chặn IP xấu | 25/05/2026 | 25/05/2026 | <https://000026.awsstudygroup.com/vi/> |
| 3 | - Tìm hiểu cơ chế mã hóa của AWS KMS (Key Management Service) và phân biệt AWS Managed Keys vs Customer Managed Keys (CMK)<br>- Tạo CMK, cấu hình Key Policy để phân quyền quản trị và sử dụng khóa<br>- Thực hành mã hóa và giải mã dữ liệu của S3 Bucket và EBS Volume bằng KMS | 26/05/2026 | 26/05/2026 | <https://000033.awsstudygroup.com/vi/> |
| 4 | - Nghiên cứu dịch vụ quản lý thông tin mật AWS Secrets Manager<br>- Khởi tạo và lưu trữ các thông tin kết nối Database nhạy cảm (Username, Password, Endpoint)<br>- Viết mã nguồn Lambda gọi Secrets Manager API để lấy thông tin kết nối lúc runtime<br>- Cấu hình tính năng tự động xoay vòng mật khẩu (Automatic Secret Rotation) | 27/05/2026 | 27/05/2026 | <https://000096.awsstudygroup.com/vi/> |
| 5 | - Kích hoạt AWS GuardDuty để giám sát bảo mật tài khoản AWS liên tục<br>- Tìm hiểu cách GuardDuty phân tích VPC Flow Logs, DNS Logs và CloudTrail Events<br>- Tạo giả lập các cuộc tấn công thử nghiệm để phân tích các cảnh báo (Findings) của GuardDuty | 28/05/2026 | 28/05/2026 | <https://000098.awsstudygroup.com/vi/> |
| 6 | - Tìm hiểu AWS Systems Manager (SSM) và tính năng Session Manager<br>- Cấu hình IAM Role cho EC2 instance có đính kèm AWS Systems Manager Agent (SSM Agent)<br>- Thực hiện kết nối Terminal vào EC2 qua AWS Console mà không cần mở port SSH 22 và không cần SSH Key | 29/05/2026 | 29/05/2026 | <https://000058.awsstudygroup.com/vi/> |

### Kết quả đạt được tuần 6:

* **Tăng cường bảo mật ứng dụng với AWS WAF:**
  * Ngăn chặn thành công các truy cập trái phép và các loại tấn công phổ biến (OWASP Top 10) vào hệ thống ứng dụng.
  * Hiểu cách thiết lập các rate-based rules để chống lại các cuộc tấn công từ chối dịch vụ (DDoS) cơ bản.

* **Làm chủ mã hóa và quản lý khóa với KMS:**
  * Triển khai thành công mã hóa dữ liệu ở trạng thái tĩnh (encryption at rest) cho toàn bộ tài nguyên lưu trữ quan trọng.
  * Hiểu rõ cách phân quyền sử dụng khóa thông qua Key Policies và IAM Policies.

* **Bảo vệ thông tin mật với Secrets Manager:**
  * Loại bỏ hoàn toàn việc lưu trữ thông tin nhạy cảm dưới dạng hardcode trong file config hay mã nguồn.
  * Triển khai thành công tính năng xoay vòng mật khẩu định kỳ tự động giúp tăng cường mức độ an toàn cho Database.

* **Giám sát bảo mật chủ động và Quản trị máy chủ:**
  * Sử dụng GuardDuty phát hiện sớm các nguy cơ bảo mật như rò rỉ key, truy cập bất thường từ IP lạ.
  * Áp dụng thành công Session Manager để quản lý máy chủ an toàn, loại bỏ hoàn toàn rủi ro bị brute force cổng SSH (22) và quản lý file key (.pem) phức tạp.
