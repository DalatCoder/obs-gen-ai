# 4 Phương pháp điều chỉnh Prompt hiệu quả (Iteration Methods)

> 🔗 **Navigation**: [[01 - 08 - Get the most out of AI with the prompt framework|⬅️ Bài trước]] | [[01 - 10 - Generate better outputs through iteration|➡️ Bài tiếp theo]] | [[MOC - Google Prompting Essentials|📋 Tổng quan]]

Khi [[Glossary - Thuật ngữ Gen AI#Prompt|prompt]] chưa cho kết quả mong muốn, không nhất thiết phải bỏ toàn bộ công sức và bắt đầu lại từ đầu. Thay vào đó, hãy nhớ nguyên tắc **[[Glossary - Thuật ngữ Gen AI#ABI|ABI (Always Be Iterating)]]** – luôn luôn điều chỉnh và cải thiện từng bước một.

### **Có 4 phương pháp điều chỉnh prompt chính:**

### 1. Quay lại [[01 - 05 - Use the 5-step prompt framework|framework]] và bổ sung thêm chi tiết

Hãy đảm bảo prompt của bạn đủ **cụ thể và chi tiết** ở các yếu tố:

- **Nhiệm vụ (Task)**
- **Ngữ cảnh ([[Glossary - Thuật ngữ Gen AI#Context|Context]])**
- **Tài liệu tham khảo ([[Glossary - Thuật ngữ Gen AI#References|References]])**

**Ví dụ trước khi điều chỉnh:**

> “Give me five blog post ideas.” (Cho tôi 5 ý tưởng bài blog.)

**Ví dụ sau khi điều chỉnh:**

> “You are an expert on sports nutrition. Provide five blog post headlines that summarize the biggest trends happening in the industry for an audience of physical therapists working with professional basketball players.”  
> _(Bạn là chuyên gia dinh dưỡng thể thao. Cung cấp 5 tiêu đề bài blog nói về các xu hướng lớn nhất trong lĩnh vực này, dành cho đối tượng là các nhà vật lý trị liệu làm việc với cầu thủ bóng rổ chuyên nghiệp.)_

### 2. Chia nhỏ prompt thành các câu ngắn

Thay vì viết một prompt dài gồm nhiều nhiệm vụ cùng lúc, hãy chia thành nhiều prompt nhỏ hơn:

**Prompt dài ban đầu:**

> “Summarize the key data points and information in this report, then create visual graphs from the data, and shorten the key information into bullets.”

**Chia thành các prompt nhỏ hơn:**

- Prompt 1: “Summarize the key data points and information in this report.” (Tổng hợp các điểm dữ liệu quan trọng trong báo cáo.)
- Prompt 2: “Create visual graphs with the data you summarized.” (Tạo biểu đồ trực quan từ dữ liệu vừa tóm tắt.)
- Prompt 3: “Shorten the key information you summarized into bullets.” (Rút gọn thông tin quan trọng thành dạng gạch đầu dòng.)

Kết quả của từng bước nhỏ này thường chính xác hơn vì Gen AI dễ dàng xử lý một nhiệm vụ cụ thể mỗi lần.

### 3. Thay đổi cách diễn đạt hoặc chuyển sang một nhiệm vụ tương tự (Analogous task)

Khi kết quả chưa tốt, thử thay đổi **cách diễn đạt hoặc nhiệm vụ tương tự nhưng theo góc nhìn khác**:

**Ví dụ:**  
Thay vì prompt gốc:

> “Write a marketing plan for this product/service.”  
> _(Viết một kế hoạch marketing cho sản phẩm/dịch vụ này.)_

Bạn có thể chuyển sang nhiệm vụ tương tự nhưng góc nhìn mới:

> “Write a story about how this product fits into the lives of our target customer demographic.”  
> _(Viết một câu chuyện về cách sản phẩm này phù hợp với cuộc sống khách hàng mục tiêu.)_

Việc thay đổi góc nhìn giúp Gen AI tạo ra kết quả sáng tạo và hữu ích hơn.

### 4. Thêm ràng buộc cụ thể (Constraints)

Nếu kết quả đầu ra quá chung chung hoặc không mới mẻ, hãy thêm vào những **giới hạn cụ thể** để hướng AI đến kết quả sáng tạo hơn:

**Ví dụ ban đầu (thiếu constraints):**

> “Create a playlist for my upcoming road trip.”  
> _(Tạo playlist cho chuyến đi sắp tới.)_

**Ví dụ sau khi thêm constraints:**

> “Create a playlist for my upcoming road trip, include only artists from the Pacific Northwest who released music in the last five years.”  
> _(Tạo playlist cho chuyến đi sắp tới, chỉ chọn các nghệ sĩ từ vùng Pacific Northwest và có sản phẩm mới phát hành trong vòng 5 năm gần đây.)_

Các constraints này giúp AI tạo ra kết quả sáng tạo, độc đáo, sát với sở thích và yêu cầu của bạn hơn.

---

### Tóm tắt nhanh các phương pháp [[Glossary - Thuật ngữ Gen AI#Iteration|Iteration]] hiệu quả:

| Phương pháp                          | Tác dụng                                                |
| ------------------------------------ | ------------------------------------------------------- |
| Thêm chi tiết vào prompt             | Kết quả đầu ra cụ thể, sát hơn với mong muốn.           |
| Chia nhỏ prompt thành nhiều câu ngắn | Kết quả chính xác, dễ theo dõi từng bước nhỏ.           |
| Thay đổi góc nhìn/nhiệm vụ tương tự  | Thúc đẩy sự sáng tạo, đa dạng hóa kết quả.              |
| Thêm các ràng buộc cụ thể            | Tập trung vào kết quả mới lạ, phù hợp sở thích cá nhân. |

---

> 📚 **Bài học liên quan**:
>
> - [[01 - 10 - Generate better outputs through iteration|Cải thiện kết quả qua iteration]]
> - [[01 - 11 - AI IRL - Iterate on your prompts to succeed|Thực hành iteration thành công]]
> - [[01 - 05 - Use the 5-step prompt framework|Framework 5 bước cơ bản]]

Luôn nhớ:  
**ABI (Always Be Iterating) – Luôn luôn điều chỉnh, cải thiện từng bước một.**
