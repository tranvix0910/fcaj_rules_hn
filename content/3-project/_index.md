---
title: "Quy định về project"
date: 2025-01-12
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

### 1. Nội dung bắt buộc của project

Project (báo cáo cuối khóa) **phải được viết bằng 2 ngôn ngữ: tiếng Anh và tiếng Việt**.

### Các phần tối thiểu cần có trong báo cáo

#### 1.1. Thông tin sinh viên

* Họ tên
* Số điện thoại
* Email
* Trường
* Chuyên ngành
* Công ty thực tập
* Vị trí thực tập
* Thời gian thực tập

#### 1.2. Worklog (Nhật ký công việc theo tuần)

* Ghi rõ từ **Week 1 → Week 12**
* Mỗi tuần cần mô tả:
  * Công việc đã thực hiện
  * Kết quả đạt được

#### 1.3. Proposal (Đề xuất dự án)

* Tổng quan dự án
* Mục tiêu
* Vấn đề cần giải quyết
* Kiến trúc giải pháp
* Timeline thực hiện
* Ngân sách dự kiến (nếu có)
* Rủi ro tiềm ẩn

> Ví dụ: **IoT Weather Platform trên AWS**

#### 1.4. Events Participated (Sự kiện đã tham gia)

Mỗi sự kiện cần ghi rõ:

* Tên sự kiện
* Thời gian và địa điểm
* Vai trò của bản thân
* Nội dung chính
* Bài học rút ra và đóng góp cá nhân

#### 1.5. Workshop (Project kỹ thuật chính)

* Overview (Tổng quan)
* Prerequisite (Điều kiện tiên quyết)
* Mô tả kiến trúc hệ thống
* Các bước thực hành chi tiết, ví dụ:
  * Truy cập S3 từ VPC / on-premises
  * Cấu hình VPC Endpoint
  * Thiết lập IAM Policy
  * Kiểm thử
  * Dọn dẹp tài nguyên (Clean-up)

#### 1.6. Self-evaluation (Tự đánh giá)

Đánh giá bản thân theo các tiêu chí sau, mỗi tiêu chí chọn mức **Tốt / Khá / Trung bình** kèm nhận xét:

* Kiến thức
* Khả năng học hỏi
* Tính chủ động
* Kỷ luật
* Giao tiếp
* Teamwork
* Giải quyết vấn đề
* Đóng góp cho dự án

#### 1.7. Sharing and Feedback (Chia sẻ và phản hồi)

* Cảm nhận về chương trình
* Mức độ hài lòng
* Các điểm cần cải thiện
* Có giới thiệu chương trình cho bạn bè không? Vì sao?

---

### 2. Hình thức và công cụ thực hiện project

#### 2.1. Hình thức khuyến khích

