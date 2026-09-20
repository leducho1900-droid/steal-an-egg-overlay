STEAL AN EGG OVERLAY V5.28 — LUMINOUS EGGS X100–X1000

ĐÃ THÊM:
- Riêng Luminous Eggs có nút X100, X200, X300 ... X1000 trong Control.
- Bấm X nào thì chữ trên thẻ Luminous Eggs đổi qua X đó.
- Không đổi tiền / không có $/s cho Luminous Eggs.
- Không đụng 10 ảnh card V5.27, pet, nền, aura, bố cục.
- Giữ full hiệu ứng và tiền tự tạo $/s của các pet khác.
- Luminous Cthulhu base vẫn = $13B/s.

QUAN TRỌNG:
Lần này có thêm dữ liệu mới eggMult nên cần thay code Worker 1 lần.
D1 database/binding DB giữ nguyên, không cần tạo lại.

BƯỚC 1 — UPDATE WORKER:
1. Vào Cloudflare -> Worker:
   steal-an-egg-overlay-backend
2. Bấm Edit code.
3. Mở file CLOUDFLARE_WORKER_V5_28.js trong ZIP.
4. Copy toàn bộ code -> dán đè code Worker cũ.
5. Save and Deploy.
6. Test:
   https://steal-an-egg-overlay-backend.leducho1900.workers.dev/
   Nếu đúng sẽ thấy:
   "Steal An Egg Overlay Backend V5.28"

BƯỚC 2 — UPDATE GITHUB:
1. Giải nén ZIP.
2. Vào WEB_UPLOAD.
3. Copy toàn bộ file + cards + pet_layers + pet_masks + aura_masks.
4. Ghi đè repo steal-an-egg-overlay.
5. GitHub Desktop -> Commit to main -> Push origin.
6. Chờ 30–90 giây.
7. Dùng link ?v=528 để bỏ cache.

CONTROL:
https://leducho1900-droid.github.io/steal-an-egg-overlay/control.html?v=528

OVERLAY:
https://leducho1900-droid.github.io/steal-an-egg-overlay/index.html?v=528
