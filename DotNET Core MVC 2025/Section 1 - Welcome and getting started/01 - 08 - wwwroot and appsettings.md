# Thư mục wwwroot và File Cấu hình trong ASP.NET Core MVC

## Thư mục wwwroot

Thư mục **wwwroot** là một thư mục quan trọng trong ứng dụng ASP.NET Core, có chức năng lưu trữ tất cả nội dung tĩnh (static content) của dự án.

## Nội dung tĩnh là gì?

Nội dung tĩnh bao gồm:

- File CSS
    
- File JavaScript
    
- Các gói NuGet (NuGet packages) hoặc thư viện bên thứ ba (third party libraries)
    
- Hình ảnh, file PDF, PowerPoint và các file khác
    
- Bất kỳ nội dung nào không chứa mã HTML
    

## Cấu trúc mặc định của thư mục wwwroot

Khi tạo ứng dụng MVC mới, thư mục wwwroot sẽ có sẵn:

- **site.css**: File CSS toàn cục đã được sử dụng trong ứng dụng
    
- **site.js**: File JavaScript (trống, chỉ có template cơ bản)
    
- **Thư mục lib**: Chứa các thư viện như Bootstrap, jQuery, jQuery Validation
    

> **Lưu ý quan trọng**: Mọi nội dung tĩnh trong tương lai đều phải được thêm vào thư mục wwwroot.

## File Appsettings.json

## Mục đích sử dụng

File **appsettings.json** là nơi lưu trữ:

- Chuỗi kết nối cơ sở dữ liệu (connection strings)
    
- Các khóa bí mật (secret keys) của ứng dụng
    
- Cấu hình email (ví dụ: SendGrid)
    
- Thông tin kết nối Azure Blob Storage hoặc Azure Storage Account
    

## Lợi ích của việc tập trung cấu hình

Việc lưu trữ tất cả cấu hình ở một nơi giúp:

- Dễ dàng thay đổi kết nối mà không cần tìm kiếm trong toàn bộ mã nguồn
    
- Quản lý tập trung các thông tin nhạy cảm
    
- Bảo mật tốt hơn cho ứng dụng
    

## Cấu hình theo môi trường

ASP.NET Core hỗ trợ các file cấu hình khác nhau cho từng môi trường:

- **appsettings.json**: Cấu hình chung
    
- **appsettings.development.json**: Cấu hình cho môi trường phát triển (development)
    
- **appsettings.production.json**: Cấu hình cho môi trường sản xuất (production)
    

## Cách hoạt động

Hệ thống sẽ tự động chọn file cấu hình phù hợp dựa trên biến môi trường **ASP.NET Core Environment** được định nghĩa trong file **launchsettings.json**.

Ví dụ:

- Nếu môi trường là "Development" → sử dụng appsettings.development.json
    
- Nếu môi trường là "Production" → sử dụng appsettings.production.json
    

## Tóm tắt

- **Thư mục wwwroot**: Lưu trữ tất cả nội dung tĩnh (CSS, JS, hình ảnh, v.v.)
    
- **File appsettings.json**: Lưu trữ chuỗi kết nối và các khóa bí mật
    
- **Cấu hình theo môi trường**: Hỗ trợ nhiều file cấu hình cho các môi trường khác nhau
    
- **Quản lý tập trung**: Giúp dễ dàng bảo trì và thay đổi cấu hình
    

Trong video tiếp theo sẽ tìm hiểu về file **Program.cs** - một file quan trọng khác trong ứng dụng.