STEAL AN EGG OVERLAY V5.38 — LOGIN + ADMIN KEY FIX

SỬA THEO YÊU CẦU:
- Trang đăng nhập chỉ còn ô nhập key + nút Đăng nhập.
- Không còn nút Admin tạo key trên trang đăng nhập.
- Nhập sai sẽ báo: Sai key / hết hạn / đã bị xóa / khóa máy khác.
- Nhập đúng sẽ báo xong rồi tự vào Control.
- Key thường chỉ dùng Control / Avatar / Overlay, không có mục Admin.
- Trang Admin chỉ mở bằng ADMIN_KEY.

ADMIN:
- Tạo key vĩnh viễn / 7 ngày / 24 giờ.
- Sau khi tạo chỉ hiện key, thời hạn, trạng thái.
- Có nút Sao chép key.
- Có danh sách key bên dưới:
  + Chưa kích hoạt / Đã kích hoạt
  + Số máy: 0 hoặc 1
  + Thời hạn
  + Nút xóa key
- Xóa key thì key đó không dùng được nữa. Control sẽ tự văng về trang nhập key.

KHÔNG ĐỤNG:
- 10 card
- pet/nền/aura/bố cục
- tiền $/s
- X100-X1000
- Weight / Mutation / x2-x10

BẮT BUỘC UPDATE WORKER:
1. Cloudflare -> Worker `steal-an-egg-overlay-backend`
2. Edit code
3. Mở file `CLOUDFLARE_WORKER_V5_38_LOGIN_ADMIN_KEYS_FIX.js`
4. Copy toàn bộ -> dán đè Worker cũ
5. Save and Deploy
6. Test Worker, đúng sẽ thấy:
   Steal An Egg Overlay Backend V5.38

UPDATE GITHUB:
1. Giải nén ZIP
2. Vào WEB_UPLOAD
3. Copy toàn bộ file + folders lên repo GitHub
4. Commit to main -> Push origin
5. Chờ 30–90 giây

LINKS:
Đăng nhập người dùng:
https://leducho1900-droid.github.io/steal-an-egg-overlay/login.html?v=538

Admin tạo key:
https://leducho1900-droid.github.io/steal-an-egg-overlay/admin.html?v=538

Control:
https://leducho1900-droid.github.io/steal-an-egg-overlay/control.html?v=538

Avatar setup:
https://leducho1900-droid.github.io/steal-an-egg-overlay/avatar.html?v=538
