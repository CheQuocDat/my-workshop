---
title: "Nhật ký công việc Tuần 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---
### Mục tiêu tuần 3:

* Tìm hiểu các dịch vụ Cơ sở dữ liệu (Database Services) trên AWS bao gồm Amazon RDS (Cơ sở dữ liệu quan hệ), Amazon DynamoDB (NoSQL) và Amazon ElastiCache (Bộ nhớ đệm trong bộ nhớ).
* Triển khai, bảo mật và kết nối ứng dụng với Amazon RDS MySQL.
* Thiết kế schema và tối ưu hóa hiệu năng truy vấn với Amazon DynamoDB.
* Tích hợp bộ nhớ đệm ElastiCache (Redis) để tăng tốc độ phản hồi và giảm tải cho database chính.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu các khái niệm cơ bản về Amazon RDS (Relational Database Service)<br>- Phân biệt Multi-AZ deployments (tính sẵn sàng cao) vs Read Replicas (tối ưu đọc)<br>- Thiết lập DB Subnet Groups để phân chia mạng an toàn cho Database | 04/05/2026 | 04/05/2026 | <https://000005.awsstudygroup.com/vi/> |
| 3 | - Khởi tạo một DB Instance MySQL trên Amazon RDS<br>- Cấu hình Security Group chỉ cho phép kết nối từ ứng dụng/EC2 cụ thể<br>- Kết nối client/application và thực hành các câu lệnh DDL/DML<br>- Thiết lập cơ chế tự động sao lưu (Automated Backups) và DB Snapshots | 05/05/2026 | 05/05/2026 | <https://000005.awsstudygroup.com/vi/> |
| 4 | - Tìm hiểu cơ sở dữ liệu NoSQL Amazon DynamoDB<br>- Thiết kế cấu trúc Primary Key: Partition Key vs Composite Key (Partition Key + Sort Key)<br>- Phân biệt Read/Write Capacity Modes: Provisioned (with Auto Scaling) vs On-Demand | 06/05/2026 | 06/05/2026 | <https://000060.awsstudygroup.com/vi/> |
| 5 | - Khởi tạo bảng DynamoDB và thực hành các thao tác CRUD (PutItem, GetItem, UpdateItem, DeleteItem)<br>- Phân biệt các phương thức truy xuất: Query vs Scan và tác động đến chi phí<br>- Tạo và cấu hình Global Secondary Indexes (GSI) và Local Secondary Indexes (LSI) | 07/05/2026 | 07/05/2026 | <https://000060.awsstudygroup.com/vi/> |
| 6 | - Tìm hiểu dịch vụ caching Amazon ElastiCache<br>- So sánh tính năng và use cases giữa Redis và Memcached<br>- Khởi tạo ElastiCache Redis cluster và cấu hình kết nối bảo mật<br>- Tích hợp caching vào ứng dụng để tối ưu hóa thời gian phản hồi | 08/05/2026 | 08/05/2026 | <https://000061.awsstudygroup.com/vi/> |

### Kết quả đạt được tuần 3:

* **Quản trị cơ sở dữ liệu quan hệ Amazon RDS:**
  * Khởi tạo thành công database MySQL có kiến trúc Multi-AZ sẵn sàng cho môi trường Production.
  * Thiết lập bảo mật DB Subnet Groups và Security Group cô lập database khỏi Internet công cộng.
  * Hiểu rõ cơ chế tự động backup và khôi phục dữ liệu từ point-in-time snapshot.

* **Thực hành thiết kế và vận hành NoSQL với DynamoDB:**
  * Thiết kế Schema hiệu quả cho DynamoDB, áp dụng Partition Key và Sort Key để phân bổ dữ liệu tối ưu.
  * Hiểu rõ cơ chế tính phí thông qua WCU/RCU và biết cách cấu hình chế độ On-Demand để tiết kiệm chi phí cho tải không dự đoán trước.
  * Nắm vững cách truy xuất dữ liệu bằng Query để tối ưu hiệu năng thay vì sử dụng Scan (quét toàn bộ bảng).
  * Tạo thành công chỉ mục phụ (GSI) giúp linh hoạt hóa các điều kiện tìm kiếm.

* **Tối ưu hóa hiệu năng ứng dụng với ElastiCache:**
  * Cấu hình thành công ElastiCache Redis cluster làm lớp lưu trữ tạm thời cho dữ liệu ít thay đổi.
  * Cải thiện thời gian phản hồi của ứng dụng đáng kể (dưới mức mili-giây) và giảm tải tài nguyên CPU cho cơ sở dữ liệu chính.
