## Cải thiện chất lượng đầu ra bằng phương pháp điều chỉnh Prompt (Iteration)

Ngay cả khi sử dụng khung mẫu prompting chuẩn, đôi khi kết quả nhận được từ công cụ Generative AI (Gen AI) vẫn chưa đạt yêu cầu. Lúc này, bạn cần điều chỉnh lại prompt (iteration) để làm rõ hơn và cải thiện kết quả đầu ra.

**Điều chỉnh Prompt hiệu quả nhất là thực hiện ngay trong cùng một cuộc trò chuyện (chat), để AI có thể tận dụng thông tin đã được cung cấp trước đó.**

### Ví dụ minh họa ban đầu:

Prompt chung chung:

> “Identify the latest developments in the restaurant industry.”

Prompt này có thể tạo ra các kết quả rất rộng và thiếu trọng tâm. Để cải thiện, hãy thử các phương pháp iteration sau:

---

### 1. Xem lại và bổ sung chi tiết theo khung mẫu prompting:

Bổ sung rõ ràng hơn về **nhiệm vụ (task)**, **persona**, **format**, thêm đầy đủ **ngữ cảnh (context)** và **tài liệu tham khảo (references)**.

**Ví dụ cải thiện:**

> “Create a bulleted list including the latest developments in the restaurant industry specific to urban areas that could impact the public reception of a dining experience using only ingredients native to the region.”

---

### 2. Chia prompt thành các câu nhỏ hơn:

Thay vì đưa ra một prompt dài và phức tạp, hãy tách ra từng bước nhỏ rõ ràng hơn:

- **Prompt 1:** “Create a bulleted list including the latest developments in the restaurant industry.”
    
- **Prompt 2:** “Summarize the trends that would specifically impact restaurants in urban areas.”
    
- **Prompt 3:** “Write a pros and cons list on how those developments could impact the public reception of a dining experience using only ingredients native to the region.”
    

Việc chia nhỏ giúp AI dễ hiểu và dễ tập trung vào từng nhiệm vụ hơn.

---

### 3. Thay đổi cách diễn đạt hoặc chuyển sang nhiệm vụ tương tự (analogous task):

Hãy đổi cách diễn đạt prompt để AI tiếp cận vấn đề theo góc nhìn mới, giúp tạo ra kết quả sáng tạo hơn:

**Ví dụ:**

> “I’m starting a restaurant that will only include produce from within 50 miles. You’re a diner that lives in a major city and keeps up with the latest restaurant trends. Write a list of questions that I should consider before opening up the restaurant.”

---

### 4. Thêm ràng buộc cụ thể (constraints):

Thêm vào các giới hạn về nội dung, định dạng, độ dài hoặc yếu tố cụ thể để tập trung kết quả đầu ra của AI:

**Ví dụ:**

> “Create a bulleted list including the latest developments in the restaurant industry specific to urban areas that could impact the public reception of a dining experience using only ingredients native to the region. This list should only include trends from cities with a population of more than 500,000 people, and should only include trends relevant to vegetarian and vegan restaurants.”

Các constraints giúp tạo ra kết quả rõ ràng, sáng tạo và sát mục tiêu hơn.

---

### Tóm tắt 4 phương pháp điều chỉnh prompt:

1. **Bổ sung chi tiết theo khung mẫu prompting** (task, persona, format, context, references).
    
2. **Chia prompt dài thành các prompt nhỏ gọn** để từng bước rõ ràng hơn.
    
3. **Thay đổi cách diễn đạt hoặc nhiệm vụ tương tự** để AI sáng tạo hơn.
    
4. **Thêm các ràng buộc cụ thể (constraints)** để AI tập trung vào kết quả mong muốn.
    

Luôn nhớ: **Iterate (điều chỉnh liên tục)** là chìa khóa giúp bạn tối ưu hóa prompt và nhận được kết quả đầu ra như mong đợi.