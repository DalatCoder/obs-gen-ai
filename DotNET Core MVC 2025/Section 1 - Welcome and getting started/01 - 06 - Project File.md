# Khám phá cấu trúc dự án và chạy ứng dụng lần đầu

## Chạy ứng dụng mặc định

## Khởi chạy ứng dụng

- Nhấn nút **HTTPS** để build dự án và mở trong trình duyệt
    
- Ứng dụng sẽ được build và tự động mở trong browser
    

## Giao diện mặc định

Ứng dụng mặc định bao gồm các thành phần sau:

- **Header (tiêu đề)**: Chứa navigation menu
    
- **Navigation (điều hướng)**: Đã được cấu hình sẵn
    
    - **Home page**: Hiển thị trang chào mừng
        
    - **Privacy page**: Hiển thị trang riêng tư khác
        
- **Body (nội dung chính)**: Khu vực hiển thị nội dung
    
- **Footer (chân trang)**: Phần cuối trang
    

## Ưu điểm

- Layout cơ bản đã được thiết lập sẵn bởi .NET project mặc định
    
- Tiết kiệm thời gian thiết lập ban đầu
    

## Hiểu về Project và Solution

## Khái niệm cơ bản

- **Solution (giải pháp)**: `bulky` - có thể chứa nhiều project
    
- **Project (dự án)**: `bulky web` - hiện tại chỉ có một project trong solution
    

## Cấu trúc phân cấp

text

`Solution: bulky └── Project: bulky web`

## Kiểm tra Project File

## Cách truy cập Project File

1. Right-click vào **Project** (bulky web), không phải solution
    
2. Chọn **"Edit Project File"**
    

## Nội dung Project File

## Cấu trúc đơn giản

- Project file trong .NET 8 đã được đơn giản hóa đáng kể
    
- Phiên bản cũ của .NET Core phức tạp hơn nhiều
    

## Các thuộc tính chính trong PropertyGroup

**1. Target Framework (Framework đích)**

xml

`<TargetFramework>net8.0</TargetFramework>`

- Xác định đang sử dụng .NET 8.0 framework
    
- Thuộc tính quan trọng nhất trong project file
    

**2. Nullable**

xml

`<Nullable>enable</Nullable>`

- Tính năng được giới thiệu từ .NET 6
    
- Chi tiết sẽ được giải thích trong các video sau
    

**3. Implicit Using Statements (Câu lệnh using ngầm định)**

xml

`<ImplicitUsings>enable</ImplicitUsings>`

## Giải thích Implicit Using Statements

## Khái niệm

- Tương tự như **import statements** trong các framework frontend khác
    
- Cho phép import các thư viện từ bên ngoài
    

## Khi được bật (enabled)

- Các using statements mặc định từ .NET libraries sẽ được tự động include
    
- Không cần viết các import statements thủ công
    

## Khi được tắt (disabled)

- Phải explicitly thêm import statements
    
- Tăng độ phức tạp nhưng cho phép kiểm soát chi tiết hơn
    

## Khuyến nghị

- Giữ nguyên setting **enabled** để thuận tiện trong phát triển
    

## Vai trò của Project File

## Chức năng chính

- Chứa tất cả **project properties** được thiết lập bởi .NET
    
- Nơi thêm các **NuGet packages** và **NPM packages**
    

## Cập nhật tự động

- Khi thêm NuGet package, project file sẽ được cập nhật tự động
    
- Sẽ được trình bày chi tiết trong các video tiếp theo
    

## Tóm tắt

## Nội dung đã đề cập

1. **Ứng dụng mặc định**: Layout cơ bản với header, navigation, body, footer
    
2. **Project structure**: Hiểu về solution và project
    
3. **Project file**: Cấu trúc đơn giản với các thuộc tính chính:
    
    - Target Framework (.NET 8)
        
    - Nullable (sẽ giải thích sau)
        
    - Implicit Using Statements (thuận tiện cho development)
        

## Điểm quan trọng

- Project file đã được đơn giản hóa trong các phiên bản mới
    
- .NET 8 framework là nền tảng chính
    
- Implicit using giúp giảm boilerplate code
    

## Bước tiếp theo

- Khám phá chi tiết các files và folders khác trong dự án
    
- Tìm hiểu cách project file được cập nhật khi thêm packages
    
- Giải thích chi tiết về Nullable feature