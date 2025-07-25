# Định tuyến (Routing) trong ứng dụng MVC

## Khái niệm về Routing

**Định tuyến (Routing)** xác định rằng khi bạn nhập một URL, yêu cầu sẽ được gửi đến đâu trong ứng dụng. Trong ứng dụng MVC, chúng ta có một mẫu (pattern) nhất định để xử lý việc này.

## Cấu trúc URL Pattern trong MVC

## Phân tích URL

Khi xem xét routing, chúng ta cần loại bỏ phần tên miền (domain name) và chỉ tập trung vào phần sau đó:

- **Tên miền**: `localhost`, `google.com`, `.netmastery.com` (được loại bỏ khỏi pattern routing)
    
- **Phần routing**: Mọi thứ sau tên miền và số cổng
    

## Mẫu định tuyến cơ bản

Trong ứng dụng MVC, mẫu định tuyến điển hình là:

text

`/{controller}/{action}/{id?}`

**Hai từ khóa quan trọng nhất cần ghi nhớ:**

1. **Controller** (Bộ điều khiển)
    
2. **Action** (Hành động)
    

## Cách phân tích URL

## Cấu trúc tiêu chuẩn:

1. **Phần đầu tiên** sau tên miền = **Tên Controller**
    
2. **Phần thứ hai** = **Tên Action Method**
    
3. **Phần thứ ba** (tùy chọn) = **ID**
    

## Ví dụ phân tích URL:

|URL|Controller|Action|ID|
|---|---|---|---|
|`/category/index/3`|category|index|3|
|`/category`|category|index (mặc định)|null|
|`/category/edit/3`|category|edit|3|
|`/product/details/3`|product|details|3|

## Quy tắc mặc định

## Action mặc định

- Nếu không có action được định nghĩa trong URL, hệ thống sẽ tự động sử dụng **action "Index"**
    
- Ví dụ: `/category` sẽ được hiểu là `/category/index`
    

## Route mặc định trong Program.cs

text

`Home/Index/{id?}`

**Ý nghĩa:**

- **Controller mặc định**: Home
    
- **Action mặc định**: Index
    
- **ID**: Tùy chọn (ký hiệu `?`)
    

Khi không có gì được định nghĩa sau tên miền, ứng dụng sẽ tự động chuyển đến Home Controller và thực thi Index Action Method.

## Tầm quan trọng của việc hiểu Routing

## Lợi ích khi nắm vững routing:

- **Đọc hiểu URL**: Có thể xác định controller và action từ URL của ứng dụng MVC
    
- **Tùy chỉnh định tuyến**: Có thể thay đổi route mặc định nếu cần thiết
    
- **Kiểm soát luồng ứng dụng**: Hiểu cách ứng dụng điều hướng các yêu cầu
    

## Ghi chú quan trọng:

- Đây là **mẫu mặc định** được đội ngũ .NET cấu hình
    
- Có thể **tùy chỉnh** và **thay đổi** routing pattern trong các video sau
    
- **Controller** và **Action** là hai khái niệm cốt lõi cần ghi nhớ tuyệt đối
    

## Kết luận

Hiểu về routing là nền tảng quan trọng để làm việc với ứng dụng MVC. Từ việc phân tích URL, bạn có thể xác định được ứng dụng sẽ gọi controller nào và action method nào, giúp kiểm soát tốt hơn luồng xử lý của ứng dụng.