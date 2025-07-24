# File Program.cs trong ASP.NET Core MVC

## Tổng quan về Program.cs

File **Program.cs** là file chính trong ứng dụng ASP.NET Core. Trong các phiên bản cũ hơn của .NET Core, chúng ta có hai file riêng biệt:

- **Program.cs**
    
- **Startup.cs**
    

Tuy nhiên, với phiên bản mới hơn, nhóm phát triển .NET đã kết hợp cả hai file này thành một file duy nhất là **Program.cs**.

## Hai nhiệm vụ chính của Program.cs

Khi cấu hình ứng dụng .NET, có hai việc quan trọng cần thực hiện:

## 1. Thêm Services vào Container

- Sử dụng `builder.Services` để thêm các dịch vụ (services)
    
- Ví dụ: `AddControllersWithViews()` để hỗ trợ kiến trúc MVC
    
- Nơi để thêm các dependency injection (tiêm phụ thuộc) trong tương lai
    

## 2. Cấu hình Request Pipeline

- Định nghĩa cách xử lý các yêu cầu (requests) đến ứng dụng
    
- Sử dụng các middleware để xử lý pipeline
    

## Chi tiết cấu hình trong Program.cs

## Tạo Builder và thêm Services

csharp

`var builder = WebApplication.CreateBuilder(); builder.Services.AddControllersWithViews();`

## Cấu hình Environment

csharp

`app.Environment.IsDevelopment()`

Hệ thống cung cấp các helper methods:

- `IsDevelopment()`: Kiểm tra môi trường phát triển
    
- `IsProduction()`: Kiểm tra môi trường sản xuất
    
- `IsStaging()`: Kiểm tra môi trường staging
    
- `IsEnvironment()`: Kiểm tra môi trường tùy chỉnh
    

## Xử lý Exception (Ngoại lệ)

- **Môi trường Development**: Hiển thị chi tiết lỗi
    
- **Môi trường khác**: Chuyển hướng đến trang lỗi (`/Home/Error`)
    

## Cấu hình Pipeline

## Static Files (File tĩnh)

csharp

`app.UseStaticFiles();`

- Cấu hình đường dẫn **wwwroot**
    
- Cho phép truy cập các file tĩnh trong ứng dụng
    

## HTTPS Redirect

csharp

`app.UseHttpsRedirection();`

## Routing và Authorization

csharp

`app.UseRouting(); app.UseAuthorization();`

## Cấu hình Route mặc định

csharp

`app.MapControllerRoute(     name: "default",    pattern: "{controller=Home}/{action=Index}/{id?}" );`

**Giải thích pattern**:

- `{controller=Home}`: Controller mặc định là Home
    
- `{action=Index}`: Action mặc định là Index
    
- `{id?}`: ID là tùy chọn (dấu `?` có nghĩa là có thể null)
    

## Chạy ứng dụng

csharp

`app.Run();`

## Tóm tắt quan trọng

## Điểm cần nhớ

- **Program.cs** là file trung tâm để cấu hình ứng dụng
    
- Hai nhiệm vụ chính: **thêm services** và **cấu hình pipeline**
    
- Khi cần cấu hình gì đó cho ứng dụng, hãy tìm đến file **Program.cs**
    

## Lời khuyên cho người học

- Nếu bạn chưa hiểu hết các khái niệm như middleware pipeline, đừng lo lắng
    
- Điều quan trọng là biết **Program.cs** là nơi để cấu hình ứng dụng
    
- Khi tiến triển trong khóa học, mọi thứ sẽ trở nên rõ ràng hơn
    

## Thuật ngữ quan trọng

- **Services Container**: Nơi chứa các dịch vụ của ứng dụng
    
- **Request Pipeline**: Chuỗi xử lý các yêu cầu HTTP
    
- **Middleware**: Các thành phần xử lý trong pipeline
    
- **Dependency Injection**: Kỹ thuật tiêm phụ thuộc quan trọng trong .NET Core
    

> **Mục tiêu học tập**: Hiểu rằng Program.cs là file cấu hình chính và biết nơi để thêm services cũng như cấu hình pipeline khi cần thiết.