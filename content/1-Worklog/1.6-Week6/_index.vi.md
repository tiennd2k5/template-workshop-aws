---

title: "Nhật ký công việc Tuần 6"
date: 2026-07-18
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
----------------------

### Mục tiêu Tuần 6:

* Cải thiện tốc độ phản hồi của Face Recognition API bằng cách lưu trữ face embeddings trên RAM.
* Tăng cường cơ chế xác thực bằng cách kết hợp HttpOnly Cookie với Bearer Token Header làm phương án dự phòng.
* Chuẩn hóa cấu hình CORS và Content Security Policy (CSP) cho ứng dụng.

### Nội dung công việc:

| Ngày  | Nội dung thực hiện                                                                                                                                                      | Ngày bắt đầu | Ngày hoàn thành |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| Thứ 2 | - Tối ưu `load_embeddings_into_cache()` để nạp các face vector embeddings trực tiếp vào RAM khi ứng dụng khởi động                                                      | 13/07/2026   | 13/07/2026      |
| Thứ 3 | - Cập nhật `/auth/login` để trả về `token` xác thực <br> - Cấu hình `api.js` gửi token thông qua header `Authorization: Bearer <token>`                                 | 14/07/2026   | 14/07/2026      |
| Thứ 4 | - Điều chỉnh các directive `connect-src` trong `index.html` và `backend/middleware/csp.py` <br> - Cho phép frontend thực hiện các API request giữa các domain khác nhau | 15/07/2026   | 15/07/2026      |
| Thứ 5 | - Cập nhật biến `DEV_ORIGINS` trong `backend/main.py` <br> - Bổ sung domain của S3 Static Website vào danh sách các origin được phép truy cập                           | 16/07/2026   | 16/07/2026      |
| Thứ 6 | - Tối ưu quá trình build frontend bằng `manualChunks` của Vite <br> - Giảm kích thước JavaScript bundle xuống khoảng 133 kB                                             | 17/07/2026   | 19/07/2026      |

### Kết quả đạt được trong Tuần 6:

* Cải thiện thời gian phản hồi của Face Recognition API nhờ cơ chế nạp face embeddings vào RAM khi ứng dụng khởi động.
* Khắc phục vấn đề xác thực cross-domain giữa Frontend được host trên S3 và Backend chạy trên EC2.
* Giảm kích thước frontend bundle và cải thiện hiệu suất quá trình build bằng Vite.
