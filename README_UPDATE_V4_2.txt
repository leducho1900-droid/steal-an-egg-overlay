STEAL AN EGG OVERLAY V4.2 — REALTIME SYNC FIX

LỖI ĐÃ SỬA:
- TikTok Studio có lúc giữ / làm rớt kết nối SSE nên chỉnh Weight/Mutation xong Overlay đứng im.
- V4.2 thêm polling dự phòng mỗi ~0.7 giây.
- Control gửi state ngay + retry sau 0.25s và 0.9s.
- Weight gõ nhanh được debounce 0.12s để không spam quá nhiều request.
- Control có trạng thái: Đang gửi / Đã gửi / Mất kết nối.
- Tiền, mutation, bật/tắt, x2-x10 đều đi chung một state nên cập nhật cùng nhau.

CÁCH UPDATE:
1. Giải nén ZIP.
2. Vào WEB_UPLOAD.
3. Copy toàn bộ file + thư mục cards.
4. Dán ghi đè vào repo local steal-an-egg-overlay.
5. GitHub Desktop -> Commit to main -> Push origin.
6. Chờ GitHub Pages 30–90 giây.
7. Dùng link có ?v=42 để tránh cache.

CONTROL:
https://leducho1900-droid.github.io/steal-an-egg-overlay/control.html?v=42

OVERLAY:
https://leducho1900-droid.github.io/steal-an-egg-overlay/index.html?v=42

QUAN TRỌNG:
Trong TikTok Studio phải đổi Browser Source sang link Overlay có ?v=42.
