# LAB 4 -- KHẢO SÁT VÀ ĐÁNH GIÁ BỀ MẶT MẠNG BẰNG NMAP

## Mô tả bài Lab

LAB 4 thực hành khảo sát và đánh giá bề mặt mạng bằng công cụ Nmap trong
môi trường máy ảo cô lập.

Mục tiêu của bài thực hành là sử dụng Kali Linux làm máy quét để phát
hiện các thiết bị đang hoạt động trong mạng, xác định các cổng và dịch
vụ được mở trên máy đích Metasploitable 2.

## Môi trường thực hành

-   Oracle VirtualBox
-   Kali Linux -- máy thực hiện quét
-   Metasploitable 2 -- máy đích
-   Mạng Host-Only: `192.168.56.0/24`
-   Kali Linux: `192.168.56.101`
-   Metasploitable 2: `192.168.56.102`
-   Công cụ chính: Nmap

## Nội dung đã thực hiện

-   Kiểm tra cấu hình mạng và kết nối giữa các máy ảo.
-   Phát hiện các host đang hoạt động trong mạng bằng Nmap.
-   Khảo sát cổng TCP bằng TCP Connect Scan (`-sT`) và SYN Scan (`-sS`).
-   Thực hiện FIN, Xmas, NULL và ACK Scan để quan sát các trạng thái
    cổng.
-   Quét các cổng UDP phổ biến.
-   Nhận diện dịch vụ và phiên bản bằng `-sV`.
-   Nhận diện hệ điều hành bằng `-O`.
-   Thực hiện Aggressive Scan (`-A`) để tổng hợp thông tin.
-   Sử dụng NSE để thu thập thông tin SMB và kiểm tra MS17-010.
-   Xuất kết quả quét ra các tệp để lưu bằng chứng thực hành.

## Kết quả tổng quan

Qua quá trình khảo sát, Nmap phát hiện Metasploitable 2 có nhiều dịch vụ
đang mở như FTP, SSH, Telnet, HTTP, SMB, MySQL và PostgreSQL. Việc nhận
diện phiên bản cho thấy nhiều dịch vụ sử dụng phiên bản cũ, làm tăng bề
mặt tấn công và cần được cập nhật, giới hạn truy cập hoặc tắt khi không
cần thiết.

## Video thực hành

Video ghi lại quá trình thực hiện LAB 4:

https://youtu.be/3-Tg6aEeP68

