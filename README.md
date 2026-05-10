# Library Management System - API Testing Project

## 📌 Giới thiệu
Dự án này là bộ sưu tập (Collection) các API dùng để quản lý hệ thống thư viện, được xây dựng trong quá trình thực hành kỹ năng Testing. 
Dự án tập trung vào việc thiết kế cấu trúc dữ liệu, quản lý API bằng Postman và kiểm tra tính đúng đắn của luồng nghiệp vụ.

## 🛠 Công cụ sử dụng
* **Postman**: Thiết kế và kiểm thử API.
* **MySQL**: Thiết kế cơ sở dữ liệu.

## 🚀 Các tính năng chính (API Endpoints)
Hệ thống hỗ trợ các luồng nghiệp vụ cơ bản:
* **Quản lý Sách**: Thêm mới, cập nhật thông tin và xóa sách.
* **Quản lý Độc giả**: Đăng ký thông tin người mượn.
* **Quản lý Mượn sách**: Thực hiện các yêu cầu mượn sách.

## 🧪 Kỹ thuật Testing đã áp dụng
Trong dự án này đã thực hiện:
1. **Environment Variables**: Sử dụng biến môi trường trong Postman để linh hoạt giữa các môi trường.
2. **API Chaining**: Sử dụng kết quả của API này (ví dụ: `book_id`) làm đầu vào cho API tiếp theo.
3. **Scripts (Tests)**:
   - Sử dụng biến động (Dynamic Variables) để tạo tên sách và tác giả khác nhau cho mỗi lần chạy. Sử dụng Lodash để lấy ngẫu nhiên trạng thái (available/borrowed) cho sách và tự động lưu biến vào Environment Variables để sử dụng xuyên suốt luồng API
   - Kiểm tra mã trạng thái (Status Code 200, 201, 400, 404).
   - Kiểm tra cấu trúc dữ liệu trả về (JSON Schema).

## 📂 Cấu trúc thư mục
* `/Library_practice.postman_collection.json`: File chứa toàn bộ các request API.

## API Testing Cheklist
https://docs.google.com/spreadsheets/d/11w6kQ3tH8g11adcw5IuqhR2KJh3zeRQfpns1EPlNSi8/edit?gid=0#gid=0

## 📸 Test Evidence
Dưới đây là kết quả chạy test thực tế trên môi trường local:

**1. Create Book Success:**
