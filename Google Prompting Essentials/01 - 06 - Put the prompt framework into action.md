## Thực hành sử dụng khung mẫu tạo Prompt hiệu quả với Gemini

**Ví dụ minh họa:** Tạo prompt để lên ý tưởng cho dòng sản phẩm giày thể thao hiệu năng cao mới.

### Bước 1: Đăng nhập và đặt nhiệm vụ (Task)

Ban đầu prompt chỉ gồm nhiệm vụ chung chung:

> _“Generate five ideas for a new high-performance sneaker line.”_  
> _(Tạo 5 ý tưởng cho dòng giày thể thao hiệu năng cao mới.)_

- Prompt này chỉ có **nhiệm vụ (Task)** mà thiếu các yếu tố khác trong khung mẫu.
    
- Kết quả đầu ra của Gemini sẽ rất rộng và không cụ thể.
    

Gemini vẫn đưa ra 5 ý tưởng với tên và mô tả, nhưng ta vẫn có thể cải thiện prompt để nhận được kết quả hữu ích hơn.

### Bước 2: Bổ sung chi tiết về định dạng (Format) vào nhiệm vụ

Thêm rõ yêu cầu về định dạng và nội dung cụ thể hơn vào nhiệm vụ:

> _“List the concepts and materials for each sneaker in an outline.”_  
> _(Liệt kê ý tưởng và vật liệu cho từng mẫu giày theo dạng outline.)_

- Gemini lúc này tạo ra các ý tưởng giày chi tiết hơn, bao gồm cả vật liệu, đồng thời đáp ứng đúng định dạng yêu cầu.
    
- Prompt này tốt hơn, nhưng vẫn có thể tiếp tục tối ưu thêm.
    

### Bước 3: Bổ sung ngữ cảnh (Context)

Thêm thông tin cụ thể hơn về mục đích sử dụng giày:

> _“The sneakers should be made for athletes doing cross-training activities.”_  
> _(Các mẫu giày phải phù hợp cho vận động viên thực hiện các hoạt động tập luyện tổng hợp.)_

- Kết quả nhận được sau khi bổ sung ngữ cảnh rõ ràng sẽ phù hợp và sát với nhu cầu hơn rất nhiều.
    
- Prompt càng cụ thể, kết quả đầu ra càng sát với mục đích.
    

**→ Lưu ý:**  
Muốn kết quả đầu ra cụ thể và hữu ích hơn, luôn bổ sung đầy đủ chi tiết và ngữ cảnh.

### Bước 4: Sử dụng tài liệu tham khảo (References)

- Tham khảo (references) là những **ví dụ** để AI dựa vào khi tạo đầu ra.
    
- References giúp AI hiểu rõ hơn về phong cách, độ dài, hoặc ngôn ngữ của nội dung cần tạo.
    
- Việc cung cấp nhiều tài liệu tham khảo (2-5 ví dụ) còn được gọi là **few-shot prompting**:
    
    - **Few-shot prompting:** dùng một vài ví dụ làm tài liệu tham khảo.
        
    - **Single-shot prompting:** chỉ dùng một ví dụ tham khảo.
        
    - **Zero-shot prompting:** không cung cấp ví dụ nào cả.
        

#### Áp dụng Few-shot prompting vào ví dụ tạo sneaker mới:

- Đưa ra **hai ví dụ giày hiện có** để AI tham khảo:
    
    - Một đôi giày giá rẻ (budget line).
        
    - Một đôi giày công nghệ cao với đế thích ứng (adaptive sole).
        

Prompt mới:

> _“Keep the five ideas generated, but refine them using these two examples as references.”_  
> _(Giữ 5 ý tưởng đã tạo, nhưng hãy tinh chỉnh chúng dựa trên hai ví dụ tham khảo này.)_

- Gemini sẽ cho ra kết quả sáng tạo hơn nhưng đồng thời dựa trên phong cách và đặc điểm của những mẫu giày đã cung cấp.
    

### Bước 5: Đánh giá (Evaluate) và Điều chỉnh lặp lại (Iterate)

- **Evaluate (đánh giá)** giúp xem xét kết quả đầu ra đã đáp ứng đủ yêu cầu chưa.
    
- **Iterate (điều chỉnh)** cho phép bổ sung hoặc điều chỉnh prompt nhằm cải thiện chất lượng kết quả đầu ra.
    

**Ví dụ về cách đánh giá và điều chỉnh:**

- Lần đầu prompt quá rộng → bổ sung **Format** → kết quả tốt hơn.
    
- Đánh giá lại kết quả vẫn chưa sát nhu cầu → bổ sung thêm **Context**.
    
- Muốn cải thiện thêm nữa → cung cấp thêm **References**.
    

Quá trình này có thể lặp đi lặp lại cho đến khi nhận được kết quả mong muốn.

---

## Tổng kết các lưu ý khi sử dụng framework tạo Prompt hiệu quả:

- Luôn bắt đầu với prompt đơn giản, sau đó tăng dần độ phức tạp và chi tiết.
    
- Nếu kết quả trở nên kém chất lượng, hãy quay lại làm prompt đơn giản hơn.
    
- Luôn nhớ nguyên tắc cốt lõi:  
    **Thoughtfully Create Really Excellent Inputs**  
    _(Tạo ra những đầu vào thật chu đáo và xuất sắc.)_
    
- Luôn chủ động **đánh giá và lặp lại (evaluate and iterate)**. Điều này giúp điều chỉnh từng bước prompt để đạt kết quả tối ưu.
    
- Quá trình tạo prompt là liên tục thử nghiệm, sáng tạo, học hỏi từ những gì hiệu quả và những gì không.
    

**Ghi nhớ khẩu hiệu:**  
**“Always Be Iterating” (Luôn luôn điều chỉnh, lặp lại để hoàn thiện).**

---