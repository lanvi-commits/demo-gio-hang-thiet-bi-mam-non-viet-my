# Demo trang Giỏ hàng — Thiết bị mầm non Việt Mỹ

Mockup v2 (23/10/2026) trang `/cart/` của site Việt Mỹ do THC dựng, áp 8 ý review trong sheet
“Brief Thiết kế Website — tab Review tổng thể website” (khối Giỏ hàng, dòng 215–222):

1. Phương thức thanh toán: Tiền mặt / Chuyển khoản
2. Bỏ nofollow ở icon giỏ (gốc lỗi: `external-links.js` coi link tương đối là link ngoài)
3. Thường mua kèm: thêm xong vẽ lại giỏ + khối tổng; gợi ý theo SP bán kèm
4. Khối tổng: Tiền hàng · Vận chuyển & lắp đặt · Tạm tính (chưa gồm VAT, phí)
5. Xoá sản phẩm có toast Hoàn tác 5 giây
6. Mobile: Thường mua kèm xuống dưới khối tổng; bước 1 hiện số đỏ như desktop
7. Nút +/− là `<button>` có aria-label
8. Bỏ thẻ heading thừa (chỉ còn H1)

Công tắc **Hiện tại (live) ↔ Đề xuất**, khung Desktop / Mobile 390, “Soi nofollow + heading”.
1 file `index.html` tự chứa (CSS, font, ảnh nhúng base64), không gửi dữ liệu đi đâu.
Nguồn dựng: `nguyen-lieu/2026-10-23_gio-hang-tong-tien-build/` (`src.html` + `python3 build.py`).
