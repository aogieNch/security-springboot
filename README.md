# Bảo mật với JWT (Access và Refresh Token) sử dụng Spring Boot và MySQL

## Mô tả
Đây là một ứng dụng Java Spring Boot triển khai bảo mật với JSON Web Token (JWT), bao gồm access token và refresh token. Ứng dụng sử dụng Gmail để gửi token xác thực tài khoản đến email của người dùng. Ứng dụng cũng sử dụng MySQL làm cơ sở dữ liệu (với cách tiếp cận code-first).

### Các Endpoint
- **POST**: `/auth/register`: Đăng ký tài khoản mới.
- **POST**: `/auth/authenticate`: Xác thực và đăng nhập vào tài khoản đã có.
- **POST**: `/auth/refresh-token`: Lấy refresh token mới.

## Cài đặt
Để chạy ứng dụng này, bạn cần cài đặt:

- Java Runtime Environment (JRE)
- MySQL

Sau khi cài đặt các phần mềm yêu cầu trên, hãy làm theo các bước sau:

1. Clone kho lưu trữ.
2. Chuyển đến thư mục dự án: `cd security`.
3. Cấu hình các thuộc tính ứng dụng (ví dụ: thông tin đăng nhập cơ sở dữ liệu, thông tin đăng nhập Gmail).
4. Build dự án maven.
5. Chạy ứng dụng: `java -jar target/security-0.1.jar`.

Ứng dụng sẽ được khởi chạy, và bạn có thể bắt đầu tương tác với các endpoint đã được liệt kê ở trên.
