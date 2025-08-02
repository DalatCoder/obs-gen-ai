## Cách Viết Prompt để Tạo ra Output Hữu ích

### Nguyên lý Cơ bản: Chất lượng Input = Chất lượng Output

**Quy luật chung:** Chất lượng của những gì bạn bắt đầu sẽ ảnh hưởng lớn đến chất lượng của những gì bạn tạo ra.

**Ví dụ minh họa - Nấu ăn:**

- **Nguyên liệu tươi, chất lượng cao** → Bữa ăn ngon
- **Thiếu nguyên liệu hoặc nguyên liệu kém chất lượng** → Bữa ăn không ngon

**Áp dụng cho AI:**

- **Prompt chất lượng cao** → Output hữu ích từ công cụ AI đối thoại
- **Prompt kém chất lượng** → Output không đáp ứng mong đợi


### Khái niệm Prompt Engineering

**Định nghĩa:** Prompt Engineering là quá trình thiết kế prompt tốt nhất có thể để nhận được output mong muốn từ LLM.

**Thành phần cốt lõi:**

- **Viết prompt rõ ràng, cụ thể** (clear, specific prompts)
- **Cung cấp ngữ cảnh liên quan** (relevant context)
- **Bao gồm thông tin cần thiết** để LLM hiểu đúng yêu cầu


### So sánh Con người vs LLM trong Xử lý Context

**Tình huống:** Một người ăn chay hỏi: "Tôi nên đi nhà hàng nào ở San Francisco?"


| Đối tượng | Phản hồi | Lý do |
| :-- | :-- | :-- |
| **Con người (bạn bè)** | Gợi ý nhà hàng có món chay ngon | Hiểu ngầm về thói quen ăn uống của người hỏi |
| **LLM** | Có thể gợi ý nhà hàng không phù hợp với người ăn chay | Không có kiến thức trước về người dùng |

**Bài học:** LLM cần prompt cụ thể: *"Gợi ý nhà hàng có món chay ngon ở San Francisco"*

### Ví dụ Thực tế: Lập Kế hoạch Sự kiện Công ty

**Tình huống:** Tìm chủ đề cho hội nghị sắp tới

#### Lần thử đầu tiên (Prompt kém)

```
Prompt: "Generate a list of five potential themes for an event"
```

**Kết quả:**

- Danh sách giống chủ đề tiệc tùng hơn là hội nghị chuyên nghiệp
- **Vấn đề:** Thiếu ngữ cảnh, không rõ ràng, không cụ thể


#### Lần thử thứ hai (Prompt cải thiện)

```
Prompt: "Generate a list of five potential themes for a professional conference on customer experience in the hospitality industry"
```

**Kết quả:**

- Danh sách phù hợp với hội nghị chuyên nghiệp
- **Thành công:** Prompt cụ thể, bao gồm ngữ cảnh liên quan

**So sánh:**

- **Prompt gốc:** Chung chung, thiếu context
- **Prompt cải thiện:** Cụ thể về loại sự kiện (professional conference), chủ đề (customer experience), ngành (hospitality industry)


### Quá trình Cải thiện Prompt

**Đặc điểm của Prompt Engineering:**

- **Quá trình lặp lại** (iterative process)
- **Thiết kế giống các lĩnh vực khác:** Cần điều chỉnh và cải thiện liên tục

**Quy trình thực tế:**

1. **Viết prompt đầu tiên**
2. **Đánh giá output**
3. **Phát hiện vấn đề** (thiếu context, không rõ ràng)
4. **Sửa đổi prompt** với thông tin cụ thể hơn
5. **Kiểm tra kết quả** và lặp lại nếu cần

**Nguyên tắc chính:** Khi cung cấp hướng dẫn rõ ràng, cụ thể bao gồm ngữ cảnh cần thiết, bạn cho phép LLM tạo ra output hữu ích.

### Hạn chế cần Lưu ý

**Giới hạn của LLM:**

- Có những trường hợp không thể tạo output chất lượng **dù prompt tốt**
- **Ví dụ:** Yêu cầu thông tin về sự kiện hiện tại mà LLM không có quyền truy cập

**Thực tế:**

- Ngay cả khi cung cấp hướng dẫn rõ ràng, cụ thể, bạn vẫn có thể không nhận được output mong muốn ở lần đầu
- **Giải pháp:** Tiếp tục điều chỉnh và cải thiện prompt


### Ghi chú Quan trọng

**Yếu tố then chốt:**

- **Rõ ràng (Clear):** Diễn đạt không gây nhầm lẫn
- **Cụ thể (Specific):** Bao gồm chi tiết cần thiết
- **Context phù hợp:** Cung cấp bối cảnh để LLM hiểu đúng

**Áp dụng rộng rãi:**

- Có thể sử dụng với Gemini, ChatGPT, Microsoft Copilot hoặc bất kỳ công cụ AI đối thoại nào khác

**Liên kết:** [[Prompt Engineering]], [[LLM]], [[Context]], [[Iterative Process]], [[Conversational AI]], [[Gemini]], [[ChatGPT]], [[Output Quality]]

