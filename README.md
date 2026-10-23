# Demo trang Giỏ hàng — Thiết bị mầm non Việt Mỹ

Trang `/cart/` của site Việt Mỹ (THC dựng) — bản sạch, chỉ giao diện (23/10/2026). Khung header, breadcrumb,
footer, thanh liên hệ nổi lấy nguyên từ trang thật; phần giỏ sửa theo 8 ý review trong sheet
“Brief Thiết kế Website — tab Review tổng thể website” (khối Giỏ hàng, dòng 215–222):

1. Phương thức thanh toán: Tiền mặt / Chuyển khoản
2. Icon giỏ trên thẻ “Thường mua kèm” không nofollow
3. Thường mua kèm: thêm xong vẽ lại giỏ + khối tổng ngay; gợi ý theo SP bán kèm của SP trong giỏ
4. Khối tổng: Tiền hàng · Vận chuyển & lắp đặt · Tạm tính (chưa gồm VAT 10%, phí vận chuyển & lắp đặt); thành tiền từng dòng
5. Xoá sản phẩm có thông báo + Hoàn tác 5 giây
6. Mobile: Thường mua kèm xuống dưới khối tổng; bước 1 thanh tiến trình hiện số đỏ như desktop
7. Nút +/− là `<button>` có aria-label
8. Bỏ thẻ heading thừa (trang chỉ còn H1)

Mọi thao tác giỏ chạy trong trình duyệt, không gửi gì về máy chủ. Danh sách SP bán kèm là dữ liệu mẫu.
Nguồn dựng: `nguyen-lieu/2026-10-23_gio-hang-trang-build/` (`main.html` · `de-xuat.css` · `app.js`, `python3 build.py`).
