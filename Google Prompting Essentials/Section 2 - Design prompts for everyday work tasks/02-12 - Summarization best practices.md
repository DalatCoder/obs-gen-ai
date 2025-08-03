## Phương pháp tốt nhất để tóm tắt với AI tạo sinh (Summarization Best Practices)

### Tình huống ứng dụng

**Các trường hợp thường gặp:**

- Cần trích xuất insight (hiểu biết) từ tài liệu khổng lồ
- Gặp chuỗi email siêu dài khó nắm bắt nội dung chính
- Muốn tiết kiệm thời gian xử lý thông tin phức tạp

**Tin tốt:** Công cụ AI tạo sinh rất giỏi tóm tắt thông tin và tiết kiệm thời gian.

### Nguyên lý hoạt động của AI trong tóm tắt

**Pattern Recognition (Nhận dạng mẫu):**

- Công cụ AI tạo sinh sử dụng nhận dạng mẫu để phân tích chuỗi văn bản
- Tinh chỉnh chúng thành các bản tóm tắt ngắn hơn

**Yêu cầu quan trọng:** Tạo prompt mạnh mẽ với các thông số cụ thể về những gì cần có trong bản tóm tắt.

### Các phương pháp tốt nhất trong Prompting Framework

#### Task (Nhiệm vụ)

**Chỉ định nội dung cần tóm tắt:**

- Phần cụ thể của tài liệu
- Chủ đề phụ (sub topic) cụ thể

**Định dạng mong muốn:**

- Gạch đầu dòng (bullet points)
- Độ dài cụ thể
- Tone (giọng điệu) của bản tóm tắt

**Persona (Nhân vật):**

- Yêu cầu đầu ra phù hợp với trình độ đọc hiểu lớp 9
- Hoặc các đối tượng cụ thể khác


#### Context (Ngữ cảnh)

**Thêm ngữ cảnh bổ sung:**

- Bản tóm tắt dành cho mục đích gì
- Tại sao tạo ra bản tóm tắt này
- Giúp công cụ AI neo (anchor) phản hồi vào thứ gì đó cụ thể


#### References (Tham chiếu)

**Khi có bản tóm tắt mẫu:**

- Thêm cả bản tóm tắt mẫu và tài liệu gốc được tóm tắt
- Giúp công cụ hiểu cách tiếp cận cần thực hiện


#### Evaluate (Đánh giá)

**Rủi ro khi xử lý lượng lớn văn bản:**

- Tăng khả năng diễn giải sai
- Chuỗi suy nghĩ không liên quan
- **Hallucination (Ảo giác)** - tạo thông tin không có trong nguồn gốc

**Cách đánh giá:**

- Dựa trên nhiệm vụ đã đặt ra
- Tham chiếu chéo (cross-reference) đầu ra
- Nhờ chuyên gia đánh giá nếu có thể


#### Iterate (Lặp lại)

**Khi không nhận được bản tóm tắt hữu ích:**

- Yêu cầu điều chỉnh định dạng
- Thay đổi độ dài
- Chỉnh sửa chi tiết cụ thể không phù hợp

**Nguyên tắc:** Tiếp tục lặp lại cho đến khi nhận được bản tóm tắt phục vụ mục đích.

### Long Context 101 - Ngữ cảnh dài cơ bản

#### AI Model và Token Limit (Giới hạn token)

**Tokens (Token):**

- Khối xây dựng cơ bản của văn bản mà mô hình AI sử dụng để xử lý và hiểu ngôn ngữ
- Có thể nhỏ như một ký tự, một phần của từ, hoặc thậm chí nhiều từ
- **Ví dụ minh họa:** Nếu xây nhà bằng gạch, mỗi viên gạch là một token trong quá trình xây dựng

**Quá trình xử lý:**

- Khi cung cấp prompt cho công cụ AI, nó chia nhỏ thành các token
- Prompt càng dài, càng cần nhiều token để tạo đầu ra

**Sự phát triển của Token Limit:**

- Mô hình AI ban đầu: chỉ xử lý vài nghìn token cùng lúc
- Mô hình hiện tại: có thể xử lý hàng triệu token
- **Quan trọng:** Hiểu rõ mô hình AI đang sử dụng và giới hạn token của nó


#### Long Context Windows (Cửa sổ ngữ cảnh dài)

**Khái niệm:**

- Cho phép công cụ AI tạo sinh xử lý lượng lớn thông tin (nhiều token hơn) với nhiều định dạng khác nhau cùng lúc
- Có thể chia sẻ nhiều ngữ cảnh và thông tin nền hơn trong đầu vào

**Lợi ích chính:**

**1. Xử lý tác vụ phức tạp:**

- Tạo chiến dịch marketing nhiều phần
- Lập kế hoạch kinh doanh chi tiết
- Xử lý các nhiệm vụ có nhiều chi tiết tinh tế

**2. Phản hồi toàn diện hơn:**

- Hiểu và tạo ra các phản hồi toàn diện, cá nhân hóa và liên quan hơn
- **Ví dụ:** Xử lý báo cáo PDF dài với hàng chục trang, đồ thị và minh họa trong một đầu vào duy nhất

**3. Tiết kiệm thời gian:**

- Loại bỏ nhu cầu chia nhỏ văn bản hoặc thông tin thành các phần nhỏ hơn khi thiết kế prompt


#### Working Memory (Bộ nhớ làm việc)

**Vấn đề với việc nhớ:**

- Giống như con người có thể quên những gì đã đặt ăn tuần trước hoặc tên ai đó giữa cuộc trò chuyện
- Việc gợi lại chi tiết quá khứ cũng khó khăn đối với công cụ AI tạo sinh

**Giải pháp với Long Context Windows:**

- Hoạt động như bộ nhớ làm việc cho công cụ AI tạo sinh
- Giúp chúng nhớ những gì đã chia sẻ trước đó trong cùng chuỗi cuộc trò chuyện
- **Ví dụ so sánh:** Như nói chuyện với người đã quen biết vấn đề bạn cố gắng giải quyết thay vì giải thích tình huống với người lạ không có ngữ cảnh


### Lưu ý quan trọng

**Giới hạn của bộ nhớ:**

- Hầu hết công cụ AI tạo sinh chỉ nhớ những gì bạn đặt trong long context window trong cùng conversation thread (chuỗi cuộc trò chuyện) hoặc prompt chain (chuỗi prompt)
- Nếu đóng cửa sổ và mở lại, công cụ sẽ không nhớ
- Cần nhập lại tài liệu trước khi công cụ có thể cung cấp đầu ra liên quan


### Ghi chú thêm

**Ứng dụng thực tế:**

- Xử lý tài liệu nghiên cứu dài
- Tóm tắt báo cáo kinh doanh phức tạp
- Phân tích chuỗi email dài
- Tạo bản tóm tắt từ nhiều nguồn thông tin

**Xu hướng phát triển:**

- Công cụ AI tạo sinh liên tục cải thiện
- Khả năng xử lý các đoạn văn bản và dữ liệu lớn hơn nhiều trong một đầu vào duy nhất
- Nhà phát triển tìm cách tăng giới hạn token → công cụ AI tạo sinh ngày càng có khả năng xử lý lượng dữ liệu lớn hơn

**Liên kết:** [[Generative AI]], [[Summarization]], [[Long Context Window]], [[Token Limit]], [[Prompting Framework]], [[Pattern Recognition]], [[Hallucination]], [[Working Memory]], [[AI Model]], [[Context]], [[Evaluation]], [[Iteration]]

