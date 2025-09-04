# Server Ngọc Rồng Online by JINN1368

Được viết bằng Python để giúp quản lý máy chủ game Ngọc Rồng. Công cụ này cung cấp các chức năng cần thiết để vận hành, cấu hình và quản lý người chơi một cách dễ dàng.

## Tính năng chính

- **Tự động cập nhật:** Tự động kiểm tra và tải về phiên bản mới nhất.
- **Quản lý Server:**
  - Khởi động server game
  - Mở cổng ra Internet để người khác có thể kết nối thông qua **Serveo** hoặc **Ngrok**.
- **Quản lý Người chơi:**
  - Xem danh sách tất cả người chơi trong cơ sở dữ liệu.
  - Chỉnh sửa chi tiết thông tin của từng người chơi:
    - Chỉ số: Sức mạnh, tiềm năng, HP, KI, sát thương, giáp, chí mạng.
    - Nhiệm vụ: Thay đổi nhiệm vụ hiện tại.
    - Vật phẩm: Chỉnh sửa số lượng vàng, ngọc xanh, hồng ngọc.
    - Phân quyền: Cấp hoặc tước quyền Admin.
- **Quản lý Tài khoản:** Tạo tài khoản game trực tiếp từ menu.
- **Cấu hình & Tiện ích:**
  - Dễ dàng cấu hình cổng kết nối (port) cho server và các dịch vụ mở cổng.
  - Tự động tải và giải nén dữ liệu game.

## Yêu cầu

Trước khi sử dụng, bạn cần chuẩn bị:

1.  **Termux**: Menu sẽ hoạt động trên termux.
2.  **Thư viện Python:** Cài đặt các thư viện cần thiết có trong file `requirements.txt`.
3.  **Ksweb:** Một server MySQL đang hoạt động với database có tên là `jinro`.

## Cài đặt & Cấu hình

1.  **Tải Termux:**
    - [Tải xuống Termux](https://github.com/termux/termux-app/releases/tag/v0.118.3)

2.  **Cài đặt thư viện:**
    - Mở Termux hoặc và chạy lệnh sau:
      ```bash
      termux-setup-storage
      apt update
      apt upgrade -y
      pkg i -y python python-pip openjdk-17 git
      git clone https://github.com/lorem336/Jinro
      cd Jinro
      pip install -r requirements.txt
      ```

3.  **Cài đặt Ksweb:**
      - [Tải xuống Ksweb](https://download1336.mediafire.com/iaq6v3fvyu2gEpqsliNu9AVuGx2GZRNLiyesvKQIJfZt1EDiA0eSlCt_LLmShnRK2Gny6EgqHKLa2j9jrBH726T0477DNxOxChuCgGoC6N9IKiZW3IIlnQFE2VYX9c7Yhyxph7aSa4Pff8F2VfnqNkoGv-7c9QYD5j2JpFZogWM/6bvlddcp54mc9nf/KSWeb_v3.988_gocmod.com.apk)
4. **Cài đặt APK ngọc rồng mod**
      - [Tải xuống APK](https://github.com/JINN1368/NgocRongTermux/releases/download/APK/JINN_MANHHDC.apk)    
5. **Tệp SQL**
      - [Tải xuống tệp SQL](https://drive.google.com/file/d/1xRpMMcBQuHWWcUL_hKfGYajVGuHilZfC/view)
## Sử dụng

1.  **Chạy chương trình:**
    - Mở Termux và chạy lệnh:
      ```bash
      cd jinro 
      python main.py
      ```

2.  **Nhập mã kích hoạt:**
    - Chương trình sẽ yêu cầu bạn nhập mã kích hoạt. [Lấy mã tại đây](https://link4m.com/go/st5AyDnP) hoặc [Mã dự phòng](https://link2m.com/go/zC7YbaZ2).
    - Mã sẽ được reset trong vòng 7 ngày.

3.  **Sử dụng Menu:**
    - Sau khi xác thực thành công, một menu các chức năng sẽ hiện ra.
    - Nhập số tương ứng với chức năng bạn muốn sử dụng và làm theo hướng dẫn.

    - **1. Chạy Server Game:** Bắt đầu chạy server game.
    - **2. Mở cổng (Online):** Giúp đưa server của bạn ra mạng Internet.
    - **3. Quản lý Người Chơi:** Vào menu con để xem và chỉnh sửa thông tin người chơi.
    - **4. Cấu hình Cổng Kết Nối:** Thiết lập các port cho server và dịch vụ online.
    - **5. Tạo tài khoản:** Tạo một tài khoản game mới.
    - **6. Sửa dữ liệu:** Tải lại dữ liệu game.
    - **0. Thoát chương trình:** Đóng ứng dụng.