* Workshop website: [Mẫu workshop ↗](https://workshop-sample.fcjuni.com/)
* Template gợi ý: [FCAJ Workshop Template ↗](https://github.com/thienluhoan/fcj-workshop-template) trên GitHub

#### 2.2. Yêu cầu bắt buộc

* Có **đầy đủ 2 ngôn ngữ (vi / en)** cho phần nội dung chính
* Cấu trúc rõ ràng theo các mục đã nêu, bao gồm:
  * Hình ảnh minh họa
  * Sơ đồ kiến trúc
  * Code snippet
  * File đính kèm (CloudFormation, Dockerfile, script, …) nếu phù hợp
* Có thể tham khảo **project mẫu** (link trong tài liệu)
* **Project phải do sinh viên tự viết**, không được sao chép y nguyên project mẫu

---

### 3. Yêu cầu đối với project kỹ thuật (Workshop)

Project nên:

* Là **use-case thực tế trên AWS**, ví dụ:
  * Serverless application
  * Data pipeline
  * Monitoring system
  * IoT
* Sử dụng **ít nhất 3 dịch vụ AWS**

#### 3.1. Các yếu tố cần thể hiện

* **Thiết kế kiến trúc:**
  * Sơ đồ kiến trúc rõ ràng
  * Danh sách dịch vụ sử dụng
  * Lý do lựa chọn từng dịch vụ

* **Triển khai end-to-end:**
  * Các bước hướng dẫn chi tiết
  * Người khác có thể tái thực hiện được

* **Kiểm thử và đo lường:**
  * Log
  * Metric
  * Alert

* **Tối ưu hóa:**
  * Chi phí
  * Bảo mật cơ bản
  * Clean-up tài nguyên để tránh phát sinh chi phí

---

### 4. Thang điểm đánh giá project

#### 4.1. Ý tưởng và mục tiêu (1.0 điểm)

* **Bối cảnh và bài toán:**
  * Hệ thống dùng để làm gì?
  * Đối tượng sử dụng là ai?
  * Giải quyết vấn đề gì?
  * Ví dụ: giám sát thời tiết, logging, monitoring microservice

* **Mục tiêu cụ thể:**
  * Output mong muốn (dashboard, API, alert, …)
  * Tiêu chí đánh giá thành công

* **Phù hợp với chương trình:**
  * Use-case gắn liền với FCAJ / AWS
  * Không quá chung chung hoặc lệch chủ đề Cloud

#### 4.2. Kiến trúc và thiết kế kỹ thuật (2.0 điểm)

* **Sơ đồ kiến trúc:**
  * Diagram rõ ràng (draw.io, PowerPoint, Excalidraw, …)
  * Thể hiện đầy đủ các dịch vụ AWS và luồng dữ liệu

* **Lựa chọn dịch vụ:**
  * Giải thích lý do chọn S3 / Lambda / API Gateway / DynamoDB, …
  * Dựa trên chi phí, độ đơn giản, serverless, managed service

* **Bảo mật và IAM cơ bản:**
  * IAM Role
  * Nguyên tắc Least Privilege
  * Hạn chế public resource
  * Không hard-code access key

* **Khả năng mở rộng và vận hành:**
  * Scale: Auto Scaling, event-driven, SQS, …
  * Monitoring: CloudWatch, Alarm

#### 4.3. Triển khai và lab step-by-step (2.0 điểm)

* **Prerequisite:**
  * Tài khoản AWS
  * Region sử dụng
  * Công cụ: AWS CLI, SAM / CDK / Terraform (nếu có)
  * Quyền IAM cần thiết

* **Hướng dẫn chi tiết:**
  * Chia rõ từng bước (Step 1, Step 2, …)
  * Có screenshot / CLI command / console guide
  * Thực hiện được end-to-end

* **Test và validation:**
  * Gửi request
  * Kiểm tra log và metric
  * Kiểm thử trường hợp lỗi
  * Kết quả mong đợi

* **Clean-up:**
  * Xóa resource
  * Delete stack
  * Xóa bucket
  * Xóa alarm

#### 4.4. Tài liệu workshop và trình bày (0.5 điểm)

* **Song ngữ:**
  * Nội dung chính đầy đủ cả tiếng Việt và tiếng Anh
  * Dịch đúng ý, không lệch nghĩa nghiêm trọng

* **Cấu trúc website:**
  * Đúng layout template
  * Mục lục rõ ràng
  * Navigation hợp lý

* **Trình bày:**
  * Nội dung dễ đọc
  * Có code block
  * Có hình ảnh minh họa
  * Ít lỗi chính tả

#### 4.5. Đóng góp cá nhân (0.5 điểm)

* **Mức độ tự thực hiện:**
  * Không chỉ sao chép từ mẫu
  * Có tùy biến và sáng tạo riêng:
    * Thêm tính năng
    * Thêm dịch vụ
    * Sử dụng dữ liệu khác
    * Áp dụng cách kiểm thử khác

* **Reflection (Nhìn lại quá trình):**
  * Khó khăn gặp phải
  * Cách giải quyết
  * Hướng phát triển trong tương lai
