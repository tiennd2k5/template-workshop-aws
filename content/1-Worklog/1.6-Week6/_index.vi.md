---
title: "Worklog Tuần 6"
date: 2026-07-17
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:
* Tối ưu hóa hiệu năng API nhận diện khuôn mặt bằng RAM Cache embeddings.
* Nâng cấp cơ chế xác thực kép (HttpOnly Cookie + Bearer Token Header Fallback).
* Cấu hình chuẩn hóa CORS Whitelist & Content Security Policy (CSP).

### Các công việc triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành |
| --- | --- | --- | --- |
| 2 | - Tối ưu `load_embeddings_into_cache()` trong `backend/ai_core/src/recognizer.py` nạp vector khuôn mặt vào RAM khi backend khởi động | 13/07/2026 | 13/07/2026 |
| 3 | - Bổ sung trả về `token` trong API `/auth/login` và đính kèm `Authorization: Bearer <token>` trong `frontend/src/services/api.js` | 14/07/2026 | 14/07/2026 |
| 4 | - Nới rộng cờ `connect-src` trong `frontend/index.html` và `backend/middleware/csp.py` cho phép giao tiếp API Cross-Domain | 15/07/2026 | 15/07/2026 |
| 5 | - Cấu hình `DEV_ORIGINS` trong `backend/main.py` bổ sung domain S3 Static Web | 16/07/2026 | 16/07/2026 |
| 6 | - Tối ưu hóa đóng gói frontend Vite với `manualChunks` trong `vite.config.js` giảm bundle size xuống 133 kB | 17/07/2026 | 19/07/2026 |

### Kết quả đạt được tuần 6:
* Tốc độ phản hồi của API nhận diện khuôn mặt tăng đáng kể nhờ nạp cache sẵn vào RAM.
* Khắc phục hoàn toàn sự cố xác thực cross-domain giữa S3 Frontend và EC2 Backend.
* Tối ưu hóa thời gian build và dung lượng bundle JS frontend.
