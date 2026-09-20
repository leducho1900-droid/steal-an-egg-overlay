STEAL AN EGG OVERLAY V5.39 — LOGIN FIX

SỬA LỖI:
- Bấm Đăng nhập không phản hồi.
- Không báo đúng/sai key.
- Không tự chuyển vào Control.

V5.39 sửa:
- Login dùng JS an toàn hơn, không phụ thuộc global id.
- Có backend fallback nếu config.js chưa tải.
- Nhập đúng báo "Key đúng" rồi tự vào Control.
- Nhập sai báo lỗi rõ.
- Nếu Worker chưa update sẽ báo Worker chưa có /auth.
- Không đụng card / pet / aura / tiền / X100-X1000.

BẮT BUỘC:
Nếu bạn chưa update Worker V5.38 thì dán Worker V5.39 mới:
CLOUDFLARE_WORKER_V5_39_LOGIN_FIX.js

UPDATE:
1. Giải nén ZIP
2. Up toàn bộ WEB_UPLOAD lên GitHub
3. Nếu chưa update Worker thì update Worker bằng file V5.39
4. Dùng link mới ?v=539 để tránh cache.

LINK ĐĂNG NHẬP:
https://leducho1900-droid.github.io/steal-an-egg-overlay/login.html?v=539

ADMIN:
https://leducho1900-droid.github.io/steal-an-egg-overlay/admin.html?v=539

CONTROL:
https://leducho1900-droid.github.io/steal-an-egg-overlay/control.html?v=539
