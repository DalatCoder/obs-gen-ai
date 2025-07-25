## Tiêm phụ thuộc (Dependency Injection)

### Khái niệm cơ bản

Tiêm phụ thuộc (Dependency Injection) là một **mẫu thiết kế (design pattern)** trong đó một lớp hoặc đối tượng nhận các lớp phụ thuộc được tiêm vào thay vì tự tạo ra chúng.

**Mục đích:**

- Không phải tự tạo, quản lý và giải phóng đối tượng
- Cải thiện tính **liên kết lỏng lẻo (loose coupling)** giữa các lớp
- Là câu hỏi phỏng vấn phổ biến trong lập trình .NET


### Ví dụ thực tế - Bob đi bộ đường dài

Để hiểu khái niệm DI, hãy tưởng tượng Bob muốn đi bộ đường dài:

- Bob cần nhiều đồ dùng: bản đồ, đèn pin, thanh protein...
- Anh ấy đặt tất cả vào **ba lô (container)**
- Khi cần sử dụng, Bob chỉ việc lấy từ ba lô ra

**Nguyên lý tương tự:**

- Đặt các đối tượng cần thiết vào **vùng chứa (container)**
- Khi cần sử dụng, lấy trực tiếp từ vùng chứa
- Không phải tự tạo hoặc quản lý các đối tượng đó


### Vấn đề khi không có Dependency Injection

#### Tình huống: 3 trang web cần chức năng chung

Giả sử có 3 trang web cần:

- Gửi email
- Truy cập cơ sở dữ liệu

**Cách làm truyền thống:**

```csharp
// Trong mỗi trang, phải viết code tương tự:
var db = new DB();
var result = db.GetData();
db.Dispose();

var email = new Email();
email.SendEmail();
email.Dispose();
```

**Vấn đề phát sinh:**

- **Code trùng lặp** trong cả 3 trang
- Khi cần thay đổi lớp `DB` thành `DB_new` → phải sửa ở **tất cả các trang**
- Nếu có 30 hay 300 trang → công việc sửa đổi trở nên **rất tốn thời gian**
- Phải tự quản lý việc tạo và giải phóng đối tượng


### Giải pháp với Dependency Injection

#### Cấu trúc mới

- **3 trang web** (như trước)
- **Email và Database** (chức năng chung)
- **Vùng chứa DI (DI Container)** - thành phần đặc biệt


#### Cách hoạt động

1. **Đăng ký dịch vụ** trong DI Container:

```csharp
// Đăng ký interface và implementation
container.Register<IEmail, Email>();
container.Register<IDb, DB>();
```

2. **Các trang yêu cầu** implementation thông qua interface:
    - Trang không biết implementation cụ thể là gì
    - Chỉ cần yêu cầu `IDb` hoặc `IEmail`
3. **DI Container xử lý:**
    - Tự động tìm implementation phù hợp
    - Tạo đối tượng và cung cấp cho trang
    - Quản lý việc tạo và giải phóng đối tượng

#### Ưu điểm khi thay đổi

Khi cần thay đổi implementation:

```csharp
// Chỉ cần sửa ở một nơi - trong DI Container
container.Register<IEmail, Email_new>();  // Thay Email bằng Email_new
container.Register<IDb, DB_new>();        // Thay DB bằng DB_new
```

**Kết quả:**

- Tất cả các trang tự động nhận implementation mới
- Không cần sửa code ở 30 hay 300 trang
- **Email và Database đã liên kết lỏng lẻo** với các lớp khác


### Tích hợp trong .NET Framework

- **Dependency Injection được tích hợp sẵn** trong .NET Framework
- Chỉ cần **đăng ký dịch vụ** (register services)
- Framework tự động xử lý việc còn lại


### Ghi chú thêm

- DI là một **khái niệm quan trọng** trong kiến trúc phần mềm hiện đại
- Giúp code **dễ bảo trì, kiểm thử và mở rộng**
- Là nền tảng cho nhiều framework và thư viện .NET

*Liên kết: [[.NET Framework]], [[Design Patterns]], [[Software Architecture]]*

