---

title: "Nhật ký công việc Tuần 7"
date: 2026-07-25
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
----------------------

### Mục tiêu Tuần 7:

* Kiểm thử toàn bộ quy trình hoạt động của hệ thống giữa Frontend trên AWS S3 và Backend trên EC2.
* Đánh giá khả năng xử lý lỗi và phục hồi của hệ thống khi xảy ra mất kết nối Database hoặc độ trễ mạng cao.
* Kiểm tra trải nghiệm người dùng đối với chức năng quét khuôn mặt bằng webcam và phát nội dung media.

### Nội dung công việc:

| Ngày  | Nội dung thực hiện                                                                                                                                      | Ngày bắt đầu | Ngày hoàn thành |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| Thứ 2 | - Thực hiện kiểm thử End-to-End cho các chức năng đăng ký tài khoản, đăng nhập bằng Face ID, đăng bài trên Feed và Bookmarks                            | 20/07/2026   | 21/07/2026      |
| Thứ 4 | - Kiểm tra thời gian tải trang trong điều kiện mạng thực tế <br> - Đánh giá tốc độ phản hồi và độ ổn định của webcam face scanner                       | 22/07/2026   | 23/07/2026      |
| Thứ 6 | - Kiểm tra cơ chế xử lý lỗi và phục hồi của ứng dụng <br> - Kiểm tra phản hồi của hệ thống đối với trường hợp Rate Limit `429` và Session hết hạn `401` | 24/07/2026   | 26/07/2026      |

### Kết quả đạt được trong Tuần 7:

* Các quy trình chính của ứng dụng giữa Frontend trên AWS S3 và Backend trên EC2 hoạt động ổn định và chính xác.
* Cơ chế xử lý lỗi, phục hồi hệ thống và phản hồi cho người dùng hoạt động đúng theo yêu cầu.
