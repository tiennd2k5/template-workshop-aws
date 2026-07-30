---
title: "Worklog Tuần 4"
date: 2026-07-03
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:
* Khởi tạo và kết nối cơ sở dữ liệu AWS RDS PostgreSQL (Free Tier).
* Thiết lập Security Group liên kết giữa EC2 Backend và RDS PostgreSQL.
* Cấu hình SQLAlchemy `DATABASE_URL` hỗ trợ cả SQLite local và Cloud RDS PostgreSQL.
* Thực hiện script seed dữ liệu ban đầu và khởi tạo admin mặc định.

### Các công việc triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành |
| --- | --- | --- | --- |
| 2 | - Tạo AWS RDS PostgreSQL Instance trên AWS Console | 29/06/2026 | 29/06/2026 |
| 3 | - Cấu hình Inbound Rule cho Security Group của RDS chỉ cho phép IP EC2 kết nối qua Port 5432 | 30/06/2026 | 30/06/2026 |
| 4 | - Thêm driver `psycopg2-binary` vào `backend/requirements.txt` | 01/07/2026 | 01/07/2026 |
| 5 | - Cập nhật `backend/services/db_models.py` để linh hoạt đọc `DATABASE_URL` từ `.env` | 02/07/2026 | 03/07/2026 |
| 6 | - Kiểm thử tính năng tự tạo bảng và seed admin `123456` khi khởi chạy container trên Cloud | 04/07/2026 | 05/07/2026 |

### Kết quả đạt được tuần 4:
* Đã kết nối thành công Backend EC2 tới AWS RDS PostgreSQL.
* Dữ liệu ứng dụng (Users, Posts, Knowledge, Games, Music, Logs) được lưu trữ an toàn trên RDS.

![Phân hệ Thư viện Âm nhạc Trực tuyến](/images/music.png)
![Phân hệ Cổng Tin tức Game](/images/games.png)
![Phân hệ Bảng tin Đa phương tiện](/images/feed.png)
