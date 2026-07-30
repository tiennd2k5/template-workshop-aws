---
title: "Worklog Tuần 5"
date: 2026-07-24
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:
* Tích hợp nhật ký ứng dụng (Application Logging) với dịch vụ AWS CloudWatch Logs.
* Cấu hình theo dõi chỉ số (Metric Filters & Alarms) cho EC2 và ứng dụng Backend.

### Các công việc triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành |
| --- | --- | --- | --- |
| 2 | - Tìm hiểu dịch vụ AWS CloudWatch Logs & SDK `watchtower` | 13/07/2026 | 13/07/2026 |
| 3 | - Thêm `watchtower` vào `backend/requirements.txt` và cập nhật `backend/services/logging_service.py` | 14/07/2026 | 15/07/2026 |
| 4 | - Cấu hình gửi log sự kiện nhận diện Face ID, đăng nhập, lỗi DB về CloudWatch Log Group `/fav-web/backend` | 16/07/2026 | 17/07/2026 |
| 5 | - Khởi tạo CloudWatch Alarm cảnh báo khi mức sử dụng CPU của EC2 vượt ngưỡng 80% | 18/07/2026 | 19/07/2026 |

### Kết quả đạt được tuần 5:
* Đã tự động gửi log thực thi ứng dụng từ EC2 lên AWS CloudWatch Logs.
* Thiết lập hệ thống giám sát tải CPU và theo dõi sự cố vận hành hiệu quả. 

![AWS CloudWatch Logging & Monitoring](/images/cloudwatch.png)
