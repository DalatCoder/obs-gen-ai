# Tạo dự án ASP.NET Core MVC với Visual Studio 2022

## Bước 1: Khởi tạo dự án mới

## Mở Visual Studio 2022

- Khởi động Visual Studio 2022
    
- Chọn **"Create a new project"** ở phía bên trái màn hình
    

## Tìm kiếm template MVC

- Trong phần recent project templates (các mẫu dự án gần đây), tìm kiếm **"MVC"**
    
- Kết quả sẽ hiển thị **ASP.NET Core Web App**
    

## Lựa chọn template phù hợp

- **Chọn đúng template**: ASP.NET Core Web App có **Model View và Controller (MVC)**
    
- **Không chọn**: Web app không có MVC (sử dụng Razor Pages)
    

## Bước 2: Cấu hình dự án

## Thông tin cơ bản

- **Tên dự án (Project name)**: `bulky web`
    
- **Vị trí lưu trữ (Location)**: Chọn thư mục mong muốn
    
- **Tên solution (Solution name)**: `bulky`
    
    - Lý do: Solution sẽ chứa nhiều project khác nhau
        

## Cấu hình framework và tùy chọn

- **Framework**: Chọn **.NET 8**
    
- **Authentication type (Loại xác thực)**: Chọn **"None"**
    
    - Lý do: Sẽ thêm authentication sau, hiện tại giữ đơn giản
        
- **Configure for HTTPS**: Giữ nguyên cài đặt mặc định
    
- **Do not use top level statements**: Không chọn
    
    - Lý do: Chỉ thêm using statements ở đầu file, không quan trọng lắm
        

## Hoàn tất tạo dự án

- Nhấn nút **"Create"** để tạo dự án
    
- Visual Studio sẽ tự động tạo các files và folders mặc định
    

## Bước 3: Thêm vào source control (Git)

## Thiết lập Git repository

- Thêm dự án vào source control (kiểm soát mã nguồn)
    
- Đăng nhập vào Git repository (nếu chưa đăng nhập)
    

## Cấu hình repository

- **Tên repository**: `bulky_MVC`
    
- **Loại repository**: Private (riêng tư)
    
    - Lưu ý: Sẽ chuyển thành public (công khai) sau khi khóa học được phát hành
        
- Nhấn **"Create and Push"**
    

## Commit code

- Hệ thống hiển thị **2 outgoing changes** (2 thay đổi cần đẩy lên)
    
- Thực hiện push để đưa code lên repository
    
- Hoàn tất việc tạo dự án và commit code lên Git
    

## Tóm tắt

Đã hoàn thành việc tạo dự án ASP.NET Core MVC với các đặc điểm:

- Sử dụng .NET 8 framework
    
- Template MVC (Model-View-Controller)
    
- Chưa có authentication (sẽ thêm sau)
    
- Đã được lưu trữ trên Git repository
    
- Sẵn sàng cho việc phát triển tiếp theo
    

## Bước tiếp theo

- Khám phá các files và folders được tạo mặc định
    
- Bắt đầu phát triển các tính năng của ứng dụng