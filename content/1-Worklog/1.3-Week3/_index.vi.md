---

title: "Nhật ký công việc Tuần 3"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
----------------------

### Mục tiêu Tuần 3:

* Thiết lập EC2 Instance và cấu hình các quy tắc Security Group cần thiết thông qua AWS Console.
* Triển khai FastAPI Backend dưới dạng Docker container trên môi trường EC2.
* Kết nối ứng dụng với Amazon S3 để lưu trữ hình ảnh, webcam logs và face vector embeddings thông qua `boto3`.
* Đưa React/Vite Frontend lên Amazon S3 Static Website Hosting.

### Nội dung công việc:

| Ngày  | Nội dung thực hiện                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| Thứ 2 | - Tạo các S3 Bucket phục vụ lưu trữ dữ liệu media và hosting frontend <br> - Kết nối backend với S3 bằng SDK `boto3` thông qua `backend/services/s3_service.py`                                      | 22/06/2026   | 23/06/2026      |
| Thứ 3 | - Điều chỉnh chức năng đăng ký khuôn mặt và ghi nhận webcam logs <br> - Lưu trực tiếp các hình ảnh thu được lên S3                                                                                   | 24/06/2026   | 24/06/2026      |
| Thứ 4 | - Khởi tạo Ubuntu EC2 Instance trên AWS <br> - Thiết lập Security Group cho phép truy cập các port 80, 8000 và 22                                                                                    | 25/06/2026   | 25/06/2026      |
| Thứ 5 | - Kết nối đến EC2 Instance thông qua SSH <br> - Build và chạy Docker container `fav-web-backend` với persistent Volume mounts                                                                        | 26/06/2026   | 27/06/2026      |
| Thứ 6 | - Cấu hình quá trình build frontend bằng `npm run build`, sử dụng Public IP của EC2 làm backend endpoint <br> - Upload và triển khai các file React/Vite sau khi build lên S3 Static Website Hosting | 28/06/2026   | 28/06/2026      |

### Kết quả đạt được trong Tuần 3:

* Triển khai thành công FastAPI Backend dưới dạng Docker container trên AWS EC2.
* Đưa React/Vite Frontend lên AWS S3 Static Website Hosting và có thể truy cập được.
* Các hình ảnh được upload và face vector embeddings được tự động lưu trữ trên Amazon S3.



