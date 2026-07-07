---
title: "Nhật ký công việc Tuần 7"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---
### Mục tiêu tuần 7:

* Xây dựng kiến trúc hồ dữ liệu Serverless Data Lake trên AWS sử dụng Amazon S3 làm lõi lưu trữ.
* Tự động hóa quá trình thu thập siêu dữ liệu (metadata) và chuyển đổi dữ liệu (ETL) sử dụng AWS Glue.
* Sử dụng Amazon Athena để chạy các truy vấn SQL trực tiếp trên S3 và trực quan hóa dữ liệu kinh doanh với Amazon QuickSight.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu kiến trúc Data Lake và các giai đoạn xử lý dữ liệu lớn (Ingest, Store, Process, Analyze)<br>- Cấu hình Amazon S3 Buckets phân cấp cho các vùng dữ liệu: Raw, Processed và Curated Zone<br>- Thiết lập quyền truy cập IAM cho các dịch vụ phân tích dữ liệu | 01/06/2026 | 01/06/2026 | <https://000035.awsstudygroup.com/vi/> |
| 3 | - Tìm hiểu AWS Glue và các thành phần: Data Catalog, Crawlers, Connections và Jobs<br>- Tạo và cấu hình AWS Glue Crawler để quét dữ liệu thô trên S3<br>- Xác minh kết quả quét và tự động tạo sơ đồ bảng (Schema) trong Glue Data Catalog | 02/06/2026 | 02/06/2026 | <https://000035.awsstudygroup.com/vi/> |
| 4 | - Thiết lập một tiến trình ETL (Extract, Transform, Load) Job trong AWS Glue<br>- Cấu hình chuyển đổi định dạng dữ liệu từ dạng hàng (như CSV/JSON) sang dạng cột (Parquet)<br>- Tối ưu hóa phân vùng dữ liệu (Partitioning) trên S3 để tăng tốc truy vấn và giảm chi phí | 03/06/2026 | 03/06/2026 | <https://000070.awsstudygroup.com/vi/> |
| 5 | - Tìm hiểu dịch vụ truy vấn Serverless Amazon Athena<br>- Thực hiện cấu hình vị trí lưu kết quả truy vấn trên S3<br>- Viết các câu lệnh SQL chuẩn để thực hiện phân tích, lọc dữ liệu trực tiếp từ các bảng trong Data Catalog | 04/06/2026 | 04/06/2026 | <https://000106.awsstudygroup.com/vi/> |
| 6 | - Đăng ký và thiết lập môi trường Amazon QuickSight<br>- Cấu hình kết nối dữ liệu từ Amazon Athena và import dữ liệu vào bộ nhớ SPICE của QuickSight<br>- Thiết kế các biểu đồ tương tác, tạo Dashboard báo cáo kinh doanh và phân quyền chia sẻ | 05/06/2026 | 05/06/2026 | <https://000073.awsstudygroup.com/vi/> |

### Kết quả đạt được tuần 7:

* **Xây dựng Data Lake Serverless thành công:**
  * Triển khai hoàn chỉnh cấu trúc phân vùng lưu trữ hồ dữ liệu trên S3, đáp ứng các tiêu chuẩn quản trị dữ liệu lớn.
  * Tận dụng tối đa khả năng lưu trữ không giới hạn của S3 với chi phí cực kỳ tối ưu.

* **Tự động hóa ETL với AWS Glue:**
  * Vận hành thành công Glue Crawler để tự động phân tích cấu trúc cấu trúc dữ liệu không đồng nhất và lập danh mục dữ liệu tập trung.
  * Thực hiện thành công Job ETL chuyển đổi dữ liệu sang định dạng Parquet, giảm đến 80% dung lượng dữ liệu cần quét khi truy vấn.

* **Truy vấn và trực quan hóa báo cáo:**
  * Sử dụng Athena thực hiện truy vấn ad-hoc trực tiếp trên S3 với thời gian phản hồi nhanh mà không cần tốn chi phí vận hành máy chủ database.
  * Thiết kế hoàn chỉnh dashboard phân tích dữ liệu trên QuickSight trực quan, sinh động, hỗ trợ phân tích đa chiều phục vụ ra quyết định kinh doanh.
