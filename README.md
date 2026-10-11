## 1. Khởi chạy container
Sử dụng image `nginx:alpine`, đặt tên container là `my-web` và ánh xạ cổng `8080:80`.

Lệnh thực hiện: `docker run -d -p 8080:80 --name my-web nginx:alpine`

## 2. Kiểm tra Web Server
Lệnh kiểm tra: `curl http://localhost:8080`

Kết quả mong đợi: Trả về mã HTML của trang Nginx mặc định, có dòng chữ `Welcome to nginx!`.

## 3. Dừng và xóa container
Lệnh thực hiện: `docker stop my-web && docker rm my-web`

Kết quả: Container `my-web` được dừng và xóa sau khi thử nghiệm.

## 4. Kết luận

Thực hành khởi chạy Web Server Nginx bằng Docker ở chế độ nền, ánh xạ cổng mạng, kiểm tra phản hồi HTTP bằng `curl` và dọn dẹp container sau khi hoàn thành.
