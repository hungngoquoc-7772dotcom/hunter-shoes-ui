# Báo cáo kiểm thử

Chrome tự động trên file local, ngày 03/11/2026.

| Viewport | Buổi 1 scrollWidth | Buổi 2 scrollWidth | Cột Buổi 2 | Ảnh |
|---|---:|---:|---:|---|
| 1366px | 1366 | 1366 | 4 | 4/4 tải được |
| 768px | 1172 | 768 | 2 | 4/4 tải được |
| 390px | 1172 | 390 | 1 | 4/4 tải được |

Lỗi: thẻ cố định 276px và flex-shrink:0 khiến hàng 4 thẻ rộng hơn màn hình. Sửa: Grid minmax và breakpoint 4/2/1 cột.
Ảnh trước tỷ lệ 1,72; sau tỷ lệ4:3 với object-fit:contain.
Tại390px: chọn size39 thành công, details mở, liên kết đến #size-guide đúng.
Hover/focus có CSS; ảnh size-focus ghi lại kiểm tra tự động. Chưa kiểm tra toàn bộ hành trình bàn phím hoặc trình đọc màn hình. Nút mua vô hiệu hóa vì bản tĩnh chưa có đặt hàng.
Xem evidence/results.json để đối chiếu phép đo. Bước 8 đã bổ sung chỉnh sửa có Codex hỗ trợ: ô size36×36px →44×44px. Chạy lại1366/768/390/320px, scrollWidth bằng viewport, tất cả28 ô size nằm trong thẻ; Space/ArrowRight/Tab hoạt động. Không khẳng định sinh viên tự làm không có AI.
