## Hiểu về Multimodal Prompting

### Khái niệm cơ bản

**[[Multimodal Prompting]]** (prompt đa phương tiện) là thuật ngữ lớn với ý nghĩa đơn giản:

- **[[Modalities]]** (phương thức): các loại định dạng khác nhau như text (văn bản), image (hình ảnh), audio (âm thanh) dùng để hướng dẫn công cụ AI sinh tạo
- **Multimodal prompting**: sử dụng nhiều modalities trong cùng một prompt

**Ví dụ ứng dụng:**

- Dịch hình ảnh thành mô tả văn bản chi tiết cho người khiếm thị
- Tạo đồ họa dựa trên đoạn ghi âm mô tả chiến dịch marketing


### Lợi ích và ý nghĩa

**Phản ánh thế giới thực:**

- Thế giới là đa phương tiện (multimodal)
- Khi thuyết trình: sử dụng văn bản, hình ảnh, giọng nói để truyền đạt ý tưởng
- [[Multimodal prompting]] hoạt động tương tự: xây dựng kết nối giữa text, images, audio và các modalities khác

**Cải thiện chất lượng prompt:**

- Không phải giải pháp "một size cho tất cả"
- **Ví dụ:** Yêu cầu viết thơ về hoàng hôn + đính kèm ảnh hoàng hôn → AI sử dụng ảnh để mô tả màu sắc và chi tiết cụ thể → bài thơ sống động hơn


### Hạn chế cần lưu ý

**Những khó khăn của công cụ AI sinh tạo:**

- Khó xử lý ý tưởng trừu tượng
- Gặp thách thức với sự kết hợp phức tạp của nhiều modalities
- Đôi khi thiếu common sense (lẽ thường)
- **Chưa đáng tin cậy** cho việc đếm số lượng


### Ví dụ ứng dụng thực tế

**1. Gợi ý công thức nấu ăn:**

```
Gửi ảnh nguyên liệu trong tủ lạnh → AI gợi ý công thức dựa trên ảnh
```

**2. Tạo teaser digital cho sự kiện:**

```
Input: Logo và màu sắc của 2 thương hiệu
Output: Hình ảnh quảng cáo cho sự kiện chung
```

**3. Hỗ trợ viết truyện ngắn:**

```
Input: File âm thanh ghi lại âm thanh rừng
Prompt: Sử dụng âm thanh này để tạo cảm hứng cho bầu không khí và chi tiết câu chuyện
```


### Áp dụng khung Prompting Framework

Vẫn dựa trên **[[TCREI Framework]]**: Thoughtfully Create Really Excellent Inputs, nhưng có điều chỉnh:

**Task (Nhiệm vụ):**

- Cụ thể về persona và format
- **Rõ ràng về cách sử dụng các modalities khác nhau**
- **Giải thích lý do đưa chúng vào task**

**Context (Bối cảnh):**

- Cung cấp context để AI biết chính xác điều cần làm
- Cân nhắc modalities đang sử dụng khi cung cấp context
- **Ví dụ:** Ảnh tủ lạnh → chỉ muốn AI xem xét trái cây và rau củ, không phải đồ đóng gói

**References (Tài liệu tham khảo):**

- Chia sẻ tài liệu tham khảo dạng văn bản, hình ảnh, âm thanh
- **Lưu ý:** Không phải công cụ nào cũng hỗ trợ mọi loại reference

**Evaluate (Đánh giá):**

- Chạy prompt như thường lệ
- **Đặc biệt chú ý** đánh giá output trông như thế nào hoặc đọc ra sao
- Review chi tiết hơn so với chỉ đánh giá phản hồi văn bản

**Iterate (Lặp lại):**
Nếu output không đáp ứng nhu cầu, thử 4 phương pháp iteration:

- Quay lại prompting framework
- Chia prompt thành các task ngắn hơn
- Đưa ra constraints (ràng buộc)
- Điều chỉnh cách diễn đạt hoặc chuyển sang analogous task (nhiệm vụ tương tự)


### Kết luận

**[[Multimodal prompting]]** là công cụ mạnh mẽ cho phép:

- Chuyển đổi thông tin giữa các phương tiện khác nhau
- Tạo ra khả năng output vô hạn
- **Bạn là nghệ sĩ, công cụ AI sinh tạo là cọ vẽ của bạn**

**Liên kết:** [[Multimodal Prompting]], [[Modalities]], [[TCREI Framework]], [[AI Output Evaluation]], [[Iteration]], [[Visual Communication]], [[Audio Processing]]

