# Local Passport Website (Lab 6 - Project 2)

Mô tả ngắn

Đây là một ví dụ ứng dụng Node.js/Express sử dụng Passport (local strategy) để đăng ký, đăng nhập và xem profile người dùng. Dự án dùng mô hình đơn giản cho mục đích học tập.

Nội dung chính

- `app.js`: Điểm vào ứng dụng Express.
- `config/passport.js`: Cấu hình Passport local strategy.
- `models/User.js`: Mô hình người dùng (mongoose schema).
- `routes/auth.js`: Router cho đăng ký / đăng nhập / đăng xuất.
- `views/`: Các view EJS (`login.ejs`, `register.ejs`, `profile.ejs`).

Yêu cầu

- Node.js >= 14
- MongoDB (chạy local hoặc Atlas)

Cài đặt

1. Clone repo

   git clone <repo-url>

2. Cài đặt phụ thuộc

   npm install

3. Cấu hình biến môi trường (ví dụ dùng `.env`)

   - `MONGO_URI`: chuỗi kết nối MongoDB
   - `SESSION_SECRET`: chuỗi bí mật cho session

4. Chạy ứng dụng

   npm start

Hoạt động

- Truy cập `http://localhost:3000/register` để tạo tài khoản.
- Truy cập `http://localhost:3000/login` để đăng nhập.
- Sau khi đăng nhập, truy cập `http://localhost:3000/profile` để xem thông tin.

Ghi chú

- Đây là ví dụ đơn giản, không dùng xác thực email, không mã hóa nâng cao ngoài bcrypt (nếu đã cài), và không dùng HTTPS mặc định.

Mở rộng (gợi ý)

- Thêm xác thực email và xác minh tài khoản.
- Thêm bảo mật (helmet, rate-limiter).
- Triển khai OAuth (Google, Facebook).

Liên hệ

- Tác giả: peoPeoo2202
- Repo: LTHDV_lab6_p2
