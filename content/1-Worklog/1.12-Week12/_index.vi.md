---
title: "Nhật ký công việc Tuần 12"
date: 2026-07-06
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---
### Mục tiêu tuần 12:

* Tích hợp toàn trình (E2E), kiểm thử hệ thống và sửa các lỗi phát sinh.
* Nhập dữ liệu ngân hàng câu hỏi (Frontend, Backend, Cloud).
* Deploy ứng dụng lên môi trường Production trên AWS và thuyết trình Demo dự án.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tiến hành tích hợp toàn trình Frontend của tôi và Hạ tầng AWS (CloudFront, WAF, API Gateway, S3) do thành viên nhóm thiết lập | 06/07/2026 | 06/07/2026 | AWS Integration Guide |
| 3 | - Kiểm thử toàn trình (End-to-End Testing): Đăng ký -> Làm Quiz -> Làm Essay (ghi âm giọng nói) -> AI đánh giá (OpenAI) -> Đồng bộ điểm số lên Dashboard | 07/07/2026 | 07/07/2026 | Testing strategies & plans |
| 4 | - Nhập dữ liệu ngân hàng câu hỏi thực tế đa dạng (ưu tiên các chủ đề cốt lõi: Frontend, Backend, và kiến thức điện toán đám mây AWS) | 08/07/2026 | 08/07/2026 | Ngân hàng câu hỏi nội bộ |
| 5 | - Khắc phục các lỗi phát sinh (CORS, độ trễ Lambda, lỗi format audio trên các trình duyệt safari/chrome)<br>- Hỗ trợ nhóm hoàn thành deploy ứng dụng lên môi trường Production | 09/07/2026 | 09/07/2026 | Bug tracking & Deployment checklist |
| 6 | - Quay video demo vận hành thực tế hệ thống ITCoach<br>- Hoàn thiện báo cáo thực tập 12 tuần và thuyết trình tổng kết thực tập | 10/07/2026 | 10/07/2026 | Báo cáo & tài liệu tổng kết |

### Kết quả đạt được tuần 12:

* **Tích hợp toàn trình và Kiểm thử thành công:**
  * Toàn bộ hệ thống ITCoach được tích hợp đồng bộ: Client React kết nối an toàn tới AWS CloudFront đứng sau tường lửa AWS WAF, API Gateway tiếp nhận các yêu cầu và kích hoạt đúng các Lambda Functions.
  * Quy trình kiểm thử E2E hoạt động hoàn hảo: Đăng ký thành công -> Làm bài trắc nghiệm ghi nhận điểm -> Làm bài tự luận phỏng vấn bằng cách ghi âm giọng nói -> SQS nhận file ghi âm và đẩy qua AI Worker -> OpenAI chấm điểm thành công -> Điểm số hiển thị chính xác lên Dashboard.

* **Hoàn thiện ngân hàng câu hỏi chất lượng cao:**
  * Nhập thành công ngân hàng câu hỏi đa dạng bao gồm hơn 100 câu hỏi trắc nghiệm và tự luận phân loại theo trình duyệt/cấp độ (Frontend, Backend, DevOps, AWS Cloud).

* **Deploy thành công ứng dụng lên môi trường Production:**
  * Web app hoạt động chính thức trên domain tùy chỉnh với chứng chỉ SSL/HTTPS.
  * Tối ưu hóa hiệu năng Lambda: Bật cơ chế giữ ấm (Provisioned Concurrency) cho các Lambda API quan trọng để tránh hiện tượng Cold Start, giảm thời gian phản hồi từ 5s xuống dưới 1s.
  * Khắc phục triệt để lỗi ghi âm trên trình duyệt Safari bằng cách chuyển đổi định dạng audio sang WAV chuẩn.

* **Hoàn thành xuất sắc khóa thực tập:**
  * Quay video demo hoạt động của dự án ITCoach.
  * Hoàn thiện báo cáo thực tập tổng kết 12 tuần, thể hiện chi tiết giai đoạn học tập (Tuần 1-8) và giai đoạn làm đồ án (Tuần 9-12).
