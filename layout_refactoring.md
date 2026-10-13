# Báo cáo Phân tích Kỹ thuật Layout: Từ Legacy đến Modern CSS

## Tác hại của `position: absolute` đối với Responsive Design
- **Mất Document Flow (Dòng chảy tài liệu):** Khi gán `position: absolute`, phần tử bị nhấc bổng ra khỏi cấu trúc cây DOM tự nhiên, khiến phần tử cha trực tiếp không thể tính toán được chiều cao (`height: 0` hoặc collapse). 
- **Hệ quả trên Mobile:** Các lớp nội dung bên dưới (như đoạn văn bản bài viết) sẽ tràn lên và bị che lấp hoàn toàn bởi các khối tuyệt đối, gây vỡ giao diện trầm trọng trên thiết bị màn hình nhỏ.

## Lý do CSS Grid là giải pháp cứu cánh
- CSS Grid cho phép định nghĩa cấu trúc 2 chiều (2D - cả hàng lẫn cột) cực kỳ trực quan thông qua `grid-template-columns` và `grid-template-rows`.
- Thay vì tính toán pixel thủ công hay dùng tọa độ tuyệt đối, Grid tự động phân bổ không gian, kết hợp linh hoạt với Media Queries để co giãn mượt mà hoặc chuyển đổi từ dạng nhiều cột sang xếp chồng dọc 1 cột trên mobile mà vẫn bảo toàn hoàn hảo chiều cao và luồng nội dung.
