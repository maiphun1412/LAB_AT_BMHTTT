# LAB 1 – Bắt gói tin Telnet và SSH bằng Wireshark

## Mục tiêu
Thực hành kết nối từ xa bằng Telnet (TCP/23) và SSH (TCP/22), sử dụng Wireshark để quan sát lưu lượng và so sánh mức độ bảo mật giữa hai giao thức.

## Môi trường
- **VMware Workstation:** 2 máy ảo trong mạng nội bộ Host-only.
- **Windows 11 (Client):** `192.168.110.128` – PuTTY, Wireshark 4.6.8, Npcap.
- **Ubuntu (Server):** `192.168.110.129` – `inetutils-telnetd`, OpenSSH Server; dùng thêm NAT để cài gói.
- **Tài khoản thực hành:** `uitlab` (không công khai mật khẩu).

## Nội dung và kết quả hiện tại
1. Đã thiết lập mạng; Windows 11 ping Ubuntu thành công, Ubuntu truy cập Internet được.
2. Đã cài Telnet Server; xác nhận cổng **23** ở trạng thái `LISTEN`. Wireshark đã ghi nhận lưu lượng TCP/23, nhưng phiên Telnet trong PuTTY còn bị màn hình đen, **chưa hoàn thành phân tích thông tin đăng nhập**.
3. Đã cài OpenSSH Server; xác nhận cổng **22** ở trạng thái `LISTEN` và kiểm tra SSH host-key fingerprint. Phần đăng nhập, bắt gói SSH và demo xác thực bằng public key **chưa có bằng chứng hoàn tất**.

## Công việc còn lại
- Hoàn tất đăng nhập Telnet, bắt và phân tích TCP Stream; thử lại với mật khẩu phức tạp.
- Hoàn tất đăng nhập SSH, bắt gói Wireshark và demo SSH public-key authentication.
- Bổ sung ảnh thực hành, file `.pcapng`, báo cáo Word trả lời 11 câu hỏi và liên kết video demo.

## Lưu ý
Toàn bộ thao tác Client/Server được thực hiện trong máy ảo. Không đưa mật khẩu thật, khóa SSH riêng tư hoặc dữ liệu nhạy cảm lên repository công khai.
