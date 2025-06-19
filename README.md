# 📘 Dự án Thực hành Gửi Yêu cầu CRUD đến API bằng Postman

## 🔹 Bước 1: Giới thiệu và Mục tiêu Dự án

### 📌 Giới thiệu ngắn gọn
Trong phát triển phần mềm, đặc biệt là với các ứng dụng web và di động, **API (Application Programming Interface)** đóng vai trò là cầu nối giữa frontend và backend. Việc kiểm thử và gửi yêu cầu đến API là kỹ năng quan trọng với mọi lập trình viên và tester.

### 🎯 Mục tiêu cụ thể
Dự án này giúp người học:

- Hiểu cách hoạt động của các phương thức HTTP thường dùng:
  - `GET`: Lấy dữ liệu
  - `POST`: Tạo mới
  - `PUT`: Ghi đè toàn bộ
  - `PATCH`: Sửa một phần
  - `DELETE`: Xoá dữ liệu

- Sử dụng **Postman** – công cụ phổ biến để gửi và kiểm thử API mà không cần viết mã.

- Thực hành trên **API miễn phí** `JSONPlaceholder` để thao tác CRUD với dữ liệu mẫu.

- Viết **test** kiểm tra phản hồi và sử dụng **Collection Runner** để gửi hàng loạt request.

- Rèn luyện kỹ năng:
  - Phân tích
  - Tổ chức request
  - Làm việc theo mô hình REST trong môi trường thực tế

---

## 🔹 Bước 2: Công cụ, Tài nguyên và Dữ liệu Sử dụng

### 🛠️ 1. Công cụ chính

| Công cụ         | Vai trò                                                                 |
|----------------|-------------------------------------------------------------------------|
| Postman        | Giao diện gửi request HTTP đến API, kiểm tra phản hồi, tự động hóa      |
| JSONPlaceholder| API giả lập miễn phí, hỗ trợ thao tác CRUD mà không cần backend thật     |
| JSON           | Định dạng dữ liệu được sử dụng khi gửi/nhận qua API                     |

---

### 🌐 2. API sử dụng – JSONPlaceholder

- Trang chủ: [https://jsonplaceholder.typicode.com](https://jsonplaceholder.typicode.com)
- Đặc điểm:
  - Không cần đăng ký tài khoản
  - Dữ liệu mô phỏng, không thay đổi thật
  - Hỗ trợ nhiều endpoint như: `/posts`, `/comments`, `/users`, v.v.

- **Endpoint sử dụng trong dự án**:
https://jsonplaceholder.typicode.com/posts

### 📋 3. Cấu trúc Dữ liệu Mẫu

Dữ liệu phản hồi từ API có cấu trúc như sau:

```json
{
"userId": 1,
"id": 1,
"title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
"body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum..."
}
```

Mỗi bài viết bao gồm 4 trường dữ liệu:

| Trường   | Kiểu dữ liệu | Mô tả                          |
|----------|--------------|-------------------------------|
| userId   | Số nguyên     | ID của người tạo bài viết     |
| id       | Số nguyên     | ID duy nhất của bài viết      |
| title    | Chuỗi         | Tiêu đề bài viết              |
| body     | Chuỗi         | Nội dung bài viết             |

---

## 🧪 Môi trường Thử nghiệm

- ✅ **Postman** bản desktop (Windows)
- ❌ **Không cần xác thực**
- 🌐 **Không yêu cầu internet tốc độ cao**
- 🔁 **Dữ liệu không thay đổi phía server**, phù hợp để **thử nghiệm lặp lại**

