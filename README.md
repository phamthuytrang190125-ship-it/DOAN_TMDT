
# WEBSITE CHO THUÊ VÁY CƯỚI

## 1. Giới thiệu

Đây là đồ án môn Thương mại điện tử với đề tài "Xây dựng website cho thuê váy cưới".

Website được xây dựng nhằm hỗ trợ khách hàng xem thông tin váy cưới, đặt thuê và thanh toán trực tuyến. Bên cạnh đó, hệ thống còn hỗ trợ quản trị viên quản lý đơn thuê, kiểm tra lịch thuê và xử lý việc hoàn tiền đặt cọc.

Một số chức năng chính của hệ thống:
- Quản lý thông tin váy cưới.
- Đặt thuê váy cưới trực tuyến.
- Quản lý đơn thuê với 5 trạng thái.
- Kiểm tra và xử lý trường hợp trùng lịch thuê.
- Quản lý tiền đặt cọc và quyết toán hoàn cọc.
- Tích hợp thanh toán VNPay Sandbox.

## 2. Công nghệ sử dụng

- Frontend: HTML, CSS, JavaScript, Bootstrap.
- Backend: Python (FastAPI).
- Cơ sở dữ liệu: PostgreSQL.
- Thanh toán: VNPay Sandbox.

## 3. Yêu cầu cài đặt

Để chạy được dự án, máy tính cần cài đặt:

- Python 3.9 trở lên.
- PostgreSQL.
- Visual Studio Code.
- Extension Live Server trên VS Code.
- Trình duyệt web.

## 4. Hướng dẫn cài đặt và chạy dự án

### Bước 1: Tạo cơ sở dữ liệu

1. Mở PostgreSQL hoặc pgAdmin.
2. Tạo database mới có tên `vaycuoi_db`.
3. Mở file `vaycuoi.sql` trong thư mục dự án.
4. Chạy file SQL để tạo các bảng và thêm dữ liệu mẫu.

### Bước 2: Chạy Backend

Mở Terminal trong Visual Studio Code.

Di chuyển vào thư mục backend:

```bash
cd backend
```

Kích hoạt môi trường ảo:

Đối với Windows:

```bash
.\venv\Scripts\activate
```

Đối với macOS/Linux:

```bash
source venv/bin/activate
```

Sau đó chạy lệnh:

```bash
uvicorn main:app --reload
```

Sau khi chạy thành công, backend hoạt động tại:

http://127.0.0.1:8000

Có thể kiểm tra các API tại:

http://127.0.0.1:8000/docs

### Bước 3: Chạy Frontend

1. Mở thư mục `frontend` bằng Visual Studio Code.
2. Cài đặt extension Live Server nếu chưa có.
3. Mở file `index.html`.
4. Nhấn chuột phải và chọn `Open with Live Server`.

Website sẽ được mở trên trình duyệt tại địa chỉ:

http://127.0.0.1:5500

Lưu ý: Cần chạy backend và kết nối cơ sở dữ liệu trước khi sử dụng các chức năng của website.

## 5. Tài khoản kiểm thử

Tài khoản quản trị viên dùng để kiểm tra các chức năng duyệt đơn và quyết toán:

- Tên đăng nhập: `admin@shop.com`
- Mật khẩu: `AdminVayCuoi@2026`

Tài khoản này chỉ được sử dụng để kiểm thử trong môi trường demo.

## 6. Ghi chú

- Dự án được thực hiện phục vụ cho đồ án môn Thương mại điện tử.
- Hệ thống sử dụng VNPay Sandbox để mô phỏng quá trình thanh toán, không sử dụng tiền thật.
- Dữ liệu được lưu trữ trong PostgreSQL.
- Cần khởi động backend và frontend để website hoạt động đầy đủ.
