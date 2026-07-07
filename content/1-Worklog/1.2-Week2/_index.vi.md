---
title: "Nhật ký công việc Tuần 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---
### Mục tiêu tuần 2:

* Tìm hiểu các dịch vụ Hosting & Storage trên AWS bao gồm Amazon S3, Amazon CloudFront và Amazon Route 53.
* Triển khai và lưu trữ website tĩnh (Static Website Hosting) trên Amazon S3 với độ bảo mật cao.
* Cấu hình dịch vụ phân phối nội dung (CDN) Amazon CloudFront giúp tối ưu hóa hiệu năng, giảm độ trễ truy cập toàn cầu.
* Quản lý DNS và cấu hình tên miền tùy chỉnh sử dụng Amazon Route 53 kết hợp với chứng chỉ SSL/TLS từ ACM.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu Amazon S3 (Simple Storage Service) cơ bản<br>- Phân biệt các loại Storage Classes (Standard, IA, Glacier)<br>- Nghiên cứu cơ chế phân quyền: IAM Policies, Bucket Policies và ACLs<br>- Thiết lập cấu hình mã hóa mặc định (SSE-S3, SSE-KMS) | 27/04/2026 | 27/04/2026 | <https://000057.awsstudygroup.com/vi/> |
| 3 | - Kích hoạt tính năng Static Website Hosting trên S3<br>- Upload source code website tĩnh và cấu hình tài liệu chỉ mục (index.html, error.html)<br>- Thiết lập Bucket Policy cho phép truy cập công khai an toàn<br>- Tìm hiểu và cấu hình CORS (Cross-Origin Resource Sharing) | 28/04/2026 | 28/04/2026 | <https://000057.awsstudygroup.com/vi/> |
| 4 | - Tìm hiểu Amazon CloudFront và các khái niệm Edge Locations, Regional Edge Caches<br>- Khởi tạo CloudFront Distribution với nguồn gốc (Origin) là S3 Bucket<br>- Cấu hình Origin Access Control (OAC) để chặn truy cập trực tiếp vào S3<br>- Thiết lập Cache Behaviors, TTL và nén nội dung tự động | 29/04/2026 | 29/04/2026 | <https://000094.awsstudygroup.com/vi/> |
| 5 | - Tìm hiểu Amazon Route 53 và các phương thức định tuyến DNS<br>- Tạo Hosted Zone cho tên miền tùy chỉnh<br>- Cấu hình các bản ghi DNS cơ bản (A, AAAA, CNAME, MX, TXT)<br>- Thiết lập bản ghi Routing Alias trỏ về CloudFront Distribution | 30/04/2026 | 30/04/2026 | <https://000010.awsstudygroup.com/vi/> |
| 6 | - Yêu cầu chứng chỉ SSL/TLS miễn phí qua AWS Certificate Manager (ACM)<br>- Thực hiện xác thực tên miền bằng phương pháp DNS Validation<br>- Liên kết ACM Certificate vào CloudFront Distribution<br>- Cấu hình quy tắc bảo mật HTTPS và chuyển hướng tự động HTTP sang HTTPS | 01/05/2026 | 01/05/2026 | <https://000094.awsstudygroup.com/vi/> |

### Kết quả đạt được tuần 2:

* **Nắm vững kiến thức lưu trữ Amazon S3:**
  * Hiểu rõ cấu trúc lưu trữ dạng Object, phân biệt các Storage Classes để tối ưu hóa chi phí.
  * Biết cách cấu hình Lifecycle Policies tự động chuyển đổi lớp lưu trữ hoặc xóa dữ liệu cũ.
  * Làm chủ Bucket Policies và OAC để bảo vệ dữ liệu một cách an toàn, chỉ cho phép truy cập qua CloudFront.

* **Triển khai thành công Website tĩnh:**
  * Cấu hình và deploy website tĩnh lên S3 chạy ổn định, nhanh chóng.
  * Cấu hình CORS thành công cho phép website tương tác an toàn với các API ngoài.

* **Tối ưu hóa hiệu năng với Amazon CloudFront:**
  * Thiết lập mạng lưới CDN phân phối nội dung tĩnh toàn cầu với độ trễ thấp nhất.
  * Hiểu cách cấu hình Cache Key, TTL và cơ chế Invalidate Cache để cập nhật nội dung tức thời khi có thay đổi source code.

* **Quản trị DNS và bảo mật tên miền:**
  * Làm chủ hệ thống DNS Route 53, thiết lập các bản ghi định tuyến chính xác.
  * Tích hợp thành công HTTPS bằng chứng chỉ SSL/TLS từ ACM, bảo mật đường truyền người dùng cuối và đạt điểm tối ưu SEO.
