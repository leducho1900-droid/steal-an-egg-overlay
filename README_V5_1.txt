STEAL AN EGG OVERLAY V5.1 — D1 SYNC FIX

VÌ SAO V5 LÚC ĐƯỢC LÚC KHÔNG:
V5 cũ dùng Cloudflare Cache API để giữ state. Cache đó là local theo data center.
Control và TikTok Studio đôi lúc đi qua edge/data center khác nhau nên một bên thấy state mới,
một bên vẫn thấy state cũ. Một lúc sau route/cache thay đổi thì lại dùng được.

V5.1 BỎ HẲN CACHE API.
State được lưu trong Cloudflare D1 và Overlay dùng long-poll, nên không phải spam request 0.4 giây/lần.

BACKEND GIỮ NGUYÊN:
https://steal-an-egg-overlay-backend.leducho1900.workers.dev

ROOM GIỮ NGUYÊN:
sae_421045db4089999b697c52d464c44d3a

=== BƯỚC 1: TẠO D1 DATABASE ===
1. Cloudflare Dashboard -> tìm "D1" / "D1 SQL Database".
2. Create database.
3. Đặt tên:
   steal-an-egg-overlay-db
4. Create.

=== BƯỚC 2: GẮN D1 VÀO WORKER ===
1. Vào Worker:
   steal-an-egg-overlay-backend
2. Tab Bindings.
3. Add binding.
4. Chọn D1 database.
5. Variable name PHẢI ghi:
   DB
6. Chọn database:
   steal-an-egg-overlay-db
7. Save/Add binding.

=== BƯỚC 3: THAY CODE WORKER ===
1. Worker -> Edit code.
2. Xóa code V5 cũ.
3. Mở file CLOUDFLARE_WORKER_V5_1_D1.js trong ZIP.
4. Copy toàn bộ -> dán vào Worker.
5. Save and Deploy.

TEST:
Mở:
https://steal-an-egg-overlay-backend.leducho1900.workers.dev/
Nếu đúng phải thấy:
"Steal An Egg Overlay Backend V5.1"
và
"storage":"Cloudflare D1"

=== BƯỚC 4: UPDATE GITHUB ===
1. Vào WEB_UPLOAD trong ZIP.
2. Copy toàn bộ file + thư mục cards.
3. Ghi đè vào repo steal-an-egg-overlay.
4. GitHub Desktop -> Commit to main -> Push origin.
5. Chờ Pages 30–90 giây.

CONTROL:
https://leducho1900-droid.github.io/steal-an-egg-overlay/control.html?v=51

OVERLAY TIKTOK STUDIO:
https://leducho1900-droid.github.io/steal-an-egg-overlay/index.html?v=51

Trong TikTok Studio phải đổi Browser Source sang link ?v=51.
