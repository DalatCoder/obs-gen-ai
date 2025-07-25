# Kiến trúc MVC trong ASP.NET Core

## Giới thiệu về MVC

Khi mở Solution Explorer và xem file Program.cs, bạn sẽ thấy trong phần routing (định tuyến) có các từ khóa quan trọng là **controller** và **action**.

Trong Solution Explorer, chúng ta có các thư mục:

- **Controllers** (Bộ điều khiển)
    
- **Models** (Mô hình)
    
- **Views** (Giao diện)
    

Đây chính là định nghĩa của từ khóa **MVC**: Models, Views và Controllers.

## Các thành phần của MVC

## 1. Model (Mô hình)

- **Vai trò**: Đại diện cho hình dạng của dữ liệu (shape of the data)
    
- **Nội dung**: Chứa tất cả các bảng (tables) hoặc các lớp (classes)
    
- **Ví dụ**: Trong ứng dụng thương mại điện tử, Model sẽ chứa các lớp như:
    
    - Products (Sản phẩm)
        
    - Orders (Đơn hàng)
        
    - Order Details (Chi tiết đơn hàng)
        
    - Shopping Cart (Giỏ hàng)
        

## 2. View (Giao diện)

- **Vai trò**: Đại diện cho giao diện người dùng (user interface)
    
- **Nội dung**: Tất cả những gì bạn thấy trên màn hình
    
- **Chức năng**: Kiểm soát các phần tử HTML trong dự án web
    
- **Ví dụ**: Form, biểu đồ, bảng dữ liệu hiển thị trên trình duyệt
    

## 3. Controller (Bộ điều khiển)

- **Vai trò**: Trái tim của ứng dụng MVC
    
- **Chức năng chính**:
    
    - Xử lý yêu cầu của người dùng (handle user request)
        
    - Hoạt động như giao diện giữa Model và View
        
    - Lấy dữ liệu từ cơ sở dữ liệu thông qua Model
        
    - Truyền dữ liệu đến View để hiển thị
        

## Quy trình hoạt động của MVC

## Luồng xử lý yêu cầu:

1. **Người dùng tương tác**: Click nút hoặc mở website
    
2. **Controller nhận yêu cầu**: Yêu cầu đầu tiên được gửi đến Controller
    
3. **Controller xử lý**:
    
    - Xác định Model nào cần lấy dữ liệu
        
    - Truy xuất tất cả dữ liệu cần thiết
        
    - Xử lý và chuyển đổi dữ liệu nếu cần
        
4. **Truyền dữ liệu đến View**: Controller gửi dữ liệu đã xử lý đến View
    
5. **View tạo HTML**:
    
    - Thêm dữ liệu vào định dạng HTML
        
    - Tạo nội dung hoàn chỉnh
        
6. **Trả về kết quả**: View gửi HTML hoàn chỉnh về Controller
    
7. **Hiển thị cho người dùng**: Controller gửi phản hồi cuối cùng đến màn hình người dùng
    

## Action Methods (Phương thức hành động)

- **Định nghĩa**: Các phương thức trong Controller định nghĩa các endpoints (điểm cuối)
    
- **Vai trò**: Xác định các hành động cụ thể mà Controller có thể thực hiện
    

## Routing mặc định

Trong cấu hình routing mặc định:

text

`Home/Index/{id?}`

- **Home**: Tên Controller
    
- **Index**: Tên Action Method
    
- **{id?}**: Tham số tùy chọn
    

Nếu không có route cụ thể được định nghĩa, hệ thống sẽ mặc định chuyển đến Home Controller và thực thi Index Action.

## Tóm tắt quan trọng

**Controller là trái tim của ứng dụng MVC** - đây là điều quan trọng nhất cần nhớ trong kiến trúc MVC. Controller đóng vai trò trung gian, điều phối toàn bộ luồng xử lý từ nhận yêu cầu của người dùng đến trả về kết quả cuối cùng.