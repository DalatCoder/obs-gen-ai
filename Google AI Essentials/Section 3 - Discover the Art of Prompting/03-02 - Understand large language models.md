## Cách Hoạt Động và Hạn Chế của Mô Hình Ngôn Ngữ Lớn (Large Language Model)

### Khái niệm và Nguyên lý Hoạt động

**Mô hình ngôn ngữ lớn (Large Language Model - LLM)** là một mô hình AI được huấn luyện trên lượng văn bản khổng lồ để:

- Nhận diện các mẫu (patterns) giữa từ, khái niệm và cụm từ
- Tạo ra các phản hồi cho các yêu cầu (prompts)

**Quá trình huấn luyện:**

- LLM được huấn luyện trên hàng triệu nguồn văn bản: sách, bài báo, trang web
- Quá trình này giúp mô hình học các mẫu và mối quan hệ trong ngôn ngữ con người
- Nguyên tắc: Càng nhiều dữ liệu chất lượng cao, hiệu suất càng tốt


### Cơ chế Dự đoán Từ Tiếp theo

LLM có khả năng dự đoán từ có khả năng xuất hiện tiếp theo trong chuỗi từ bằng cách:

- Tính toán xác suất (probabilities) cho các từ có thể có
- Chọn từ có xác suất cao nhất hoặc một trong các từ có xác suất cao

**Ví dụ minh họa:**

```
Câu chưa hoàn chỉnh: "After it rained, the street was..."

Xác suất dự đoán:
- "wet" (ướt) → xác suất cao
- "clean" (sạch) → xác suất thấp hơn  
- "dry" (khô) → xác suất cực thấp

Kết quả: LLM chọn "wet" hoặc "damp" (ẩm ướt)
```

**Đặc điểm quan trọng:**

- LLM có thể cho kết quả khác nhau với cùng một prompt
- Sử dụng thống kê để phân tích mối quan hệ giữa tất cả từ trong chuỗi
- Tính toán xác suất cho hàng nghìn từ có thể xuất hiện tiếp theo


### Các Hạn chế Chính của LLM

#### 1. Thiên kiến trong Dữ liệu Huấn luyện (Training Data Bias)

- **Nguồn gốc:** Dữ liệu huấn luyện chứa thiên kiến từ các bài báo, trang web phản ánh thiên kiến xã hội
- **Biểu hiện:** LLM có thể liên kết nghề nghiệp với giới tính cụ thể
- **Hậu quả:** Đầu ra không công bằng và phản ánh định kiến


#### 2. Hạn chế về Phạm vi Kiến thức

- LLM có thể không tạo ra đủ nội dung về lĩnh vực/chủ đề cụ thể
- **Nguyên nhân:** Dữ liệu huấn luyện không chứa đủ thông tin về chủ đề đó


#### 3. Hiện tượng Ảo giác (Hallucination)

**Định nghĩa:** Ảo giác AI là các đầu ra không đúng sự thật

**Ví dụ thực tế:**

- Khi yêu cầu tóm tắt lịch sử công ty, LLM có thể:
    - Cung cấp ngày thành lập sai
    - Đưa ra số lượng nhân viên không chính xác

**Nguyên nhân gây ảo giác:**

- Chất lượng dữ liệu huấn luyện kém
- Cách diễn đạt prompt không phù hợp
- Phương pháp LLM sử dụng để phân tích văn bản và dự đoán từ tiếp theo


### Nguyên tắc Sử dụng Hiệu quả

#### Đánh giá Chỗt lượng Đầu ra

**Tiêu chí kiểm tra output của LLM:**

- **Tính chính xác:** Thông tin có đúng sự thật không?
- **Tính khách quan:** Có thiên kiến không?
- **Tính liên quan:** Có phù hợp với yêu cầu cụ thể không?
- **Tính đầy đủ:** Cung cấp đủ thông tin cần thiết không?


#### Lưu ý Quan trọng

- **Không đưa ra giả định** về khả năng của LLM
- Chất lượng output có thể khác nhau giữa các lần sử dụng cùng prompt
- **Luôn kiểm tra kỹ** chất lượng đầu ra cho mọi tác vụ:
    - Tóm tắt báo cáo dài
    - Tạo ý tưởng marketing
    - Phác thảo kế hoạch dự án


#### Kết luận

Mô hình ngôn ngữ lớn là công cụ mạnh mẽ nhưng **cần sự hướng dẫn của con người** để sử dụng hiệu quả. Hiểu rõ các hạn chế giúp đạt được kết quả tốt nhất có thể.

**Liên kết:** [[Large Language Model]], [[AI Hallucination]], [[Training Data]], [[Bias]], [[Prompt Engineering]], [[AI Output Evaluation]]

