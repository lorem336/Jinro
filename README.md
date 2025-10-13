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
      pkg i -y python python-pip openjdk-17 git openssh
      git clone https://github.com/lorem336/Jinro
      cd Jinro
      pip install -r requirements.txt
      cd ..
      git clone https://github.com/Yisus7u7/termux-ngrok
      cd termux-ngrok
      bash install.sh
      cd ..
      python main.py
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
      cd Jinro 
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
## BUFF vật phẩm 
  - chat lệnh `buff` sau đó sẽ hiển thị bảng bao gồm

| Tiêu đề | Dữ liệu |
| -------- | ------- |
| Tên nhân vật  | nhập tên nhân vật   |
| ID ITEM |  nhập id vật phẩm trong bảng item_template     |
| id option    | thuộc tính    |
| param | chỉ số |
| Số lượng | số lượng |
- Danh sách ID Option

<table border="0" cellpadding="8" cellspacing="0">
    <thead>
        <tr>
            <th>ID</th>
            <th>MÔ TẢ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>0</td>
            <td>Tấn công+#</td>
        </tr>
        <tr>
            <td>1</td>
            <td>Thời gian sử dụng # phút</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Vô hiệu và biến #% sát thương chưởng thành KI</td>
        </tr>
        <tr>
            <td>4</td>
            <td>Hồi phục #% KI khi bị đánh</td>
        </tr>
        <tr>
            <td>5</td>
            <td>+#% sức đánh chí mạng</td>
        </tr>
        <tr>
            <td>6</td>
            <td>HP+#</td>
        </tr>
        <tr>
            <td>7</td>
            <td>KI+#</td>
        </tr>
        <tr>
            <td>8</td>
            <td>Hút #% HP, KI xung quanh mỗi 5 giây</td>
        </tr>
        <tr>
            <td>9</td>
            <td>Hiệu lực trong # phút</td>
        </tr>
        <tr>
            <td>14</td>
            <td>Chí mạng+#%</td>
        </tr>
        <tr>
            <td>15</td>
            <td>Phản đòn cận chiến+#</td>
        </tr>
        <tr>
            <td>19</td>
            <td>Tấn công+#% khi đánh quái</td>
        </tr>
        <tr>
            <td>23</td>
            <td>KI+#K</td>
        </tr>
        <tr>
            <td>24</td>
            <td>Làm tăng trọng lực, gây chậm mọi người xung quanh</td>
        </tr>
        <tr>
            <td>25</td>
            <td>Tàng hình mỗi 5 giây</td>
        </tr>
        <tr>
            <td>26</td>
            <td>Hóa đá mọi người xung quanh mỗi 30 giây</td>
        </tr>
        <tr>
            <td>27</td>
            <td>+# HP/30s</td>
        </tr>
        <tr>
            <td>28</td>
            <td>+# KI/30s</td>
        </tr>
        <tr>
            <td>29</td>
            <td>Biến Sôcôla mọi người xung quanh mỗi 30 giây</td>
        </tr>
        <tr>
            <td>30</td>
            <td>Không thể giao dịch</td>
        </tr>
        <tr>
            <td>38</td>
            <td>Chỉ có tác dụng khi hợp thể</td>
        </tr>
        <tr>
            <td>47</td>
            <td>Giáp+#</td>
        </tr>
        <tr>
            <td>49</td>
            <td>Tấn công+#%</td>
        </tr>
        <tr>
            <td>50</td>
            <td>Sức đánh+#%</td>
        </tr>
        <tr>
            <td>66</td>
            <td>Chưa có</td>
        </tr>
        <tr>
            <td>73</td>
            <td></td>
        </tr>
        <tr>
            <td>77</td>
            <td>HP+#%</td>
        </tr>
        <tr>
            <td>78</td>
            <td>Sức hủy diệt+#%</td>
        </tr>
        <tr>
            <td>79</td>
            <td>Đệ tử #% sức đánh</td>
        </tr>
        <tr>
            <td>93</td>
            <td>HSD # ngày</td>
        </tr>
        <tr>
            <td>94</td>
            <td>Giáp #%</td>
        </tr>
        <tr>
            <td>95</td>
            <td>Biến #% tấn công thành HP</td>
        </tr>
        <tr>
            <td>101</td>
            <td>+#% TN,SM</td>
        </tr>
        <tr>
            <td>103</td>
            <td>KI +#%</td>
        </tr>
        <tr>
            <td>104</td>
            <td>Biến #% tấn công quái thành HP</td>
        </tr>
        <tr>
            <td>105</td>
            <td>Vô hình khi không đánh quái và boss</td>
        </tr>
        <tr>
            <td>106</td>
            <td>Không ảnh hưởng bởi cái lạnh</td>
        </tr>
        <tr>
            <td>109</td>
            <td>Hôi, giảm #% HP</td>
        </tr>
        <tr>
            <td>110</td>
            <td>Dò pha lê</td>
        </tr>
        <tr>
            <td>111</td>
            <td>Phân tâm</td>
        </tr>
        <tr>
            <td>114</td>
            <td>+#% TĐ chạy</td>
        </tr>
        <tr>
            <td>116</td>
            <td>Kháng TDHS</td>
        </tr>
        <tr>
            <td>117</td>
            <td>Đẹp +#% SĐ cho mình và người xung quanh</td>
        </tr>
        <tr>
            <td>118</td>
            <td>Tới ngay mục tiêu và gây choáng trong # mili giây</td>
        </tr>
        <tr>
            <td>119</td>
            <td>Gây mù xung quanh trong # giây</td>
        </tr>
        <tr>
            <td>120</td>
            <td>Ra đòn sau # giây</td>
        </tr>
        <tr>
            <td>121</td>
            <td>Ru ngủ trong # giây</td>
        </tr>
        <tr>
            <td>122</td>
            <td>Bảo vệ trong # giây</td>
        </tr>
        <tr>
            <td>123</td>
            <td>Trói gô mục tiêu trong # giây</td>
        </tr>
        <tr>
            <td>124</td>
            <td>Tỉnh giấc bị yếu đi -#% sức đánh trong 10 giây</td>
        </tr>
        <tr>
            <td>125</td>
            <td>Tăng và hồi phục #% HP tạm thời cho mình và xung quanh trong 30 giây</td>
        </tr>
        <tr>
            <td>126</td>
            <td>Biến sôcôla làm yếu đi -#% sức đánh trong 30 giây</td>
        </tr>
        <tr>
            <td>141</td>
            <td>$(5 món 100% sát thương Kamejoko)</td>
        </tr>
        <tr>
            <td>145</td>
            <td>$(Ở gần 1 CT Dr Slum khác loại +20% sức đánh +66% tốc độ chạy)</td>
        </tr>
        <tr>
            <td>146</td>
            <td>$(Ở gần 2 CT Dr Slum khác loại +30% sức đánh +100% tốc độ chạy)</td>
        </tr>
        <tr>
            <td>150</td>
            <td>(Chỉ số tăng khi ở gần Android Sát Thủ khác loại)</td>
        </tr>
        <tr>
            <td>153</td>
            <td>#% tỉ lệ phát nổ sau khi chết</td>
        </tr>
        <tr>
            <td>162</td>
            <td>Cute hồi #% KI/s bản thân và xung quanh</td>
        </tr>
        <tr>
            <td>173</td>
            <td>Phục hồi #% HP và KI cho đồng đội</td>
        </tr>
        <tr>
            <td>192</td>
            <td>SET BASIL</td>
        </tr>
        <tr>
            <td>193</td>
            <td>$(Tăng 10%HP,KI và 20% sức đánh chí mạng khi mặc 2 món BASIL)</td>
        </tr>
        <tr>
            <td>212</td>
            <td>Thú cưỡi của người chăm chỉ</td>
        </tr>
    </tbody>
</table>
