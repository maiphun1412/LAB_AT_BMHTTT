# LAB 3 - NHẬN DIỆN VÀ ỨNG PHÓ CÁC MỐI ĐE DỌA ĐẾN AN TOÀN THÔNG TIN

## 1. Thông tin sinh viên

- **Họ và tên:** Nguyễn Thị Phương Mai
- **MSSV:** 1150080146
- **Tên lab:** LAB 3 - Nhận diện và ứng phó các mối đe dọa đến an toàn thông tin

## 2. Phiên bản môi trường thực hành

- **VMware Workstation Pro:** 26H1u1
- **Máy ảo:** Windows 11 25H2 x64
- **OS Build yêu cầu:** 26200.9445 (KB5124008)
- **Network Adapter:** Host-only
- **CPU:** 2 vCPU
- **RAM:** 6 GB
- **Ổ đĩa:** 64 GB
- **Microsoft Defender Antivirus:** tích hợp Windows 11, giữ bật Real-time Protection và Tamper Protection
- **Windows PowerShell:** 5.1
- **Sysmon:** 15.22
- **Autoruns:** 14.3
- **Process Explorer:** 17.14
- **Wireshark:** 4.6.8 + Npcap
- **Python:** 3.14.7

## 3. Cách dựng môi trường

1. Cài đặt VMware Workstation Pro 26H1u1.
2. Tạo máy ảo Windows 11 25H2 x64.
3. Cấu hình máy ảo:
   - 2 vCPU
   - 6 GB RAM
   - 64 GB ổ đĩa
   - Network Adapter: Host-only
4. Cài Windows 11 và cập nhật đúng phiên bản theo yêu cầu của bài lab.
5. Tạo snapshot sạch trước khi thực hành.
6. Tạo thư mục làm việc:
   - `C:\LAB3\Evidence`
   - `C:\LAB3\Tools`
   - `C:\LAB3\Downloads`
   - `C:\LAB3\Assets`
7. Sao chép và kiểm tra SHA-256 của `LAB3_Threats_Assets.zip`.
8. Cài đặt Python 3.14.7, Wireshark 4.6.8 và Npcap.
9. Tải bộ Sysinternals chính thức gồm Sysmon, Autoruns và Process Explorer.
10. Thu baseline hệ thống trước khi tạo các tình huống thực hành.

## 4. Các tình huống đã thực hiện

| Tình huống | Nội dung | Kết quả |
|---|---|---|
| TH1 | Xác định Asset, Vulnerability, Threat, Risk và lập Risk Register | Chưa cập nhật |
| TH2 | Kiểm chứng Microsoft Defender bằng EICAR | Chưa cập nhật |
| TH3 | Tấn công mật khẩu và nguy cơ keylogging; kiểm tra Event ID 4624/4625/4648 | Chưa cập nhật |
| TH4 | Nhận diện persistence và dịch vụ lắng nghe bằng Sysmon, Autoruns, Process Explorer | Chưa cập nhật |
| TH5 | Quan sát HTTP và HTTPS bằng Wireshark; phân tích Sniffing/MITM/Spoofing | Chưa cập nhật |
| TH6 | Mô phỏng tải cục bộ, phân tích DDoS dataset và Mail Bombing log | Chưa cập nhật |
| TH7 | Phân tích Social Engineering, Phishing và Spear Phishing | Chưa cập nhật |
| Cleanup | Xóa artefact LAB3, kiểm tra lại hệ thống và tạo SHA-256 cho Evidence | Chưa cập nhật |


### Điều kiện hoàn thành

- Thu thập đủ bằng chứng theo yêu cầu.
- Defender và Tamper Protection vẫn hoạt động.
- Không tạo traffic gây tải ra ngoài phạm vi localhost.
- Không thực hiện DDoS, spoofing hoặc MITM chủ động trên mạng bên ngoài VM lab.
- Các artefact thử nghiệm được loại bỏ sau khi hoàn thành.
- File Evidence được tính SHA-256 và lưu vào `evidence_sha256.csv`.



## . Bằng chứng cần lưu

Các ảnh và log được lưu trong thư mục `LAB3/` và `C:\LAB3\Evidence`.

Một số ảnh chính:

- `H1_VM_WindowsVersion.png`
- `H2_ToolVersions.png`
- `H3_Baseline_Defender_Firewall.png`
- `H4_ProtectionHistory_EICAR.png`
- `H5_Event4625.png`
- `H6_Sysmon_Event1.png`
- `H7_Autoruns_LAB3_Run_Demo.png`
- `H8_ProcessExplorer_Python.png`
- `H9_HTTP_Plaintext.png`
- `H10_TLS_443.png`
- `H10_Load_and_Log_Analysis.png`
- `H10_Phishing_Offline.png`
- `H11_Recovery_Verification.png`

