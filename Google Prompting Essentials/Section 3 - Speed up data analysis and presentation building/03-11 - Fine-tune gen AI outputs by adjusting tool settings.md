## Tinh chỉnh Kết quả AI Generative bằng Cách Điều chỉnh Thiết lập Công cụ

### Giới thiệu về Sampling Parameters

Các công cụ AI generative sử dụng sự kết hợp giữa các mẫu đã học và xác suất để quyết định từ tiếp theo. Quá trình này giống như việc tung xúc xắc để chọn từ, nhưng bạn có thể ảnh hưởng đến kết quả của "lần tung xúc xắc" đó.

Một số công cụ như [Google AI Studio](https://aistudio.google.com/prompts/new_chat) cung cấp bảng điều khiển cho phép điều chỉnh các thiết lập này, thường gọi là **tham số lấy mẫu** (sampling parameters):

- Hoạt động như các rào chắn hướng dẫn việc lựa chọn từ của AI
- Giúp tạo ra kết quả tốt hơn và phù hợp hơn
- Ba tham số chính: **temperature**, **top-k**, và **top-p**


### Temperature - Núm Điều chỉnh Sáng tạo

Temperature là thiết lập phổ biến và có tác động lớn nhất:

#### Nhiệt độ Cao (High Temperature)

- **Tác dụng**: Tạo ra phản hồi sáng tạo và bất ngờ hơn
- **Ứng dụng**: Phù hợp cho các tác vụ nghệ thuật như động não ý tưởng hoặc viết truyện ngắn


#### Nhiệt độ Thấp (Low Temperature)

- **Tác dụng**: Tạo ra kết quả dự đoán được và nhất quán hơn
- **Ứng dụng**: Hữu ích cho các tác vụ yêu cầu phản hồi chính xác, thực tế như tóm tắt báo cáo hoặc tạo timeline


#### Ví dụ Minh họa

Với câu bắt đầu: "This morning, I went to the..."

- **Nhiệt độ thấp**: AI chọn từ có điểm số cao nhất, rõ ràng nhất → "grocery store"
- **Nhiệt độ cao**: AI có thể chọn từ bất ngờ hơn → "haunted house" hoặc "moon"


### Top-k và Top-p - Các Núm Điều chỉnh Tập trung

Hai thiết lập này hoạt động như **núm điều chỉnh tập trung** (focus dials), tạo ra danh sách từ nhỏ hơn và phù hợp hơn trước khi temperature đưa ra lựa chọn sáng tạo.

#### Top-k

- **Chức năng**: Đặt số lượng từ cố định mà công cụ có thể chọn
- **Ví dụ**: Thiết lập top-k = 10 → công cụ chỉ chọn từ trong top 10 tùy chọn có khả năng cao nhất


#### Top-p

- **Chức năng**: Đặt số lượng từ động mà công cụ có thể chọn
- **Cơ chế**: Tự động thu nhỏ hoặc mở rộng danh sách tùy chọn dựa trên độ dự đoán được của từ tiếp theo
- **Ví dụ**: Top-p cao (p=0.9) hoạt động như bộ lọc chất lượng, chỉ xem xét các lựa chọn có khả năng cao nhất


#### Sự Khác biệt Chính

- **Top-k**: Sử dụng danh sách lựa chọn kích thước cố định
- **Top-p**: Sử dụng danh sách lựa chọn kích thước linh hoạt

**Mẹo**: Khi sử dụng top-p, nên để top-k ở thiết lập mặc định.

### Công thức Thành công

#### Công thức 1: Phân tích Tập trung (Focused Analysis)

**Mục tiêu**: Tạo ra câu trả lời thực tế, nhất quán và dự đoán được

**Ứng dụng**:

- Tóm tắt báo cáo
- Trích xuất insights từ dữ liệu
- Viết tài liệu kỹ thuật
- Tạo code

**Thiết lập**:

- **Temperature**: Thấp (0.1 đến 0.4)
- **Top-k hoặc Top-p**: Để mặc định vì temperature thấp đã làm cho kết quả rất tập trung


#### Công thức 2: Động não Sáng tạo (Creative Brainstorming)

**Mục tiêu**: Tạo ra kết quả bất ngờ, đa dạng và sáng tạo

**Ứng dụng**:

- Động não ý tưởng mới
- Soạn thảo tài liệu marketing
- Viết truyện hư cấu

**Thiết lập**:

- **Temperature**: Cao (0.8 đến 1.0)
- **Top-k hoặc Top-p**: Giá trị cao (như 0.95 cho top-p) để cho AI tự do sáng tạo nhưng vẫn lọc bỏ các tùy chọn không liên quan


### Ghi chú Quan trọng

**Cảnh báo về Hallucinations**:

- Điểm số cao có thể tạo ra insights bất ngờ
- Nhưng cũng tăng khả năng tạo ra thông tin không chính xác hoặc ảo giác (hallucinations)
- **Luôn xem xét và kiểm tra thực tế** kết quả đầu ra, đặc biệt khi sử dụng cấu hình sáng tạo

**Nguyên tắc Cân bằng**:

- Prompt tốt chỉ là điểm khởi đầu, không phải đích đến
- Chìa khóa là tìm ra sự cân bằng phù hợp giữa câu trả lời sáng tạo và dự đoán được
- Temperature là núm điều chỉnh sáng tạo, trong khi top-p và top-k giúp giữ cho sự sáng tạo đó tập trung

**Liên kết:** [[Generative AI]], [[AI Prompting]], [[Temperature]], [[Sampling Parameters]], [[Hallucinations]], [[Google AI Studio]]

