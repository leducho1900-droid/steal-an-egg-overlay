STEAL AN EGG OVERLAY V5.40 — ADMIN LOGIN UNIFIED

SỬA THEO YÊU CẦU:
- Ô đăng nhập dùng chung cho key thường và key chủ Admin.
- Nhập key Admin vào trang đăng nhập sẽ tự vào trang Admin tạo key.
- Chỉ key chủ Admin mới thấy/mở phần tạo key.
- Key thường chỉ vào Control / Avatar / Overlay, không có mục Admin.
- Khi xóa key, output key mới tạo ở trên sẽ biến mất nếu đó là key bị xóa.

ADMIN OUTPUT:
- Sau khi tạo key chỉ hiện:
  + Thời hạn
  + Key
  + Nút Sao chép key
- Danh sách bên dưới vẫn có:
  + Chưa kích hoạt / Đã kích hoạt
  + Số máy
  + Nút xóa key

KHÔNG ĐỤNG:
- 10 card
- pet/nền/aura/bố cục
- tiền $/s
- X100-X1000
- Weight / Mutation / x2-x10

BẮT BUỘC UPDATE WORKER:
1. Cloudflare -> Worker `steal-an-egg-overlay-backend`
2. Edit code
3. Mở file `CLOUDFLARE_WORKER_V5_40_ADMIN_LOGIN_UNIFIED.js`
4. Copy toàn bộ -> dán đè Worker cũ
5. Save and Deploy
6. Test Worker, đúng sẽ thấy:
   Steal An Egg Overlay Backend V5.40

UPDATE GITHUB:
1. Giải nén ZIP
2. Vào WEB_UPLOAD
3. Copy toàn bộ file + folders lên repo GitHub
4. Commit to main -> Push origin
5. Chờ 30–90 giây

LINK:
https://leducho1900-droid.github.io/steal-an-egg-overlay/login.html?v=540
