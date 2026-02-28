# 📈 Biểu đồ Sinh viên Kỹ thuật Robot - UET
Dự án là một script Python đơn giản sử dụng `pandas` và `matplotlib` để vẽ biểu đồ đường thể hiện sự gia tăng số lượng sinh viên ngành Kỹ thuật Robot (UET) qua các khóa.
## 🚀 Công nghệ sử dụng
* **Ngôn ngữ:** Python 3.10
* **Thư viện ngoài:** pandas, matplotlib
* **Công cụ triển khai:** Docker
## 🛠️ Hướng dẫn chạy dự án bằng Docker
Vì ứng dụng chạy trong Docker không có giao diện UI, biểu đồ sẽ được xuất ra thành một file ảnh `bieu_do_robot.png`. 
Bước 1: Build Docker image
```bash
docker build -t bieu-do-robot.
Bước 2: Chạy Container và liên kết thư mục (Mount Volume)
Để có thể lấy được file ảnh từ trong Docker ra ngoài máy tính của bạn, hãy chạy lệnh sau:
+Trên Windows (Command Prompt):
  docker run -v "%cd%":/app bieu-do-robot
+Trên Mac/Linux/Windows PowerShell:
  docker run -v ${PWD}:/app bieu-do-robot
Bước 3: Xem kết quả
Mở thư mục hiện tại của dự án, bạn sẽ thấy file ảnh bieu_do_robot.png đã được tạo ra thành công!
