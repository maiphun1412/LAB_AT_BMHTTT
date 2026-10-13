# LAB 1 – BẮT GÓI TIN TELNET VÀ SSH BẰNG WIRESHARK

## 1. Mục tiêu
- Tìm hiểu cách hoạt động của giao thức Telnet và SSH.
- Sử dụng Wireshark để bắt và phân tích gói tin.
- So sánh mức độ bảo mật giữa Telnet và SSH.

## 2. Môi trường thực hành
- **Phần mềm máy ảo:** VMware Workstation Pro.
- **Windows 11:** Máy Client, sử dụng PuTTY và Wireshark.
- **Ubuntu Linux:** Máy Server, cấu hình dịch vụ Telnet và SSH.
- **Mạng:** Host-only, kết hợp NAT để cài đặt phần mềm.

## 3. Nội dung thực hiện
- Thiết lập mạng và kiểm tra kết nối giữa hai máy ảo.
- Cài đặt và cấu hình Telnet Server trên Ubuntu.
- Sử dụng PuTTY để kết nối từ Windows đến Ubuntu.
- Bắt và phân tích lưu lượng Telnet, SSH bằng Wireshark.
- Tìm hiểu phương thức xác thực SSH bằng Public Key.

## 4. Kết quả
- Thiết lập được môi trường thực hành trên VMware.
- Sử dụng Wireshark để quan sát các gói tin truyền qua mạng.
- Nhận thấy Telnet không mã hóa dữ liệu truyền, trong khi SSH bảo vệ nội dung phiên bằng mã hóa.
- Hiểu rõ hơn sự khác biệt về bảo mật giữa hai giao thức.

## 5. Kết luận
Qua bài thực hành, em hiểu được cách sử dụng Wireshark để phân tích lưu lượng mạng và nhận thấy SSH an toàn hơn Telnet khi sử dụng để quản trị hệ thống từ xa.
