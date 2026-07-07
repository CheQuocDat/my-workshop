---
title: "Nhật ký công việc Tuần 11"
date: 2026-07-06
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---
### Mục tiêu tuần 11:

* Phát triển giao diện Frontend nâng cao (Mock Interview workspace, Dashboard thống kê, Gamification).
* Tích hợp toàn diện Frontend với các API Gateway của dự án.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Thiết kế không gian làm việc phỏng vấn giả lập (Mock Interview UI): Tích hợp phát file âm thanh câu hỏi từ S3 và nút thu âm tương tác | 29/06/2026 | 29/06/2026 | Audio element & React state guides |
| 3 | - Phát triển Dashboard thống kê tiến độ học tập: vẽ biểu đồ điểm số, hiển thị lịch sử làm bài trắc nghiệm và tự luận | 30/06/2026 | 30/06/2026 | Chart.js & Recharts docs |
| 4 | - Tích hợp tính năng Gamification: Cộng điểm kinh nghiệm (XP), thăng cấp độ, và mở khóa huy hiệu (Badges) khi hoàn thành các chủ đề | 01/07/2026 | 01/07/2026 | Tài liệu thiết kế hệ thống tương tác |
| 5 | - Thực hiện kết nối API Gateway: Đọc JWT Token từ Cognito và gửi kèm vào headers Authorization của mọi request<br>- Viết logic upload file ghi âm câu trả lời lên S3 qua Presigned URL | 02/07/2026 | 02/07/2026 | AWS Axios Integration & S3 uploads |
| 6 | - Tối ưu hóa giao diện đa thiết bị (Responsive Design)<br>- Sửa lỗi trải nghiệm người dùng (UX bugs) trong quá trình ghi âm và phát âm thanh | 03/07/2026 | 03/07/2026 | CSS Flexbox/Grid & Mobile testing |

### Kết quả đạt được tuần 11:

* **Hoàn thiện Frontend nâng cao:**
  * **Mock Interview Workspace:** Giao diện tối giản hiện đại. Người dùng có thể nghe giọng nói AI đặt câu hỏi chuyên môn, nhấp chuột để bắt đầu ghi âm câu trả lời, xem trực quan thanh tiến trình ghi âm và gửi bài phỏng vấn.
  * **Interactive Dashboard:** Tích hợp thư viện biểu đồ, hiển thị trực quan tỷ lệ trả lời đúng theo từng kỹ năng (Frontend, Backend, Cloud), thống kê thời gian học tập, giúp sinh viên nhận diện các điểm yếu cần cải thiện.
  * **Gamification:** Thiết kế hệ thống khen thưởng thúc đẩy học tập. Đăng nhập hàng ngày nhận streak, làm bài quiz nhận XP, hoàn thành lộ trình mở khóa các huy hiệu độc đáo (ví dụ: "Vua Mạng AWS", "Bậc Thầy React").

* **Tích hợp API Gateway & Security:**
  * Đồng bộ cơ chế xác thực: Lưu trữ và tự động làm mới JWT token của Cognito ở Client, cấu hình CORS trên API Gateway để ngăn chặn các truy cập trái phép.
  * Upload file ghi âm trực tiếp và bảo mật từ Frontend lên S3 thông qua cơ chế Presigned URL được sinh động từ Backend Lambda, giúp giảm tải băng thông cho server API Gateway.
  * Đạt độ phản hồi tốt: UI xử lý mượt các trạng thái Loading, Success, Error khi gọi API. Giao diện thân thiện và hoạt động trơn tru trên cả desktop và mobile.
