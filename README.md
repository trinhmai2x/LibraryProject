# Library Management System - API Testing Project

## 📌 Giới thiệu
Dự án này là bộ sưu tập (Collection) các API dùng để quản lý hệ thống thư viện, được xây dựng trong quá trình thực hành kỹ năng Testing. 
Dự án tập trung vào việc thiết kế cấu trúc dữ liệu, quản lý API bằng Postman và kiểm tra tính đúng đắn của luồng nghiệp vụ.

## 🛠 Công cụ sử dụng
* **Postman**: Thiết kế và kiểm thử API.
* **MySQL**: Thiết kế cơ sở dữ liệu và truy vấn dữ liệu thư viện.
* **Git/GitHub**: Quản lý phiên bản mã nguồn.

## 🚀 Các tính năng chính (API Endpoints)
Hệ thống hỗ trợ các luồng nghiệp vụ cơ bản:
* **Quản lý Sách**: Thêm mới, cập nhật thông tin và xóa sách.
* **Quản lý Độc giả**: Đăng ký thông tin người mượn.
* **Quản lý Mượn/Trả**: Thực hiện các yêu cầu mượn sách và kiểm tra trạng thái trả sách.

## 🧪 Kỹ thuật Testing đã áp dụng
Trong dự án này đã thực hiện:
1. **Environment Variables**: Sử dụng biến môi trường trong Postman để linh hoạt giữa các môi trường (Dev/Staging).
2. **API Chaining**: Sử dụng kết quả của API này (ví dụ: `book_id`) làm đầu vào cho API tiếp theo.
3. **Scripts (Tests)**:
   - Kiểm tra mã trạng thái (Status Code 200, 201).
   - Kiểm tra cấu trúc dữ liệu trả về (JSON Schema).
   - Kiểm tra thời gian phản hồi (Response time < 500ms).

## 📂 Cấu trúc thư mục
* `/Library_practice.postman_collection.json`: File chứa toàn bộ các request API.
* `/database_scripts.sql`: (Nếu có) Các câu lệnh SQL tạo bảng và data mẫu.

## 📖 Hướng dẫn sử dụng
1. Tải file `Library_practice.postman_collection.json` về máy.
2. Mở ứng dụng **Postman**.
3. Chọn **Import** -> Chọn file vừa tải về.
4. Cấu hình **Environment** nếu cần và bắt đầu chạy các request.
