# Tổng quan ứng dụng thương mại điện tử với .NET Core

## Giới thiệu chung

Video này trình bày ứng dụng cuối cùng sẽ được xây dựng trong khóa học. Đây là một ứng dụng thương mại điện tử (e-commerce application) hoàn chỉnh với nhiều tính năng phức tạp.

## Tính năng dành cho khách hàng (Customer Features)

## Trang chủ và hiển thị sản phẩm

- Hiển thị danh sách sản phẩm (products) với hình ảnh và giá cả
    
- Hiển thị số lượng sản phẩm trong giỏ hàng (shopping cart)
    
- Trang chi tiết sản phẩm với hệ thống giảm giá theo số lượng
    

## Hệ thống định giá linh hoạt

- Giá sản phẩm thay đổi theo số lượng đặt hàng
    
- Ví dụ: Đặt 51 sản phẩm sẽ có giá 85 thay vì giá gốc
    

## Xác thực và đăng ký

- Yêu cầu đăng nhập khi thêm sản phẩm vào giỏ hàng
    
- Hỗ trợ đăng ký tài khoản mới với validation tích hợp
    
- Tích hợp đăng nhập qua Facebook
    

## Giỏ hàng và thanh toán

- Thông báo toast (toaster notification) khi cập nhật giỏ hàng
    
- Hiển thị tổng tiền (grand total)
    
- Cho phép xóa sản phẩm và chỉnh sửa số lượng trực tiếp
    
- Tích hợp thanh toán qua Stripe với thẻ test 4242 4242 4242 4242
    
- Hiển thị xác nhận đơn hàng với mã đơn hàng (order ID)
    

## Quản lý đơn hàng của khách hàng

- Xem lịch sử đơn hàng
    
- Theo dõi trạng thái đơn hàng (order status)
    
- Xem thông tin vận chuyển (carrier and tracking information)
    

## Tính năng dành cho quản trị viên (Admin Features)

## Quản lý nội dung (Content Management)

- Menu quản lý nội dung chỉ hiển thị cho admin
    
- Quản lý danh mục sản phẩm (categories): tạo mới, cập nhật, xóa
    
- Quản lý sản phẩm với các tính năng CRUD (Create, Read, Update, Delete)
    

## Quản lý sản phẩm nâng cao

- Bảng dữ liệu (data table) với tính năng tìm kiếm, lọc và sắp xếp
    
- Trình soạn thảo văn bản phong phú (rich text editor) cho mô tả sản phẩm
    
- Quản lý hình ảnh sản phẩm với khả năng tải lên mới
    
- Hệ thống định giá theo từng khoảng số lượng:
    
    - Giá cho số lượng 1-50
        
    - Giá cho số lượng trên 50
        
    - Giá cho số lượng trên 100
        
- Gán danh mục cho sản phẩm thông qua dropdown
    
- Xác nhận xóa bằng Sweet Alert
    

## Quản lý người dùng

- Tạo tài khoản người dùng với các vai trò khác nhau:
    
    - Admin
        
    - Employee (nhân viên)
        
    - Company (công ty)
        
    - Customer (khách hàng)
        

## Quản lý đơn hàng

- Xem tất cả đơn hàng với trạng thái chi tiết
    
- Cập nhật trạng thái đơn hàng:
    
    - Approved (đã duyệt)
        
    - Processing (đang xử lý)
        
    - Shipped (đã gửi hàng)
        
- Nhập thông tin vận chuyển khi gửi hàng
    
- Cập nhật thông tin đơn hàng
    

## Hệ thống tài khoản công ty (Company Account System)

## Đặc điểm tài khoản công ty

- Có thể đặt hàng mà không cần thanh toán ngay lập tức
    
- Thanh toán trễ (delayed payment) - thường có 30 ngày để thanh toán sau khi hàng được gửi
    
- Khác biệt với tài khoản khách hàng cá nhân phải thanh toán ngay
    

## Quy trình tạo tài khoản công ty

1. Admin tạo công ty trong tab Company
    
2. Tạo tài khoản người dùng và gán vào công ty đã tạo
    
3. Khi đăng ký, xuất hiện dropdown để chọn công ty
    

## Quy trình đặt hàng của công ty

- Tự động điền thông tin dựa trên dữ liệu đăng ký
    
- Không yêu cầu thanh toán ngay lập tức
    
- Hiển thị trang xác nhận với mã đơn hàng
    

## Quy trình thanh toán

## Thanh toán cho khách hàng cá nhân

- Chuyển hướng đến Stripe để thanh toán
    
- Sử dụng thẻ test để kiểm tra
    
- Hiển thị Payment Intent ID khi thanh toán thành công
    

## Thanh toán cho công ty

- Trạng thái "Approved for delayed payment"
    
- Nút "Pay Now" xuất hiện sau khi đơn hàng được gửi
    
- Có thể thanh toán qua admin hoặc tự thanh toán khi đăng nhập
    

## Kết luận

Ứng dụng này bao gồm nhiều tính năng phức tạp và sẽ được trình bày chi tiết trong một khóa học dài. Học viên sẽ học được nhiều chủ đề đa dạng với .NET Core để xây dựng một ứng dụng hoàn chỉnh mà có thể tự hào về kết quả cuối cùng.