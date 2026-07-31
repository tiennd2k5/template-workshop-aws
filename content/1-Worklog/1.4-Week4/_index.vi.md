---

title: "Nhật ký công việc Tuần 4"
date: 2026-07-05
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
----------------------

### Mục tiêu Tuần 4:

* Thiết lập cơ sở dữ liệu PostgreSQL trên AWS RDS và kết nối với ứng dụng.
* Cấu hình các quy tắc Security Group để cho phép EC2 Backend giao tiếp với RDS PostgreSQL.
* Cập nhật cấu hình SQLAlchemy để hỗ trợ đồng thời SQLite trên môi trường local và PostgreSQL trên AWS RDS.
* Xây dựng và thực thi các script khởi tạo dữ liệu ban đầu, bao gồm tài khoản quản trị và các danh mục mặc định.

### Nội dung công việc:

| Ngày  | Nội dung thực hiện                                                                                                                                                                       | Ngày bắt đầu | Ngày hoàn thành |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| Thứ 2 | - Khởi tạo và cấu hình PostgreSQL Database Instance bằng AWS RDS thông qua AWS Console                                                                                                   | 29/06/2026   | 29/06/2026      |
| Thứ 3 | - Điều chỉnh cấu hình Security Group của RDS <br> - Cho phép EC2 Backend kết nối đến PostgreSQL thông qua Port 5432                                                                      | 30/06/2026   | 30/06/2026      |
| Thứ 4 | - Bổ sung thư viện kết nối PostgreSQL bằng cách thêm `psycopg2-binary` vào `backend/requirements.txt`                                                                                    | 01/07/2026   | 01/07/2026      |
| Thứ 5 | - Cập nhật `backend/services/db_models.py` để đọc và xử lý biến `DATABASE_URL` từ file `.env` <br> - Đảm bảo ứng dụng có thể sử dụng cả SQLite local và PostgreSQL trên môi trường cloud | 02/07/2026   | 03/07/2026      |
| Thứ 6 | - Kiểm tra cơ chế tự động migration trên môi trường cloud <br> - Chạy script seed để tạo tài khoản quản trị (`123456`) và các dữ liệu mặc định trên RDS                                  | 04/07/2026   | 05/07/2026      |

### Kết quả đạt được trong Tuần 4:

* Kết nối thành công FastAPI Backend trên EC2 với cơ sở dữ liệu PostgreSQL được triển khai trên AWS RDS.
* Dữ liệu của ứng dụng, bao gồm Users, Posts, Knowledge, Games, Music và Logs, được lưu trữ lâu dài trên RDS.



