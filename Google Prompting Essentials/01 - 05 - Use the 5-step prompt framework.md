# Framework 5 bước cho Prompting hiệu quả

> 🔗 **Navigation**: [[01 - 04 - Course overview|⬅️ Bài trước]] | [[01 - 06 - Put the prompt framework into action|➡️ Bài tiếp theo]] | [[MOC - Google Prompting Essentials|📋 Tổng quan]]

Để tạo một [[Glossary - Thuật ngữ Gen AI#Prompt|**prompt**]] hiệu quả, ta nên tuân theo một **[[Glossary - Thuật ngữ Gen AI#Framework|khung mẫu]] đơn giản** bao gồm 5 bước:

**Task → Context → References → Evaluate → Iterate**

- Nếu quên thứ tự các bước, bạn có thể nhớ cụm:  
   **Thoughtfully Create Really Excellent Inputs**

## Giải thích cụ thể từng bước trong khung mẫu tạo Prompt:

### 1. Xác định nhiệm vụ (**Task**)

- **Mô tả rõ ràng nhiệm vụ cụ thể** mà bạn muốn công cụ [[Glossary - Thuật ngữ Gen AI#Gen AI|trí tuệ nhân tạo tạo sinh (Generative AI)]] hỗ trợ.
- Khi mô tả nhiệm vụ, cần đề cập thêm:
  - **[[Glossary - Thuật ngữ Gen AI#Persona|Persona]]**: vai trò hoặc kinh nghiệm mà bạn muốn AI đóng vai khi tạo nội dung.
    - Ví dụ: "Một người viết diễn văn chuyên nghiệp" (professional speech writer), hoặc "Giám đốc marketing có 15 năm kinh nghiệm" (marketing executive with 15 years of experience).
    - Bạn cũng có thể chỉ định **đối tượng nhận thông tin** cụ thể như "khách hàng" (customer), hay "cấp quản lý của bạn" (your manager).
  - **Format**: hình thức bạn muốn nhận kết quả đầu ra.
    - Ví dụ: danh sách gạch đầu dòng (bulleted list), câu ngắn (short sentences), bảng (table).

**Ví dụ:**  
Thay vì nói chung chung:

> "Give me some ideas for a birthday present under $30."

Hãy viết rõ ràng và cụ thể hơn:

> "Give me five ideas for a birthday present. My budget is $30. The gift is for a 29-year-old who loves winter sports and has recently switched from snowboarding to skiing."

---

### 2. Cung cấp ngữ cảnh (**[[Glossary - Thuật ngữ Gen AI#Context|Context]]**)

- Đưa vào prompt những **chi tiết quan trọng, cụ thể** để giúp công cụ Generative AI hiểu rõ chính xác yêu cầu của bạn.
- Ngữ cảnh rõ ràng sẽ giúp kết quả thu được chính xác và hữu ích hơn → [[01 - 07 - AI IRL - Improve your prompts by adding context and persona|Tìm hiểu thêm]]

---

### 3. Bổ sung tài liệu tham khảo (**[[Glossary - Thuật ngữ Gen AI#References|References]]**)

- Nếu có thể, hãy cung cấp thêm **ví dụ, tài liệu tham khảo, dữ kiện liên quan** vào prompt.
- Điều này giúp AI tạo ra kết quả phù hợp và sát với yêu cầu cụ thể hơn.
- Tuy nhiên, không phải lúc nào bạn cũng có sẵn thông tin tham khảo rõ ràng, đặc biệt khi làm việc với các chủ đề trừu tượng hay tìm kiếm ý tưởng mới.

**Ví dụ:**  
Bạn muốn AI gợi ý món quà sinh nhật phù hợp, hãy cung cấp những món quà bạn đã từng tặng trước đây để AI hiểu rõ sở thích và phong cách cá nhân hơn.

---

### 4. Đánh giá kết quả đầu ra (**Evaluate**)

- Sau khi nhận được kết quả, hãy **đánh giá kỹ càng** xem:
  - Prompt đã đưa vào có tạo ra được kết quả như mong muốn chưa?
  - Kết quả nhận được đã đáp ứng đầy đủ, rõ ràng yêu cầu đặt ra hay chưa?

---

### 5. Điều chỉnh và lặp lại (**[[Glossary - Thuật ngữ Gen AI#Iteration|Iterate]]**)

- Nếu kết quả thu được chưa đúng như kỳ vọng, hãy tiếp tục:
  - **Điều chỉnh prompt**, thêm bớt chi tiết, thông tin cụ thể hơn.
  - **Thử lại (iterate)** nhiều lần đến khi nhận được kết quả mong muốn → [[01 - 09 - Practice 4 iteration methods|Học 4 phương pháp iteration]]
- Đây chính là một bước then chốt trong việc tạo prompt hiệu quả, và sẽ được khai thác kỹ hơn trong các bài học tiếp theo.

---

## Một số lưu ý thêm về khung mẫu tạo prompt hiệu quả:

- Có nhiều cách thức khác nhau để xây dựng một prompt hiệu quả.
- Thứ tự các bước trong prompt **không quan trọng bằng chất lượng nội dung** mà bạn đưa vào prompt.

---

> 📚 **Bài học liên quan**:
>
> - [[01 - 06 - Put the prompt framework into action|Thực hành framework]]
> - [[01 - 08 - Get the most out of AI with the prompt framework|Tối ưu hóa framework]]
> - [[01 - 09 - Practice 4 iteration methods|4 phương pháp iteration]]

- Chỉ cần bạn tuân thủ nguyên tắc:  
   **Thoughtfully Create Really Excellent Inputs**  
   (tạm dịch: Tạo đầu vào một cách chu đáo và xuất sắc),  
   bạn sẽ thu được kết quả đầu ra chất lượng cao.
