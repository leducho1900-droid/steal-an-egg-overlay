STEAL AN EGG OVERLAY V5.36 — ADMIN KEYS + AVATAR OVERLAY

ĐÃ THÊM:
1) Admin web tạo key:
   - admin.html
   - Nút tạo key vĩnh viễn
   - Nút tạo key 7 ngày
   - Nút tạo key 24 giờ
   - Mỗi key tự có 1 room/link overlay riêng
   - Key khóa vào 1 máy khi người dùng đăng nhập lần đầu

2) Avatar overlay:
   - avatar.html để chọn avatar
   - Avatar nằm trong khung tròn viền trắng + nút đỏ
   - Có dấu "=" và Luminous Eggs bên phải
   - Có nút Copy Link Overlay Avatar
   - Có nút quay lại trang đầu

3) Trang đầu:
   - home.html

KHÔNG ĐỤNG:
- 10 card hiện tại
- pet/nền/aura/bố cục chính
- tiền $/s
- Luminous Eggs X100-X1000
- các chức năng Weight / Mutation / x2-x10

BẮT BUỘC UPDATE WORKER:
Vì bản này thêm key + avatar nên phải dán code Worker mới.

BƯỚC 1 — THÊM ADMIN_KEY:
1. Cloudflare -> Worker `steal-an-egg-overlay-backend`
2. Settings -> Variables and Secrets
3. Add secret:
   Name: ADMIN_KEY
   Value: mật khẩu admin bạn tự đặt
4. Save

BƯỚC 2 — UPDATE WORKER:
1. Cloudflare -> Worker `steal-an-egg-overlay-backend`
2. Edit code
3. Mở file `CLOUDFLARE_WORKER_V5_36_ADMIN_KEYS_AVATAR.js` trong ZIP
4. Copy toàn bộ code -> dán đè code cũ
5. Save and Deploy
6. Test link Worker, nếu đúng sẽ thấy:
   Steal An Egg Overlay Backend V5.36

BƯỚC 3 — UPDATE GITHUB:
1. Giải nén ZIP
2. Vào WEB_UPLOAD
3. Copy toàn bộ file + folders lên repo GitHub
4. Commit to main -> Push origin
5. Chờ 30–90 giây

LINKS:
Trang đầu:
https://leducho1900-droid.github.io/steal-an-egg-overlay/home.html?v=536

Admin tạo key:
https://leducho1900-droid.github.io/steal-an-egg-overlay/admin.html?v=536

Control:
https://leducho1900-droid.github.io/steal-an-egg-overlay/control.html?v=536

Avatar setup:
https://leducho1900-droid.github.io/steal-an-egg-overlay/avatar.html?v=536

Overlay chính:
https://leducho1900-droid.github.io/steal-an-egg-overlay/index.html?v=536

Avatar overlay:
https://leducho1900-droid.github.io/steal-an-egg-overlay/avatar_overlay.html?v=536
