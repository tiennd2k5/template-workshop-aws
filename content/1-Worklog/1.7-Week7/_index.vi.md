---
title: "Worklog Tuần 7"
date: 2026-07-24
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:
* Kiểm thử toàn diện hệ thống tích hợp end-to-end trên AWS S3 và EC2.
* Kiểm thử khả năng chịu lỗi (Failover & Error Handling) khi ngắt kết nối DB hoặc ngắt mạng.
* Kiểm thử giao diện trải nghiệm người dùng (UX/UI), luồng quét khuôn mặt và phát nhạc/video.

### Các công việc triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành |
| --- | --- | --- | --- |
| 2 | - Thực hiện End-to-End Testing cho các chức năng Đăng ký, Đăng nhập Face ID, Đăng bài Feed, Bookmark | 20/07/2026 | 21/07/2026 |
| 4 | - Kiểm thử tải trang và độ trễ phản hồi của webcam scanner trong môi trường mạng thực tế | 22/07/2026 | 23/07/2026 |
| 6 | - Kiểm thử xử lý sự cố (Error boundary, rate limit 429, session expiry 401) | 24/07/2026 | 26/07/2026 |

### Kết quả đạt được tuần 7:
* Toàn bộ luồng nghiệp vụ ứng dụng trên AWS S3 + EC2 hoạt động ổn định và chính xác.
* Khả năng bắt lỗi và phản hồi cho người dùng được xử lý mượt mà.
