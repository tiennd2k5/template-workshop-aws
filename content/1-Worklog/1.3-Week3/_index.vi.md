---
title: "Worklog Tuần 3"
date: 2026-06-26
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:
* Khởi tạo EC2 Instance & Security Groups trên AWS Console.
* Triển khai Backend FastAPI Docker lên EC2.
* Tích hợp lưu trữ AWS S3 cho ảnh raw, ảnh log webcam & vector embeddings (`boto3`).
* Triển khai Frontend React/Vite lên AWS S3 Static Website Hosting.

### Các công việc triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành |
| --- | --- | --- | --- |
| 2 | - Tạo AWS S3 Buckets cho media storage & frontend hosting <br> - Tích hợp `boto3` SDK vào `backend/services/s3_service.py` | 22/06/2026 | 23/06/2026 |
| 3 | - Cập nhật logic lưu ảnh webcam log và ảnh đăng ký khuôn mặt trực tiếp lên S3 Bucket | 24/06/2026 | 24/06/2026 |
| 4 | - Khởi tạo Ubuntu EC2 Instance, mở Security Group Port 80/8000/22 | 25/06/2026 | 25/06/2026 |
| 5 | - SSH vào EC2, build và chạy `fav-web-backend` container với `-v` Volume mounts | 26/06/2026 | 27/06/2026 |
| 6 | - Build `npm run build` với `VITE_API_URL` trỏ tới EC2 Public IP và upload đè lên S3 Static Web | 28/06/2026 | 28/06/2026 |

### Kết quả đạt được tuần 3:
* Backend Docker chạy thành công trên AWS EC2 (`http://52.63.251.110`).
* Frontend React/Vite live trên AWS S3 Static Website.
* Ảnh tải lên và vector khuôn mặt được tự động lưu trữ trên AWS S3.

![Quản lý AWS EC2 Instance](/images/ec2.png)
![Lưu trữ dữ liệu AWS S3 Storage](/images/s3.png)
