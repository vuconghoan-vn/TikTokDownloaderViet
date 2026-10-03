# Downloader TIKTOK DOUYIN — bản web

Tải `Manzovu-Web.zip` và giải nén toàn bộ gói vào thư mục riêng ngoài public_html. Gói gồm mã nguồn, bản dịch tiếng Việt, logo và giao diện.

## Cài đặt

1. Dùng Python 3.12, cài `pip install -r requirements.txt`.
2. Tạo ứng dụng WSGI: gốc `webapp`, tệp `passenger_wsgi.py`, đối tượng `application`.
3. Thư mục `webapp/jobs` cần quyền ghi; không công khai dữ liệu trong thư mục này.
4. Thay mã AdSense trong `webapp/public/index.html` và `ads.txt` nếu dùng tài khoản khác.

## Tình trạng

Đã tải được video TikTok thử trên máy Windows, dung lượng 3.507.539 byte. Chưa xác nhận chạy trên manzovu.com: ngày 01/10/2026 hosting Tenten báo 503, thiếu `/opt/alt/python312/bin/lswsgi`; đổi phiên bản bị khóa. Cần sửa môi trường máy chủ.

Bản web ban đầu hỗ trợ tải liên kết video/ảnh; chưa chuyển toàn bộ tính năng desktop. Trước khi vận hành công khai cần giới hạn yêu cầu, dọn tệp hết hạn và kiểm thử Linux. AdSense cần Google phê duyệt.

## Giấy phép

Dựa trên https://github.com/JoeanAmier/TikTokDownloader, GPL-3.0. Giấy phép có trong gói. Gói không chứa cookie, mật khẩu, dữ liệu tải hoặc nhật ký cá nhân.
