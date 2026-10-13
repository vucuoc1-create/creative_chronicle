# AI Prompt Log - CreativeChronicle Project

1. **Tra cứu cú pháp CSS Grid Mosaic Gallery:**
   - *Prompt:* "Làm sao để tạo layout mosaic gồm 1 ảnh lớn bên trái chiếm 2 hàng và 2 ảnh nhỏ bên phải bằng CSS Grid mà không cần gán chiều cao tuyệt đối?"
   - *Kết quả học được:* Sử dụng `grid-template-columns: 2fr 1fr;` kết hợp thuộc tính `grid-row: span 2` cho ô ảnh chính để tự động chiếm trọn không gian theo chiều dọc.

2. **Tra cứu khoảng cách và tiện ích Bootstrap Responsive Grid:**
   - *Prompt:* "Các class của Bootstrap 5 nào dùng để cấu hình lưới 4 cột trên desktop, 2 cột trên tablet và 1 cột trên mobile, kèm khoảng cách đều giữa các thẻ card?"
   - *Kết quả học được:* Sử dụng tổ hợp class `<div class="row g-4">` chứa các thẻ con `<div class="col-12 col-md-6 col-lg-3">` kết hợp class tiện ích khoảng cách `gap-2` hoặc `d-flex`.
