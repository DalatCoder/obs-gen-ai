# Khám phá cấu trúc dự án: Dependencies và Launch Settings

## Connected Services (Dịch vụ kết nối)

- Hiện tại **Connected Services** đang trống
    
- Sẽ bỏ qua phần này vì chưa có nội dung
    

## Dependencies (Phụ thuộc)

## Khái niệm Dependencies

- Khi xây dựng ứng dụng .NET, thường sẽ cần thêm nhiều **packages** (gói thư viện) để có thêm chức năng
    
- Ví dụ các trường hợp cần thêm packages:
    
    - Truy cập cơ sở dữ liệu (database access)
        
    - Tích hợp thanh toán (payment integration)
        

## Trạng thái hiện tại

- **Hiện tại**: Không có package nào trong dependencies
    
- **Tương lai**: Sẽ thêm các packages khi cần thiết
    

## Dependencies với nhiều Project

- Khi có nhiều project, có thể thêm project khác như một dependency
    
- Dependencies sẽ tự động phản ánh điều này
    
- Sẽ được trình bày trong các video sau
    

## Định nghĩa Dependencies

- **Dependencies** có nghĩa là project này phụ thuộc vào:
    
    - Các packages (từ NuGet)
        
    - Các project khác
        
- Hiện tại chưa có phụ thuộc nào
    

## Properties Folder và Launch Settings

## Cấu trúc

- **Properties folder** chứa file **launchSettings.json**
    

## Chức năng của launchSettings.json

- Định nghĩa các cài đặt khi **chạy** hoặc **debug** ứng dụng
    
- Xác định những gì xảy ra khi nhấn nút **HTTPS** để chạy ứng dụng
    

## Cấu hình IIS Settings

## Cài đặt URL và Port

- **IIS Settings** định nghĩa:
    
    - URL cho **HTTP** với port number cụ thể
        
    - URL cho **HTTPS** với port number riêng biệt
        

## Profiles (Hồ sơ cấu hình)

## Các loại Profiles

Profiles phản ánh những gì hiển thị trong dropdown, bao gồm:

- **HTTP profile**
    
- **HTTPS profile**
    
- **IIS Express**
    

## Cấu hình Profile

- Mỗi profile định nghĩa URL để chạy ứng dụng
    
- Thiết lập các **environment variables** (biến môi trường)
    

## Environment Variables (Biến môi trường)

## Khái niệm

- **Environment variables** giống như **global variables** (biến toàn cục)
    
- Được định nghĩa và có thể sử dụng trong ứng dụng
    

## Ví dụ sử dụng Environment Variables

## 1. Phân biệt môi trường Development vs Production

- **ASP.NET Core Environment = "Development"**:
    
    - Sử dụng development database
        
    - Kiểm tra biến này trong code để quyết định database nào sử dụng
        
- **Production environment**:
    
    - Sử dụng production database
        

## 2. Payment Integration

- **Development environment**:
    
    - Sử dụng development keys
        
    - Không cần thẻ tín dụng thật
        
- **Production environment**:
    
    - Sử dụng production keys
        
    - Xử lý thanh toán thẻ tín dụng thật
        

## Quản lý Environment Variables

- Tất cả environment variables và profiles được định nghĩa trong **launchSettings.json**
    

## Thực hành với HTTPS Profile

## Profile hiện tại

- Đang sử dụng **HTTPS profile**
    
- **Application URL**: Cổng 7169
    

## Thay đổi Port

1. **Chỉnh sửa**: Thay đổi port từ 7169 thành 7001
    
2. **Chạy ứng dụng**: Ứng dụng chạy trên port 7001
    
3. **Kết quả**: Có thể thay đổi thuộc tính theo yêu cầu
    

## Chuyển đổi Profile

- Có thể **toggle** (chuyển đổi) giữa các profiles
    
- Chọn profile nào muốn chạy ứng dụng
    
- Cũng có **IIS Express** để lựa chọn
    

## Lưu ý quan trọng

## Về việc chỉnh sửa

- **Thông thường**: Không thay đổi profiles nhiều
    
- **Mục đích**: Cung cấp tổng quan 5 phút về launchSettings.json
    

## Quản lý thay đổi

- Có thể **undo git changes** để khôi phục cài đặt gốc
    
- Linh hoạt trong việc sử dụng port tùy ý
    

## Tóm tắt

## Đã đề cập

1. **Connected Services**: Trống, bỏ qua
    
2. **Dependencies**: Chưa có packages, sẽ thêm sau
    
3. **Properties/launchSettings.json**:
    
    - Cấu hình chạy/debug
        
    - Profiles và environment variables
        
    - Thay đổi ports và URLs
        

## Ý nghĩa

- **launchSettings.json** là file cấu hình quan trọng cho development
    
- Cho phép tùy chỉnh môi trường development vs production
    
- Linh hoạt trong việc cấu hình URLs và ports
    

## Bước tiếp theo

- Khám phá **Controllers folder** và các files khác trong dự án
    
- Tìm hiểu chi tiết về cấu trúc MVC