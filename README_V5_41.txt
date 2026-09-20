STEAL AN EGG OVERLAY V5.41 — CLEAN ADMIN + CONTROL

SỬA THEO YÊU CẦU:
- Xóa key thì key đó biến mất luôn khỏi danh sách, không còn hiện dòng "Đã xóa".
- Nếu key mới tạo ở output bị xóa thì output đó cũng mất luôn.
- Control đã xóa nút "Trang đầu".
- Avatar setup đã xóa nút "Quay lại trang đầu", chỉ giữ nút quay lại Control.
- Chữ trạng thái xanh bỏ chữ D1: "Đã kết nối" / "Đang đồng bộ".
- Ghi chú Control đổi thành:
  Weight nhập 1–1000. Weight 1 = đúng tiền gốc; tăng Weight thì tự nhân theo đường cong size. Mutation cộng bonus theo hệ số. Weight/Mutation tự tính tiền. Đồng bộ qua Cloudflare D1, không dùng Cache API. Weight/Mutation/Bật-Tắt/x2–x10 cập nhật chung một state; x1 không hiện nhãn, Luminous Eggs không có nhãn số lượng.

KHÔNG ĐỤNG:
- 10 card
- pet/nền/aura/bố cục
- tiền $/s
- X100-X1000
- Weight / Mutation / x2-x10 logic

BẮT BUỘC UPDATE WORKER:
1. Cloudflare -> Worker `steal-an-egg-overlay-backend`
2. Edit code
3. Mở file `CLOUDFLARE_WORKER_V5_41_CLEAN_ADMIN_CONTROL.js`
4. Copy toàn bộ -> dán đè Worker cũ
5. Save and Deploy
6. Test Worker, đúng sẽ thấy:
   Steal An Egg Overlay Backend V5.41

UPDATE GITHUB:
1. Giải nén ZIP
2. Vào WEB_UPLOAD
3. Copy toàn bộ file + folders lên repo GitHub
4. Commit to main -> Push origin
5. Chờ 30–90 giây

LINK:
https://leducho1900-droid.github.io/steal-an-egg-overlay/login.html?v=541
