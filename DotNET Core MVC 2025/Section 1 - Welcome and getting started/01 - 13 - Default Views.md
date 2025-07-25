# Layout và Master Page trong MVC

## Layout - Master Page của ứng dụng

## Vai trò của _Layout.cshtml:

Khi chạy ứng dụng, ngoài nội dung từ view (như `Index.cshtml`), chúng ta còn thấy **header** và **footer**. Những phần này được load từ **_Layout.cshtml** - master page của toàn bộ ứng dụng.

## Cấu trúc _Layout.cshtml:

xml

```html
<!DOCTYPE html> 
<html> 
<head>     
	<!-- CSS và styling --> 
</head> 
<body>     
	<header>        <!-- Navigation links: Home, Privacy -->    </header>          @RenderBody()         
	<footer>        <!-- Footer content -->    </footer> 
</body>
</html>
```

## RenderBody() Helper:

- **Chức năng**: Helper tích hợp sẵn trong MVC
    
- **Vai trò**: Hiển thị nội dung động từ controller
    
- **Cách hoạt động**:
    
    - Nếu controller trả về Index view → Hiển thị nội dung Index tại vị trí `@RenderBody()`
        
    - Nếu controller trả về Privacy view → Hiển thị nội dung Privacy tại vị trí `@RenderBody()`
        

## Các file quan trọng trong thư mục Shared

## 1. _ViewStart.cshtml

**Mục đích**: Định nghĩa layout mặc định cho ứng dụng

csharp

`@{     Layout = "_Layout"; }`

**Quan trọng**:

- Nếu thay đổi tên file layout, phải cập nhật tại đây
    
- Ví dụ: Đổi thành `Layout = "Layout"` sẽ gây lỗi nếu file không tồn tại
    

## 2. _ViewImports.cshtml

**Chức năng**: File import toàn cục (global import file)

**Nội dung típica:**

- **Using statements**: Thay vì viết `using` trong mọi file
    
- **Tag helpers**: Hỗ trợ các thẻ HTML đặc biệt
    
- **Models**: Import các model cần thiết
    

**Phạm vi áp dụng**:

- Chỉ áp dụng cho **Views**
    
- **Không** áp dụng cho Controllers hoặc Models
    

## 3. _ValidationScriptsPartial.cshtml

**Mục đích**: Chứa JavaScript cho client-side validation

**Lý do tách riêng**:

- Không phải trang nào cũng cần validation
    
- Chỉ include khi cần thiết
    
- Tối ưu hiệu suất tải trang
    

## Partial Views (Giao diện con)

## Định nghĩa:

**Partial Views** là các view không thể hiển thị độc lập, mà phải được sử dụng như một phần của view chính.

## Quy ước đặt tên:

- **Prefix**: Bắt đầu bằng dấu gạch dưới `_`
    
- **Ví dụ**: `_Layout.cshtml`, `_ValidationScriptsPartial.cshtml`
    
- **Mục đích**: Dễ nhận biết đây là component được sử dụng toàn ứng dụng
    

## Đặc điểm:

- **Không độc lập**: Không thể render riêng lẻ
    
- **Tái sử dụng**: Có thể được consume trong nhiều view khác nhau
    
- **Toàn cục**: Thường được dùng xuyên suốt ứng dụng
    

## Tag Helpers

## Ví dụ trong _Layout.cshtml:

xml

`<a asp-controller="Home" asp-action="Index">Home</a> <a asp-controller="Home" asp-action="Privacy">Privacy</a>`

**Lưu ý**: Tag helpers sẽ được giải thích chi tiết trong các video sau.

## Error.cshtml

**Chức năng**: View hiển thị thông báo lỗi khi có exception xảy ra trong ứng dụng.

## Cấu trúc tổng quan Views

text

```
Views/ 
├── Home/ 
│   ├── Index.cshtml 
│   └── Privacy.cshtml 
├── Shared/ 
│   ├── _Layout.cshtml           (Master page) 
│   ├── _ViewStart.cshtml        (Layout configuration) 
│   ├── _ViewImports.cshtml      (Global imports) 
│   
├── _ValidationScriptsPartial.cshtml 
│   └── Error.cshtml
```

## Luồng hoạt động Layout

## Quy trình render:

1. **Controller** trả về view (VD: Index)
    
2. **_ViewStart.cshtml** xác định layout (`_Layout`)
    
3. **_Layout.cshtml** được load với:
    
    - Header cố định
        
    - Footer cố định
        
    - Nội dung dynamic tại `@RenderBody()`
        
4. **View content** được inject vào `@RenderBody()`
    
5. **Kết quả cuối**: Trang hoàn chỉnh với layout + content
    

## Best Practices

## CSS và JavaScript toàn cục:

- **Đặt trong**: `_Layout.cshtml`
    
- **Áp dụng cho**: Toàn bộ ứng dụng
    
- **Ví dụ**: Bootstrap, jQuery, custom CSS
    

## Using Statements:

- **Đặt trong**: `_ViewImports.cshtml`
    
- **Lợi ích**: Không cần repeat trong mỗi view file
    
- **Phạm vi**: Chỉ áp dụng cho Views
    

## Tóm tắt quan trọng

**Layout System** là backbone của giao diện trong MVC:

- **_Layout.cshtml**: Master page chứa cấu trúc chung
    
- **_ViewStart.cshtml**: Cấu hình layout mặc định
    
- **_ViewImports.cshtml**: Import toàn cục cho views
    
- **RenderBody()**: Vị trí hiển thị nội dung dynamic
    
- **Partial Views**: Component tái sử dụng với prefix `_`
    

Hiểu rõ layout system giúp xây dựng giao diện nhất quán và dễ bảo trì cho toàn bộ ứng dụng.