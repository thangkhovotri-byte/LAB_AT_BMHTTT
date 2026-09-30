# LAB 4: Network Scanning and Hardening

* **Họ và tên:** Nguyễn Phạm Đông Dương
* **Mã sinh viên:** 1150080047
* **Lớp:** 11_ĐH_THMT

---

## 1. Thông tin môi trường Lab
* **Máy tấn công (Attacker):** Kali Linux (`192.168.234.129`)
* **Máy nạn nhân (Victim):** Metasploitable 2 (`192.168.234.130`)
* **Kiến trúc mạng:** Sử dụng card mạng ảo chế độ **Host-Only** trên VMware Workstation.

## 2. Nội dung thực hiện
* **Phần 1: Quét mạng và thu thập thông tin (Nmap)**
  * Kiểm tra kết nối và tìm kiếm host hoạt động (`-sn`).
  * Quét cổng TCP ẩn (`-sS`).
  * Nhận diện phiên bản dịch vụ (`-sV`).
  * Nhận diện hệ điều hành (`-O`).
  * Kiểm tra lỗ hổng dịch vụ bằng NSE Script (SMB).
  * Xuất kết quả quét ra file (`ket_qua.txt`, `ket_qua.xml`).

* **Phần 2: Kịch bản Hardening (Bảo cứng hệ thống)**
  * **Before:** Ghi nhận trạng thái dịch vụ Apache đang mở (`open`) qua lệnh quét Nmap.
  * **Thực thi:** Dừng dịch vụ không cần thiết trên Metasploitable 2 (`sudo /etc/init.d/apache2 stop`).
  * **After:** Kiểm tra lại bằng Nmap để xác nhận cổng dịch vụ đã chuyển sang trạng thái đóng (`closed`).

## 3. Link minh chứng
* **Báo cáo chi tiết:** [File Word trong thư mục này]
* **Video quay quá trình thực hiện:** 
p1:   https://youtu.be/ub6Bmnwb0OM

p2:  https://youtu.be/h6ljwZ4ucPQ 

p3:   https://youtu.be/FeEhxBZPA04 
