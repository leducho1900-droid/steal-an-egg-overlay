STEAL AN EGG OVERLAY V1

1) Upload TOÀN BỘ file trong thư mục WEB_UPLOAD lên GitHub Pages.
2) Mở control.html để điều khiển.
3) Dán link index.html vào Browser Source của TikTok Studio.
4) Control và Overlay đồng bộ qua ntfy topic riêng:
   sae-overlay-v1-84f0ac76e4c94fe5a3e0d8c1

Công thức:
- Weight nhập 1–1000.
- Scale = cube_root(Weight) (chuẩn hóa mốc Weight 1 = giá đang ghi trên thẻ gốc).
- Nếu Scale <= 5: SizeFactor = Scale^1.85
- Nếu Scale > 5: SizeFactor = 19.637875755794113 * (Scale/5)^1.2
- MutationFactor = 1 + tổng(multiplier - 1)
- Income = giá gốc trên thẻ × SizeFactor × MutationFactor

Mutation:
Silver x1.2
Golden x2.5
Rainbow x3.5
Bloom x1.25
Spirit Bloom x2.5
Parasite x3
Fractured x2.75

Luminous Eggs X100 giữ nguyên vì đây không phải pet có $/s trong ảnh gốc.

Ảnh gốc cards_original.png được giữ nguyên 100%. Các thẻ trong Overlay chỉ là viewBox hiển thị trực tiếp vùng tương ứng của ảnh gốc.
