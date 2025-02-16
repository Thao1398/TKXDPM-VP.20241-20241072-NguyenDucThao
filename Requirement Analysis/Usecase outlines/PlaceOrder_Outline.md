###Outline Use Case - Đặt Hàng (AIMS Project)
1. Tên Use Case: Đặt Hàng (Place Order)
2. Mô tả:
Khách hàng đặt hàng, nhập thông tin giao hàng, thanh toán, theo dõi đơn, có thể hủy đơn trước khi được duyệt.

3. Luồng Chính (Basic Flow)
Xem giỏ hàng: Khách hàng kiểm tra sản phẩm đã chọn.
Cập nhật giỏ hàng: Chỉnh sửa số lượng hoặc xóa sản phẩm.
Xác nhận đơn hàng: Kiểm tra tổng giá (chưa VAT, phí ship).
Chọn phương thức giao hàng: Tiêu chuẩn hoặc giao hàng nhanh.
Tiến hành thanh toán: Nhập thông tin thẻ, gửi yêu cầu đến VNPay.
Xác nhận thanh toán: VNPay xử lý, phản hồi kết quả.
Gửi email xác nhận đơn hàng: Hệ thống thông báo thành công.
Duyệt hoặc từ chối đơn hàng: Quản trị viên xét duyệt đơn hàng.
Theo dõi đơn hàng: Khách kiểm tra trạng thái đơn hàng.
Hủy đơn hàng: Nếu chưa duyệt, khách có thể hủy và được hoàn tiền.
4. Luồng Thay Thế (Alternative Flows)
- Hết hàng: Hệ thống yêu cầu khách cập nhật giỏ hàng.
- Thanh toán thất bại: Khách thử lại hoặc đổi phương thức.
- Đơn hàng bị từ chối: Quản trị viên có thể từ chối đơn (lý do kho hết hàng, lỗi hệ thống).
- Hủy đơn hàng thành công: Hệ thống gửi yêu cầu hoàn tiền đến VNPay.
- Hoàn tiền thất bại: VNPay từ chối, hệ thống thông báo khách liên hệ hỗ trợ.
