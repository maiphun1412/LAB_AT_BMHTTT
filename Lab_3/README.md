# LAB 3 – NHẬN DIỆN VÀ ỨNG PHÓ CÁC MỐI ĐE DỌA ĐẾN AN TOÀN THÔNG TIN

## 1. Thông tin sinh viên

- **Họ và tên:** Nguyễn Thị Phương Mai
- **MSSV:** 1150080146
- **Tên bài:** LAB 3 – Nhận diện và ứng phó các mối đe dọa đến an toàn thông tin

## 2. Môi trường thực hành

Bài lab được thực hiện trên máy ảo Windows 11 bằng VMware Workstation.

| Thành phần | Cấu hình thực tế |
|---|---|
| Hệ điều hành | Windows 11 Pro 25H2, Build 26200.8037 |
| CPU / RAM / Ổ đĩa | 2 vCPU / 6 GB / 64 GB |
| Mạng | Host-only |
| Python | 3.14.7 |
| Wireshark | 4.6.8 |
| Sysmon | 15.22 |
| Autoruns | 14.3 |
| Process Explorer | 17.14 |

Microsoft Defender, Real-time Protection, Tamper Protection và ba profile Windows Firewall đều được xác nhận đang bật.

## 3. Nội dung đã thực hiện

| Nội dung | Kết quả |
|---|---|
| Chuẩn bị môi trường | Đã cấu hình máy ảo, cài đặt và kiểm tra công cụ |
| Snapshot | Đã tạo `LAB3_BASELINE_20261012` |
| Baseline | Đã thực hiện các lệnh thu thập thông tin hệ thống, Defender, Firewall và tiến trình |
| TH1 – Asset, Vulnerability, Threat, Risk | Đã xây dựng bảng phân tích rủi ro để đưa vào báo cáo |
| TH2 – Microsoft Defender và EICAR | Đã thực hiện bước thử nghiệm, chưa xác nhận đầy đủ bằng chứng Protection History |
| TH3 – Mật khẩu và Event Log | Đã tạo tài khoản `lab3user`, kiểm tra dịch vụ Secondary Logon và đổi mật khẩu. `runas` gặp lỗi, chưa thu được log xác thực phù hợp |
| TH4 – Sysmon và Persistence | Đã tìm được file cấu hình `sysmon-lab.xml` và chuẩn bị thực hiện các bước cấu hình, kiểm tra |
 
## 4. Kết quả và ghi nhận

- Máy ảo Windows 11 hoạt động, các công cụ cần thiết đã được cài đặt.
- Microsoft Defender và Windows Firewall vẫn bật trong quá trình thực hành.
- Đã kiểm tra tài khoản `lab3user` tồn tại và hoạt động.
- Lệnh `runas` báo `Unable to acquire user password`; file `auth_events_before_rotation.txt` chưa có dữ liệu phù hợp.
- Đã xác định được đường dẫn cấu hình Sysmon tại `C:\LAB3\LAB3_Threats_Assets\lab3_assets\sysmon-lab.xml`.
- Đã thực hiện sao lưu và reset các artefact thử nghiệm LAB3 để chuẩn bị quay lại video.


