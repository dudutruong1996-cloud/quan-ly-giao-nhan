# Quản lý Giao Nhận (local-first)

Ứng dụng web tiếng Việt dành cho một người dùng, chạy trên trình duyệt Windows.

## Tính năng
- Tạo/sửa đơn, tìm kiếm và lọc trạng thái.
- Nhật ký thay đổi trạng thái.
- Danh sách đơn giao thất bại và lên lịch giao lại.
- Mở địa chỉ hoặc chuỗi điểm giao bằng Google Maps.
- Gợi ý thứ tự điểm gần nhất bằng tọa độ (geocoding Nominatim, cần Internet).
- Xuất CSV mở bằng Excel; sao lưu/khôi phục JSON.
- Dữ liệu nghiệp vụ lưu trong localStorage của trình duyệt, không gửi đơn hàng lên GitHub.

## Chạy
Mở `index.html` bằng Chrome hoặc Edge. Khi dùng GitHub Pages, ứng dụng cũng chạy như một website tĩnh.

## Lưu ý quan trọng
- Đây là bản MVP. Tối ưu tuyến hiện dùng thuật toán điểm gần nhất theo khoảng cách đường chim bay, không phải thời gian lái xe thực tế; chưa xét đường một chiều, kẹt xe, giờ giao hay tải trọng.
- Tìm tọa độ dùng dịch vụ Nominatim của OpenStreetMap qua Internet; cần nhập địa chỉ đầy đủ. Google Maps được mở để dẫn đường.
- Trình duyệt lưu dữ liệu cục bộ theo hồ sơ người dùng. Không xóa dữ liệu trang web nếu chưa xuất bản sao lưu. Dùng cùng một trình duyệt/thiết bị để thấy cùng dữ liệu.
- Không lưu dữ liệu khách hàng thật trong repository công khai.
- Không tự động kết nối Facebook/TikTok, không tự xác nhận thanh toán/COD.
