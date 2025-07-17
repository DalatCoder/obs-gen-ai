# Prompting đa phương thức (Multimodal Prompting)

## Khái niệm Multimodal Prompting

**Prompting đa phương thức (Multimodal Prompting)** là việc sử dụng **nhiều loại phương tiện khác nhau** để tạo prompt cho công cụ trí tuệ nhân tạo tạo sinh (Gen AI), chẳng hạn như:

- **Hình ảnh + Văn bản**
    
- **Âm thanh + Văn bản**
    
- Các kết hợp khác
    

## Ứng dụng trong môi trường làm việc

## Các trường hợp sử dụng phổ biến

**Phân tích dữ liệu trực quan:**

- Chụp ảnh biểu đồ và yêu cầu Gen AI giải thích dữ liệu bằng ngôn ngữ đơn giản
    

**Thiết kế và branding:**

- Upload các lựa chọn logo khác nhau cho việc đổi thương hiệu công ty
    
- Yêu cầu Gen AI đưa ra thêm lựa chọn dựa trên từng hướng thiết kế
    

**Xử lý ngôn ngữ:**

- Ghi âm tiếng nước ngoài và yêu cầu phiên dịch sang ngôn ngữ hiểu được
    

## Ví dụ thực tế 1: Tạo caption mạng xã hội cho nail art

## Tình huống

Một doanh nhân cần tạo caption mạng xã hội cho thiết kế nail art mới đang bán.

## Quy trình thực hiện

**Bước 1:** Chụp ảnh sản phẩm nail art

**Bước 2:** Input hình ảnh vào Gemini với prompt:

text

`"Viết một bài đăng mạng xã hội với hình ảnh này.  Bài đăng cần vui vẻ, ngắn gọn và tập trung vào việc  đây là bộ sưu tập thiết kế mới tôi đang bán"`

## Áp dụng Prompting Framework

Mặc dù sử dụng hình ảnh, vẫn cần áp dụng các yếu tố khác của prompting framework:

- **Chỉ định nhiệm vụ** (task): Viết bài đăng mạng xã hội
    
- **Thêm bối cảnh** (context): Bộ sưu tập thiết kế mới đang bán
    
- **Định dạng** (format): Vui vẻ, ngắn gọn
    

## Tối ưu hóa thêm

**Để có tone/voice cụ thể:**

- Có thể input thêm một số caption từ các bài đăng trước đó làm tài liệu tham khảo
    

**Kết quả mẫu:**

- Gemini phân tích hình ảnh và tạo caption thú vị
    
- Sử dụng emoji để chia nhỏ văn bản
    
- Tương tác với followers bằng cách đặt câu hỏi về thiết kế yêu thích
    

## Ví dụ thực tế 2: Trích xuất thông tin từ lịch trình hội nghị

## Tình huống

Tham dự hội nghị, nhận được lịch trình sự kiện và muốn team tập trung vào một số sự kiện cụ thể.

## Prompt mẫu

text

`"Tôi muốn gửi lời nhắc cho đồng nghiệp về một số sự kiện  cụ thể từ lịch trình hội nghị này.  Trích xuất thời gian của keynote speaker và hai panel discussion  từ lịch trình này thành một bảng"`

## Áp dụng Framework

- **Chỉ định nhiệm vụ**: Trích xuất thông tin
    
- **Cung cấp bối cảnh**: Lời nhắc cho đồng nghiệp về sự kiện cụ thể
    
- **Định dạng**: Bảng (table)
    

## Kết quả và mở rộng

- **Bảng rõ ràng** giúp team dễ dàng biết đi đâu và khi nào
    
- **Có thể mở rộng thêm**: Yêu cầu Gemini soạn thảo email về các sự kiện này
    

## Lợi ích của Multimodal Prompting

## Phản ánh cách trải nghiệm thế giới tự nhiên

**Trong thực tế:**

- Con người không chỉ thảo luận từ ngữ hoặc hình ảnh riêng lẻ trong bài thuyết trình
    
- Chúng ta **xây dựng kết nối** giữa chúng để hiểu đầy đủ hơn về chủ đề
    

**Trong AI:**

- **Kết hợp** văn bản, hình ảnh và các phương thức khác
    
- **Mở ra cách mới** để giải quyết vấn đề hoặc tiết kiệm thời gian
    

## Các ứng dụng đa dạng khác

**Xử lý bản đồ và không gian:**

- Chuyển đổi ảnh bản đồ thành danh sách địa danh nổi tiếng
    
- Trích xuất danh sách tên phòng từ sơ đồ tầng văn phòng
    

**Phân tích âm thanh:**

- Tìm kiếm insight quan trọng trong file âm thanh
    

**Xử lý tài liệu hình ảnh:**

- Trích xuất thông tin từ các tài liệu được chụp ảnh
    

## Nguyên tắc quan trọng

## Duy trì Prompting Framework

**Bất kể phương thức nào** bạn đang sử dụng để prompt, luôn nhớ:

- **Áp dụng prompting framework** để đạt kết quả tốt nhất
    
- **Chỉ định nhiệm vụ rõ ràng**
    
- **Cung cấp bối cảnh hữu ích**
    
- **Xác định định dạng mong muốn**
    

## Câu hỏi để suy ngẫm

**"Làm thế nào bạn có thể tận dụng các phương thức khác nhau trong prompt để hỗ trợ công việc?"**

Multimodal prompting mở ra những khả năng mới trong việc tương tác với AI, giúp công việc hiệu quả hơn bằng cách kết hợp nhiều loại dữ liệu đầu vào khác nhau.