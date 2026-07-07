---
title: "Nhật ký công việc Tuần 4"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---
### Mục tiêu tuần 4:

* Tìm hiểu điện toán máy chủ serverless trên AWS thông qua dịch vụ cốt lõi AWS Lambda.
* Thiết lập và quản lý các cổng kết nối API an toàn sử dụng Amazon API Gateway.
* Xây dựng và triển khai các ứng dụng serverless một cách tự động sử dụng công cụ AWS SAM (Serverless Application Model).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu kiến trúc Serverless và cơ chế Event-Driven<br>- Giới thiệu dịch vụ AWS Lambda, cấu hình Memory, Timeout và IAM Execution Role<br>- Viết hàm Lambda cơ bản để xử lý chuỗi và JSON đầu vào | 11/05/2026 | 11/05/2026 | <https://000022.awsstudygroup.com/vi/> |
| 3 | - Phát triển các hàm Lambda nâng cao kết nối với S3 và DynamoDB bằng AWS SDK<br>- Cấu hình Environment Variables (Biến môi trường) để quản lý cấu hình động<br>- Kiểm tra và debug Lambda function sử dụng CloudWatch Logs | 12/05/2026 | 12/05/2026 | <https://000022.awsstudygroup.com/vi/> |
| 4 | - Tìm hiểu dịch vụ Amazon API Gateway<br>- Phân biệt REST APIs vs HTTP APIs (hiệu năng cao, chi phí thấp)<br>- Tạo API và cấu hình các Resources, Methods (GET, POST, PUT, DELETE)<br>- Cấu hình CORS (Cross-Origin Resource Sharing) để cho phép client gọi API | 13/05/2026 | 13/05/2026 | <https://000066.awsstudygroup.com/vi/> |
| 5 | - Tích hợp API Gateway với Lambda sử dụng Lambda Proxy Integration<br>- Xử lý tham số truyền vào: Query String Parameters, Path Parameters và Request Body<br>- Cấu hình API Gateway Stages và triển khai API lên môi trường Dev/Prod | 14/05/2026 | 14/05/2026 | <https://000066.awsstudygroup.com/vi/> |
| 6 | - Cài đặt AWS SAM CLI trên môi trường máy local<br>- Khởi tạo project SAM mới, phân tích cấu trúc file template.yaml (AWS CloudFormation)<br>- Thực hiện build và deploy ứng dụng Serverless lên AWS bằng lệnh `sam deploy` | 15/05/2026 | 15/05/2026 | <https://000080.awsstudygroup.com/vi/> |

### Kết quả đạt được tuần 4:

* **Lập trình điện toán Serverless với AWS Lambda:**
  * Hiểu rõ cơ chế kích hoạt theo sự kiện (event sources) và cách Lambda co giãn tự động theo lượng request.
  * Tối ưu hóa cấu hình Memory từ đó cải thiện tốc độ xử lý và chi phí tương ứng.
  * Thành thạo việc đọc ghi CloudWatch Logs để phân tích lỗi trong mã nguồn Lambda.

* **Thiết kế và triển khai API Gateway:**
  * Triển khai thành công hệ thống HTTP API Gateway làm lớp trung gian nhận request từ Client.
  * Cấu hình thành công CORS giúp ngăn chặn các cuộc tấn công cross-site scripting khi Frontend gọi API.
  * Áp dụng Lambda Proxy Integration để truyền toàn bộ dữ liệu request (headers, query, body) vào event object của Lambda một cách nguyên bản.

* **Tự động hóa triển khai với AWS SAM:**
  * Định nghĩa toàn bộ hạ tầng serverless bao gồm Lambda, API Gateway và DynamoDB trong tệp tin `template.yaml`.
  * Thực hiện triển khai hạ tầng dưới dạng mã (IaC) nhanh chóng, đảm bảo tính nhất quán giữa môi trường local và cloud.
