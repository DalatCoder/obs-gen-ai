# Hoạt động thực tế của Controller, Action và View

## Cấu trúc thư mục trong Solution Explorer

Trong Solution Explorer có 3 thư mục chính chưa được khám phá:

- **Views** (Giao diện)
    
- **Models** (Mô hình)
    
- **Controllers** (Bộ điều khiển)
    

## Quy tắc đặt tên Controller

## Quy tắc bắt buộc:

- **Tên controller** phải có hậu tố **"Controller"**
    
- Ví dụ: `HomeController`, `ProductController`
    
- **Vị trí**: Phải được đặt trong thư mục **Controllers**
    
- **Lưu ý**: Nếu đặt sai vị trí, controller sẽ không hoạt động
    

## Ví dụ trong dự án:

- Có `HomeController` trong thư mục Controllers
    
- Models chỉ có `ErrorViewModel` - một class cơ bản với 2 properties
    

## Mối quan hệ giữa Controller và View

## Quy tắc tổ chức thư mục:

- Mỗi controller sẽ có thư mục tương ứng trong **Views**
    
- **Tên thư mục** = **Tên controller** (không bao gồm từ "Controller")
    
- Ví dụ: `HomeController` → thư mục `Home` trong Views
    

## Cấu trúc thực tế:

text

```
Controllers/   
└── HomeController.cs Views/   
└── Home/      
	├── Index.cshtml      
	└── Privacy.cshtml
```

## Action Methods trong Controller

## Định nghĩa Action Method:

- Là các phương thức trong Controller class
    
- Trả về kiểu `IActionResult`
    
- Tên action method tương ứng với tên view
    

## Ví dụ trong HomeController:

csharp

```c#
public IActionResult Index() {     
	return View(); 
} 

public IActionResult Privacy() {    
	return View(); 
}
```

## Cách hệ thống xử lý yêu cầu

## Luồng thực thi:

1. **URL**: `/Home/Index`
    
2. **Hệ thống tìm**: HomeController
    
3. **Thực thi**: Index() action method
    
4. **Trả về**: View từ `/Views/Home/Index.cshtml`
    

## Quy tắc mặc định cho View:

- `return View()` → Tìm view cùng tên với action method
    
- Tìm trong thư mục cùng tên với controller
    
- Phần mở rộng: `.cshtml`
    

## Debugging và kiểm tra

## Cách sử dụng Breakpoint:

1. **Thêm breakpoint**: Click vào ký hiệu tròn bên trái dòng code
    
2. **Chạy ứng dụng**: Khi truy cập URL, breakpoint sẽ được kích hoạt
    
3. **Kiểm tra**: Xác nhận action method nào được thực thi
    

## Kết quả debugging:

- URL `/Home/Index` → Kích hoạt breakpoint tại `Index()` action
    
- URL `/Home/Privacy` → Kích hoạt breakpoint tại `Privacy()` action
    

## Tùy chỉnh View được trả về

## Override view mặc định:

csharp

```c#
public IActionResult Index() {     
	return View("Privacy"); // Trả về Privacy.cshtml thay vì Index.cshtml 
}
```

## Thay đổi route mặc định:

- Trong Program.cs có thể thay đổi: `Home/Index/{id?}`
    
- Thành: `Home/Privacy/{id?}`
    
- Kết quả: Trang mặc định sẽ hiển thị Privacy view
    

## Điểm quan trọng cần ghi nhớ

## Model không luôn bắt buộc:

- Controller có thể trả về **static view** (view tĩnh)
    
- Không phải lúc nào cũng cần Model để render view
    
- Tùy thuộc vào yêu cầu của ứng dụng
    

## Naming Convention (Quy ước đặt tên):

- **Controller class**: Tên + "Controller" (VD: HomeController)
    
- **Thư mục Views**: Chỉ tên controller (VD: Home)
    
- **View files**: Tên action method + .cshtml
    

## Debugging Tips:

- Sử dụng breakpoint để theo dõi luồng thực thi
    
- Kiểm tra URL pattern để xác định controller/action được gọi
    
- Quan sát mối quan hệ giữa URL và code thực thi
    

## Tóm tắt

**Kiến trúc MVC** có thể phức tạp khi mới bắt đầu, nhưng pattern này rất mạnh mẽ. Việc hiểu 50-70% nội dung ở giai đoạn này là tiến bộ tốt. Khi bắt đầu thực hành trong các phần tiếp theo, mọi thứ sẽ trở nên rõ ràng và dễ hiểu hơn.

**Điểm then chốt**: Controller xử lý yêu cầu → Thực thi Action Method → Trả về View tương ứng → Hiển thị cho người dùng.