### Chi tiết cập nhật
- Tái cấu trúc dự án
- Dưới đây là danh sách chức năng đã hoàn thiện và sẽ cập nhật
  - [x] Mở/Đóng máy chủ offline
  - [x] Tự động cập nhật 
  - [ ] Quản lý chỉ số - nhân vật, tài sản
  - [ ] Tạo tài khoản
  - [ ] Mở cổng online
### Cài đặt
```bash
clear; pkg update; pkg upgrade -y; pkg install python python-pip -y; for u in "https://github.com/lorem336/Jinro/raw/refs/heads/main/jinro.py" "https://github.com/lorem336/Jinro/raw/refs/heads/main/setup.py" "https://raw.githubusercontent.com/lorem336/Jinro/refs/heads/main/termux.txt" "https://raw.githubusercontent.com/lorem336/Jinro/refs/heads/main/config.inc.php" "https://raw.githubusercontent.com/lorem336/Jinro/refs/heads/main/httpd-ssl.conf" "https://raw.githubusercontent.com/lorem336/Jinro/refs/heads/main/httpd.conf" "https://raw.githubusercontent.com/lorem336/Jinro/refs/heads/main/.htaccess" "https://raw.githubusercontent.com/lorem336/Jinro/refs/heads/main/version.txt"; do f=$(basename "$u"); curl -sL "$u" -o "$f" & done; wait; python setup.py; wait; exit
```

### Tài nguyên
- [Tệp SQL](https://github.com/lorem336/Jinro/releases/download/v2.0.0-20251125/jinro.sql)
- [MOD APK](https://github.com/lorem336/Jinro/releases/download/v2.0.0-20251125/manhhdc.apk)

- Để biết kiến trúc cpu là gì hãy tìm kiếm google với từ khóa `tên máy cpu bit` ví dụ `s25 ultra cpu bit`
- Chọn 1 phiên bản termux phù hợp với kiến trúc cpu
  - [Termux arm64-v8a](https://github.com/termux/termux-app/releases/download/v0.118.3/termux-app_v0.118.3+github-debug_arm64-v8a.apk)
  - [Termux armeabi-v7a](https://github.com/termux/termux-app/releases/download/v0.118.3/termux-app_v0.118.3+github-debug_armeabi-v7a.apk)
  - [Termux x86](https://github.com/termux/termux-app/releases/download/v0.118.3/termux-app_v0.118.3+github-debug_x86.apk)
  - [Termux x86_64](https://github.com/termux/termux-app/releases/download/v0.118.3/termux-app_v0.118.3+github-debug_x86_64.apk)
