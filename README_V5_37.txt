STEAL AN EGG OVERLAY V5.37 — LOGIN GATE + ADMIN ONLY

ĐÃ SỬA THEO YÊU CẦU:
- Vào web phải nhập key người dùng mới được vào.
- Key người dùng chỉ dùng:
  + Trang đầu
  + Control
  + Avatar setup
  + Overlay riêng
- Key người dùng KHÔNG vào được phần tạo key.
- Phần Admin tạo key chỉ mở khi nhập đúng ADMIN_KEY.
- State POST/điều khiển overlay cũng yêu cầu key + đúng máy.
- Mỗi key vẫn là 1 key = 1 máy = 1 room/link riêng.

KHÔNG ĐỤNG:
- 10 card
- pet/nền/aura/bố cục chính
- tiền $/s
- Luminous Eggs X100-X1000
- Weight / Mutation / x2-x10

BẮT BUỘC UPDATE WORKER:
1. Cloudflare -> Worker `steal-an-egg-overlay-backend`
2. Edit code
3. Mở file `CLOUDFLARE_WORKER_V5_37_LOGIN_GATE_ADMIN_ONLY.js`
4. Copy toàn bộ -> dán đè Worker cũ
5. Save and Deploy
6. Test Worker, đúng sẽ thấy:
   Steal An Egg Overlay Backend V5.37

NHỚ SECRET:
Cloudflare Worker -> Settings -> Variables and Secrets:
ADMIN_KEY = mật khẩu admin của bạn

UPDATE GITHUB:
1. Giải nén ZIP
2. Vào WEB_UPLOAD
3. Copy toàn bộ file + folders lên repo GitHub
4. Commit to main -> Push origin
5. Chờ 30–90 giây

LINKS:
Đăng nhập người dùng:
https://leducho1900-droid.github.io/steal-an-egg-overlay/login.html?v=537

Trang đầu sau đăng nhập:
https://leducho1900-droid.github.io/steal-an-egg-overlay/home.html?v=537

Admin tạo key:
https://leducho1900-droid.github.io/steal-an-egg-overlay/admin.html?v=537

Control:
https://leducho1900-droid.github.io/steal-an-egg-overlay/control.html?v=537

Avatar setup:
https://leducho1900-droid.github.io/steal-an-egg-overlay/avatar.html?v=537
