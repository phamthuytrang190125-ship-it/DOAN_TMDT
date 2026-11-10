ĐỒ ÁN MÔN THƯƠNG MẠI ĐIỆN TỬ: WEBSITE CHO THUÊ VÁY CƯỚI
1. Giới thiệu
Đây là mã nguồn hệ thống Website Thương mại điện tử Cho thuê váy cưới.
Hệ thống bao gồm các chức năng cốt lõi: Quản lý vòng đời đơn hàng khép kín (5 trạng thái), thuật toán chống trùng lịch thuê, quyết toán hoàn cọc minh bạch và tích hợp thanh toán VNPay Sandbox.

Frontend: HTML, CSS, JavaScript (Bootstrap).

Backend: FastAPI (Python).

Database: PostgreSQL.

2. Yêu cầu hệ thống
Python 3.9+

PostgreSQL

Trình duyệt web và Visual Studio Code (Live Server)

3. Hướng dẫn cài đặt và chạy dự án
Bước 1: Khởi tạo Cơ sở dữ liệu (Database)
Mở PostgreSQL (hoặc pgAdmin/Postgres.app).

Tạo một Database mới (ví dụ: vaycuoi_db).

Chạy file vaycuoi.sql có sẵn trong thư mục gốc để tạo các bảng (Users, Dresses, RentalOrders...) và import dữ liệu mẫu.

Bước 2: Chạy hệ thống Backend (FastAPI)
Mở Terminal, di chuyển vào thư mục backend:
```bash
cd backend
```

Kích hoạt môi trường ảo (venv):

Trên Windows:
```bash
.\venv\Scripts\activate
```

Trên macOS / Linux:
```bash
source venv/bin/activate
```

Khởi động server Backend:
```bash
uvicorn main:app --reload
```
Server backend sẽ chạy tại địa chỉ: `http://127.0.0.1:8000`Tài liệu API (Swagger UI): `http://127.0.0.1:8000/docs`

Bước 3: Chạy hệ thống Frontend
Mở thư mục frontend bằng phần mềm Visual Studio Code.

Cài đặt tiện ích Live Server.

Chuột phải vào file index.html -> chọn Open with Live Server.Giao diện web sẽ tự động mở lên tại `http://127.0.0.1:5500`.

4. Tài khoản test Demo
Sử dụng tài khoản Quản trị viên (Admin) sau để test các tính năng duyệt đơn và quyết toán:

Tên đăng nhập: admin@shop.com

Mật khẩu: AdminVayCuoi@2026
