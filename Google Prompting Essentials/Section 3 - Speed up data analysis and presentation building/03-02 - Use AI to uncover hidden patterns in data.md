## Phân tích Dữ liệu với AI Tạo sinh - Kỹ thuật Prompting

### Nguyên tắc cơ bản

- **Dữ liệu có thể dạy bạn rất nhiều điều**, nhưng trước tiên bạn cần biết cách diễn giải nó
- Sử dụng [[Prompting Framework]] một cách có suy nghĩ để tạo ra các đầu vào xuất sắc
- Mục tiêu: Khai thác insights (thông tin chi tiết) và patterns (mô hình) từ dữ liệu


### Lưu ý quan trọng trước khi bắt đầu

- **Không phải tất cả [[AI Tools]] đều hoạt động được với dữ liệu**
- Cần kiểm tra khả năng của công cụ trước khi sử dụng
- Ví dụ minh họa sử dụng: [[Gemini]] models trong [[Google AI Studio]]


### Nguyên tắc sử dụng AI có trách nhiệm

- **Luôn xem xét chính sách của tổ chức** trước khi đưa dữ liệu nhạy cảm hoặc bí mật vào prompt
- Trong ví dụ này: sử dụng dữ liệu công khai từ [[Kaggle]]


### Quy trình thực hành với dữ liệu chuỗi cửa hàng tạp hóa

#### Bước 1: Chuẩn bị và tải dữ liệu

- **Upload dữ liệu trực tiếp** từ Google Drive (nếu dùng Google Sheet)
- Từ máy tính (nếu dùng Microsoft Excel)
- [[AI Studio]] giúp phân tích dữ liệu để tìm trends (xu hướng) và patterns


#### Bước 2: Tổ chức dữ liệu

- **Prompt mẫu**: "Attached is a Google sheet of store data. How can I create a new column in sheets that calculates the average sales per customer for each store?"
- Kết quả:
    - Mô hình cung cấp gợi ý hữu ích để tính doanh số trung bình mỗi khách hàng
    - Giải thích cách sử dụng công thức mô tả rõ ràng để đặt tên cột mới


#### Bước 3: Tìm kiếm xu hướng

- **Prompt mẫu**: "Give me insights into the relationship between daily customer count, items available and sales based on the given data"
- **Kết quả thú vị**:
    - Không có mối tương quan rõ ràng giữa số lượng sản phẩm trong cửa hàng và tổng doanh số
    - Một số cửa hàng nhỏ thậm chí vượt trội hơn các cửa hàng lớn
    - Đưa ra các lý do tiềm ẩn để điều tra thêm và suy nghĩ về chiến lược bán hàng


### Lợi ích của việc sử dụng AI trong phân tích dữ liệu

- **Tiết kiệm thời gian**: Không cần dành hàng giờ để xử lý dữ liệu
- **Hiệu quả cao**: Chỉ cần vài prompts để có kết quả
- **Trích xuất insights có ý nghĩa** một cách nhanh chóng
- Có thể **iterate (lặp lại)** prompt để có kết quả gần với yêu cầu hơn


### Ghi chú thêm

- Luôn **xem xét và điều chỉnh prompt** nếu kết quả chưa phù hợp
- Sử dụng phương pháp **step-by-step** (từng bước) khi yêu cầu hỗ trợ
- Áp dụng cho bất kỳ bảng tính nào cần phân tích

**Liên kết:** [[Generative AI]], [[Prompting Framework]], [[Data Analysis]], [[Google AI Studio]], [[Gemini]], [[AI Tools]], [[Kaggle]]

