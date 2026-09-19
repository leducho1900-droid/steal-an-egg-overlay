STEAL AN EGG OVERLAY V5 — CLOUDFLARE SYNC

LÝ DO V4.X BỊ MẤT KẾT NỐI:
- V4.x dùng ntfy để truyền Control -> Overlay.
- Nếu ntfy bị chặn / rớt kết nối trong trình duyệt hoặc TikTok Studio, bật/tắt, tiền, mutation, x2-x10 sẽ không sang Overlay.

V5 BỎ HẲN NTFY.
V5 dùng Worker riêng:
https://steal-an-egg-overlay-backend.leducho1900.workers.dev

Worker dùng Cloudflare Cache để Control và TikTok Studio cùng máy nhận state rất nhanh.
STATE_KV là TÙY CHỌN, không bắt buộc để test.

BƯỚC 1 — TẠO WORKER
1. Vào Cloudflare Dashboard.
2. Workers & Pages -> Create -> Worker.
3. Đặt tên CHÍNH XÁC:
   steal-an-egg-overlay-backend
4. Deploy.
5. Bấm Edit code.
6. Xóa code mẫu và dán toàn bộ nội dung file:
   CLOUDFLARE_WORKER_V5.js
7. Deploy / Save and deploy.

BƯỚC 2 — TEST WORKER
Mở:
https://steal-an-egg-overlay-backend.leducho1900.workers.dev/
Nếu đúng sẽ thấy JSON có:
"Steal An Egg Overlay Backend V5"

BƯỚC 3 — UPDATE GITHUB
1. Giải nén ZIP.
2. Vào WEB_UPLOAD.
3. Copy TOÀN BỘ file + thư mục cards.
4. Dán ghi đè vào repo local steal-an-egg-overlay.
5. GitHub Desktop -> Commit to main -> Push origin.
6. Chờ GitHub Pages 30–90 giây.

BƯỚC 4 — DÙNG LINK MỚI
Control:
https://leducho1900-droid.github.io/steal-an-egg-overlay/control.html?v=50

Overlay:
https://leducho1900-droid.github.io/steal-an-egg-overlay/index.html?v=50

Trong TikTok Studio PHẢI đổi Browser Source sang link Overlay có ?v=50.

KHI HOẠT ĐỘNG:
- Control sẽ hiện: ● Đã kết nối Cloudflare / ● Đã đồng bộ Cloudflare
- Bật/tắt pet -> Overlay đổi
- Weight/Mutation -> tiền đổi
- x2/x5 -> badge đổi
- x1 -> badge biến mất
- Luminous Eggs không có badge số lượng

ROOM RIÊNG CỦA BẢN NÀY:
sae_421045db4089999b697c52d464c44d3a

TÙY CHỌN — LƯU STATE BỀN HƠN:
Có thể tạo KV Namespace và bind với tên STATE_KV sau. Không bắt buộc để test realtime trên cùng máy.
