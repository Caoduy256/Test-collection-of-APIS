# Dự án Thực hành Gửi Yêu cầu CRUD đến API bằng Postman

## Giới thiệu và Mục tiêu Dự án

### Giới thiệu ngắn gọn
Trong phát triển phần mềm, đặc biệt là với các ứng dụng web và di động, API (Application Programming Interface) đóng vai trò là cầu nối giữa frontend và backend. Việc kiểm thử và gửi yêu cầu đến API là kỹ năng quan trọng với mọi lập trình viên và tester.

### Mục tiêu cụ thể
Dự án này giúp người học:

- Hiểu cách hoạt động của các phương thức HTTP thường dùng:
  - GET: Lấy dữ liệu
  - POST: Tạo mới
  - PUT: Ghi đè toàn bộ
  - PATCH: Sửa một phần
  - DELETE: Xoá dữ liệu

- Sử dụng Postman – công cụ phổ biến để gửi và kiểm thử API mà không cần viết mã.

- Thực hành trên API miễn phí JSONPlaceholder để thao tác CRUD với dữ liệu mẫu.

- Viết test kiểm tra phản hồi và sử dụng Collection Runner để gửi hàng loạt request.

- Rèn luyện kỹ năng:
  - Phân tích
  - Tổ chức request
  - Làm việc theo mô hình REST trong môi trường thực tế

---

## Công cụ, Tài nguyên và Dữ liệu Sử dụng

### 1. Công cụ chính

| Công cụ         | Vai trò                                                                 |
|----------------|-------------------------------------------------------------------------|
| Postman        | Giao diện gửi request HTTP đến API, kiểm tra phản hồi, tự động hóa      |
| JSONPlaceholder| API giả lập miễn phí, hỗ trợ thao tác CRUD mà không cần backend thật     |
| JSON           | Định dạng dữ liệu được sử dụng khi gửi/nhận qua API                     |

---

### 2. API sử dụng – JSONPlaceholder

- Trang chủ: https://jsonplaceholder.typicode.com

- Đặc điểm:
  - Không cần đăng ký tài khoản
  - Dữ liệu mô phỏng, không thay đổi thật
  - Hỗ trợ nhiều endpoint như: /posts, /comments, /users, v.v.

- Endpoint sử dụng trong dự án:
  https://jsonplaceholder.typicode.com/posts

---

### 3. Cấu trúc Dữ liệu Mẫu

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

## Môi trường Thử nghiệm

- Postman bản desktop (Windows)
- Không cần xác thực
- Không yêu cầu internet tốc độ cao
- Dữ liệu không thay đổi phía server, phù hợp để thử nghiệm lặp lại

## Thực hành Gửi Request CRUD từng bước

### 1. Lấy danh sách bài viết (GET)

- URL:  
  `https://jsonplaceholder.typicode.com/posts`

- Phương thức: `GET`

- Kết quả trả về:  
  ![image](https://github.com/user-attachments/assets/ac954892-ef61-4527-aede-ff192d0c4e9f)


- Mục đích:  
  `GET` là phương thức phổ biến nhất để truy xuất dữ liệu.  
  Cho phép client (web, mobile, tester...) lấy thông tin từ server mà không làm thay đổi dữ liệu.  
  Dùng để:
  - Hiển thị danh sách bài viết
  - Đối chiếu sau khi cập nhật/xoá
  - Hiểu cấu trúc và tình trạng dữ liệu ban đầu

---

### 2. Tạo bài viết mới (POST)

- URL:  
  `https://jsonplaceholder.typicode.com/posts`

- Phương thức: `POST`

- Kết quả trả về:  
 ![image](https://github.com/user-attachments/assets/712ccd29-96c1-4b25-a791-8378d20b0da4)


- Mục đích:  
  `POST` được dùng để gửi dữ liệu mới lên server.  
  Dùng khi:
  - Tạo bài viết mới
  - Gửi biểu mẫu
  - Tạo tài khoản,...

---

### 3. Ghi đè toàn bộ bài viết (PUT)

- URL:  
  `https://jsonplaceholder.typicode.com/posts/1`

- Phương thức: `PUT`

- Kết quả trả về:  
  ![image](https://github.com/user-attachments/assets/25db7645-4985-47ee-8a96-581e7f9c198b)


- Mục đích:  
  `PUT` dùng để cập nhật toàn bộ một đối tượng.  
  - Ghi đè toàn bộ tài nguyên hiện tại.
  - Phải truyền đầy đủ tất cả các trường, kể cả không thay đổi.

---

### 4. Sửa một phần bài viết (PATCH)

- URL:  
  `https://jsonplaceholder.typicode.com/posts/1`

- Phương thức: `PATCH`

- Kết quả trả về:  
  ![image](https://github.com/user-attachments/assets/51419383-68b3-4a38-b243-c1e3964681be)


- Mục đích:  
  `PATCH` được dùng để cập nhật từng phần của một đối tượng.  
  - Không ghi đè toàn bộ như `PUT`
  - Tối ưu băng thông
  - Thể hiện rõ ý định cập nhật một phần

---

### 5. Xoá bài viết (DELETE)

- URL:  
  `https://jsonplaceholder.typicode.com/posts/1`

- Phương thức: `DELETE`

- Kết quả trả về:  
 ![image](https://github.com/user-attachments/assets/8057cf34-62cf-4fd8-9be5-7ee682577207)


- Mục đích:  
  `DELETE` dùng để xoá tài nguyên khỏi server.  
  Thường dùng để:
  - Xoá bài viết
  - Huỷ đơn hàng
  - Xoá tài khoản,...
---
###Tổng kết kết quả

| Kỹ năng                 | Trạng thái           |
|------------------------|----------------------|
| Gửi yêu cầu CRUD       | Hoàn thành           |
| Viết test kiểm tra     | Có kiểm thử          |
| Hiểu phản hồi API      | Đã phân tích         |

