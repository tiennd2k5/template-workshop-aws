---
title: "Sự kiện 1: Event Meeting"
date: 2026-07-30
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# Sự kiện 1: Event Meeting 

- **Tên sự kiện:** Event Meeting 
- **Thời gian:** 11/07/2026
- **Vai trò:** Người tham dự
- **Drive hình ảnh & slide sự kiện:** [Google Drive Folder](https://drive.google.com/drive/folders/1GfbwjmjqX4xpUiN5UZ62xLbRSs9-fwyM?usp=sharing)

---

### Nội dung chương trình & Các chủ đề chính:

Sự kiện bao gồm vòng chung kết Cloud Architect, cùng với các buổi chia sẻ kiến thức kỹ thuật, trong đó các thành viên có kinh nghiệm của AWS First Cloud AI Journey (FCAJ) chia sẻ kiến thức chuyên môn, kinh nghiệm thực tế và các phương pháp tốt trong lĩnh vực công nghệ Cloud và kỹ thuật phần mềm.

1. **Nguyễn Huỳnh Sơn**
   - **Chủ đề:** SLA và Monitoring – Từ SLA đến Monitoring những yếu tố thực sự quan trọng
   - **Bài học chính:**
     - Hoạt động Monitoring nên tập trung vào trải nghiệm khách hàng và kết quả kinh doanh, thay vì chỉ theo dõi các chỉ số của hạ tầng.
     - Hạ tầng hoạt động ổn định không đồng nghĩa với việc trải nghiệm người dùng cũng đang tốt.
     - Xây dựng hệ thống Monitoring theo nhiều lớp: Trải nghiệm khách hàng → Chỉ số kinh doanh → Ứng dụng → Hạ tầng → Tài nguyên Cloud.
     - Monitoring là một phần của quản lý rủi ro, giúp phát hiện vấn đề trước khi chúng ảnh hưởng đến khách hàng hoặc vi phạm SLA.
     - Theo AWS Shared Responsibility Model, AWS chịu trách nhiệm quản lý hạ tầng Cloud, trong khi khách hàng chịu trách nhiệm về độ tin cậy của ứng dụng và trải nghiệm người dùng.
     - Nên theo dõi các hành trình của người dùng (ví dụ: đăng nhập, thanh toán, tìm kiếm, đặt hàng) thay vì chỉ dựa vào CPU, bộ nhớ hoặc các health check.

2. **Ngô Lê Tấn Huy**
   - **Chủ đề:** Inside the Exam – AWS Cloud Practitioner
   - **Bài học chính:**
     - Kỳ thi AWS Certified Cloud Practitioner (CLF-C02) tập trung vào kiến thức nền tảng về Cloud, không yêu cầu lập trình hoặc triển khai kỹ thuật chuyên sâu.
     - Ưu tiên nắm vững các khái niệm cốt lõi của AWS: Cloud Concepts, Security & Compliance, Cloud Technology & Services, và Billing & Support dựa trên tỷ trọng của từng phần trong kỳ thi.
     - Học các dịch vụ AWS dựa trên chức năng và trường hợp sử dụng chính cùng các từ khóa đặc trưng, thay vì cố gắng ghi nhớ mọi tính năng (ví dụ: SQS → decoupling, S3 → object storage, IAM → access management).
     - Nắm vững các nguyên tắc quan trọng của AWS như Shared Responsibility Model, IAM Least Privilege, AWS Well-Architected Framework và Cloud Adoption Framework, vì đây là những nội dung thường xuất hiện trong kỳ thi.
     - Việc ôn thi hiệu quả nên tập trung vào phân tích các câu trả lời sai, thực hành trực tiếp với AWS Free Tier và hiểu lý do tại sao mỗi đáp án đúng hoặc sai, thay vì chỉ làm thật nhiều đề luyện tập.
     - Trong quá trình thi, có thể tăng độ chính xác bằng cách loại bỏ các đáp án rõ ràng không phù hợp, tránh suy nghĩ quá phức tạp, chú ý đến các từ khóa như NOT, Least Cost, Most Scalable, đồng thời sử dụng chức năng đánh dấu câu hỏi để quản lý thời gian hiệu quả.

3. **Thịnh Nguyễn**
   - **Chủ đề:** Securing Your Web Apps with AWS Security Agent
   - **Bài học chính:**
     - Các hoạt động đánh giá bảo mật truyền thống thường tốn nhiều thời gian, chi phí và có tính nhất quán hạn chế, khiến việc kiểm thử bảo mật liên tục khó mở rộng.
     - AWS Security Agent sử dụng Amazon Bedrock để tự động thực hiện các tác vụ bảo mật trong vòng đời phát triển phần mềm, bao gồm đánh giá thiết kế, kiểm tra mã nguồn và penetration testing.
     - Thực hiện Shift Left Security bằng cách phát hiện lỗ hổng sớm thông qua đánh giá kiến trúc và phân tích Pull Request tự động, từ đó giảm chi phí xử lý vấn đề ở các giai đoạn sau.
     - Khác với các trợ lý AI truyền thống, Agent có khả năng cung cấp các phát hiện có thể kiểm chứng bằng cách thực hiện khai thác thực tế và tạo attack graph, giúp xác nhận lỗ hổng thay vì chỉ đưa ra phân tích lý thuyết.
     - Kiểm thử bảo mật bằng AI có thể giảm đáng kể sự phụ thuộc vào penetration testing thủ công, nhưng nên được sử dụng để bổ trợ thay vì thay thế chuyên môn của con người, đặc biệt đối với các business logic phức tạp và cơ chế xác thực nâng cao như MFA hoặc mTLS.
     - Doanh nghiệp cũng cần đánh giá sự cân bằng giữa chi phí và lợi ích khi sử dụng các Security Agent tự động, vì chi phí phụ thuộc vào thời gian thực thi, nhưng trong nhiều trường hợp vẫn có thể thấp hơn đáng kể so với việc thuê các đội penetration testing truyền thống.