---

title: "Nhật ký công việc Tuần 5"
date: 2026-07-11
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
----------------------

### Mục tiêu Tuần 5:

* Tích hợp hệ thống ghi log của ứng dụng với AWS CloudWatch Logs.
* Thiết lập cơ chế giám sát, Metric Filter và Alarm cho EC2 Instance và các dịch vụ Backend.

### Nội dung công việc:

| Ngày  | Nội dung thực hiện                                                                                                                                                         | Ngày bắt đầu | Ngày hoàn thành |
| ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| Thứ 2 | - Tìm hiểu về dịch vụ AWS CloudWatch Logs và vai trò của nó trong việc giám sát ứng dụng <br> - Nghiên cứu cách sử dụng thư viện logging `watchtower` dành cho Python      | 06/07/2026   | 06/07/2026      |
| Thứ 3 | - Bổ sung `watchtower` vào `backend/requirements.txt` <br> - Cập nhật cơ chế ghi log trong `backend/services/logging_service.py`                                           | 07/07/2026   | 08/07/2026      |
| Thứ 5 | - Cấu hình để log của ứng dụng được gửi đến CloudWatch Log Group `/fav-web/backend` <br> - Theo dõi các sự kiện Face ID, hoạt động đăng nhập và lỗi liên quan đến Database | 09/07/2026   | 10/07/2026      |
| Thứ 7 | - Tạo CloudWatch Alarm để giám sát EC2 Instance <br> - Thiết lập Alarm kích hoạt khi mức sử dụng CPU vượt quá 80%                                                          | 11/07/2026   | 12/07/2026      |

### Kết quả đạt được trong Tuần 5:

* Log của ứng dụng được tự động thu thập từ Backend trên EC2 và gửi lên AWS CloudWatch.
* Hoàn thành cấu hình giám sát mức sử dụng CPU của EC2 và thiết lập CloudWatch Alarm tương ứng.



