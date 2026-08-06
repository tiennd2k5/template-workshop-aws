---
title: "Event 3: FCAJ x Agentic AI Build Week"
date: 2026-07-30
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Event 3: AWS FCAJ Agent Forge - Deepdive

- **Tên sự kiện:** AWS FCAJ Agent Forge - Deepdive
- **Thời gian:** 01/08/2026
- **Vai trò:** Người tham dự (Attendee)
- **Hình ảnh & Slide:** [Google Drive Folder](https://drive.google.com/drive/folders/1YAY4dXyeaCeSQIU3Hhz6TrnyQM_x0ShV?usp=sharing)

---

## Nội dung chương trình

Trong ngày đầu tiên của workshop, diễn giả tập trung giới thiệu các khái niệm nền tảng về **Agentic AI** và cách xây dựng các hệ thống AI Agent có thể triển khai trong môi trường thực tế (production), thay vì chỉ dừng lại ở các bản demo.

Các nội dung chính bao gồm:

- Giới thiệu về Agentic AI và mức độ tự chủ của AI Agent.
- Model Context Protocol (MCP) và Agent-to-Agent (A2A) trong việc kết nối Agent với công cụ và các Agent khác.
- Giới thiệu Strands Agents SDK và Kiro IDE phục vụ phát triển ứng dụng Agentic AI.
- Tổng quan về nền tảng Amazon Bedrock AgentCore.
- Tìm hiểu ba thành phần quan trọng của AgentCore:
  - AgentCore Runtime
  - AgentCore Identity
  - AgentCore Gateway

---

## Kiến thức tiếp thu

### 1. Tổng quan về Agentic AI

Buổi trình bày giúp làm rõ sự khác biệt giữa chatbot thông thường và AI Agent. Một AI Agent không chỉ trả lời câu hỏi mà còn có khả năng:

- Lập kế hoạch (Planning)
- Ghi nhớ ngữ cảnh (Memory)
- Truy cập cơ sở tri thức (Knowledge Base)
- Sử dụng các công cụ bên ngoài (Tools)
- Quan sát kết quả và tự điều chỉnh (Observation & Guardrails)

Qua đó, Agent có thể tự động thực hiện nhiều bước để hoàn thành một mục tiêu thay vì chỉ phản hồi theo từng câu hỏi riêng lẻ. :contentReference[oaicite:0]{index=0}

---

### 2. Những thách thức khi triển khai AI Agent trong thực tế

Diễn giả nhấn mạnh rằng việc xây dựng một bản demo AI khá đơn giản, tuy nhiên để đưa Agent vào môi trường production cần giải quyết nhiều vấn đề như:

- Bảo mật
- Quản lý định danh (Identity)
- Kết nối với công cụ bên ngoài
- Quản lý bộ nhớ
- Theo dõi và giám sát (Observability)
- Đánh giá hiệu quả (Evaluation)
- Quản trị và kiểm soát (Governance)

Amazon Bedrock AgentCore được giới thiệu là nền tảng hỗ trợ giải quyết các bài toán này. :contentReference[oaicite:1]{index=1}

---

### 3. Amazon Bedrock AgentCore Runtime

AgentCore Runtime là môi trường serverless dành riêng cho việc triển khai AI Agent.

Một số tính năng nổi bật:

- Hỗ trợ triển khai Agent từ nhiều framework khác nhau.
- Tự động mở rộng tài nguyên mà không cần quản lý hạ tầng.
- Hỗ trợ các tác vụ chạy trong thời gian dài.
- Mỗi phiên làm việc được cách ly bằng microVM nhằm tăng cường bảo mật.
- Có thể tích hợp với các thành phần khác như Identity, Gateway, Memory và Observability. :contentReference[oaicite:2]{index=2} :contentReference[oaicite:3]{index=3}

---

### 4. Amazon Bedrock AgentCore Identity

AgentCore Identity chịu trách nhiệm quản lý xác thực và phân quyền cho AI Agent.

Buổi học giới thiệu hai khái niệm quan trọng:

- **Inbound Authentication:** xác thực người dùng trước khi được phép gọi Agent.
- **Outbound Authentication:** cho phép Agent truy cập các API hoặc tài nguyên bên ngoài thay mặt người dùng một cách an toàn.

Ngoài ra, diễn giả cũng giới thiệu **Workload Access Token (WAT)**, một loại token chứa đồng thời thông tin định danh của Agent và người dùng để đảm bảo việc truy cập tài nguyên được kiểm soát chặt chẽ. :contentReference[oaicite:4]{index=4}

---

### 5. Amazon Bedrock AgentCore Gateway

Khi AI Agent cần kết nối với nhiều API hoặc MCP Server, việc quản lý từng kết nối riêng lẻ sẽ trở nên phức tạp.

AgentCore Gateway đóng vai trò là lớp trung gian, cung cấp:

- Điểm kết nối thống nhất tới các API và công cụ.
- Hỗ trợ chuẩn Model Context Protocol (MCP).
- Quản lý quyền truy cập chi tiết.
- Chuyển đổi request/response.
- Theo dõi, ghi log và kiểm soát việc sử dụng công cụ.

Nhờ đó việc tích hợp giữa AI Agent với các hệ thống doanh nghiệp trở nên đơn giản và an toàn hơn. :contentReference[oaicite:5]{index=5}

---