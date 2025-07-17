## Khai thác tối ưu AI bằng khung mẫu tạo Prompt

Để khai thác hiệu quả nhất từ công cụ Generative AI (Gen AI), bạn cần hiểu rõ mối quan hệ giữa đầu vào (input - prompt) và đầu ra (output). Khung mẫu dưới đây giúp bạn tạo ra những prompt rõ ràng, cụ thể và hiệu quả:

**Thoughtfully Create Really Excellent Inputs**

**(Task → Context → References → Evaluate → Iterate)**

### 1. Xác định nhiệm vụ (Task)

Nhiệm vụ là yêu cầu cụ thể bạn muốn Gen AI thực hiện. Hãy viết rõ ràng, cụ thể để tránh hiểu nhầm.

- Nên thêm thông tin:
    
    - **Persona** (vai trò, chuyên môn cụ thể) như: chuyên gia khoa học, nhà phân tích thị trường, hướng tới người quản lý, nhóm làm việc.
        
    - **Format** (định dạng kết quả mong muốn) như: danh sách, bảng, đoạn văn ngắn, v.v.
        

**Ví dụ:**

> Bạn là nhà phê bình phim chuyên về điện ảnh Ý. Hãy tạo một bảng liệt kê các phim Ý xuất sắc nhất thập niên 1970, phân loại theo thể loại (giật gân, chính kịch, hài), kèm tóm tắt 100 từ cho mỗi phim, tên đạo diễn và năm phát hành.

### 2. Cung cấp ngữ cảnh cần thiết (Context)

Chi tiết càng đầy đủ, kết quả càng chính xác. Ngữ cảnh là các thông tin bổ sung giúp Gen AI hiểu rõ nhiệm vụ hơn, ví dụ như mục tiêu, lý do thực hiện hoặc trải nghiệm trước đây của bạn.

**Ví dụ:**

> Bạn là chuyên gia khoa học đang thiết kế chương trình giảng dạy mới tại trường cao đẳng địa phương. Hãy giải thích ngắn gọn và hấp dẫn về cách DNA được phát hiện và tác động của nó đối với thế giới, dành cho đối tượng không chuyên, với mục đích thu hút sinh viên.

**Mẹo nhỏ:** Context thường là phần dài nhất của một prompt. Có thể cung cấp các tài liệu có sẵn để tạo context nhanh chóng và hiệu quả.

### 3. Cung cấp tài liệu tham khảo (References)

References là các ví dụ cụ thể hoặc tài liệu tham khảo giúp Gen AI định hướng chính xác hơn khi tạo nội dung. Bạn có thể cung cấp tài liệu dưới dạng văn bản, hình ảnh hoặc âm thanh (tùy theo công cụ AI).

**Cách cấu trúc references hiệu quả:**

- **Sử dụng cụm từ chuyển tiếp**: “Tham khảo các tài liệu sau đây”, “Sử dụng ví dụ bên dưới”, v.v.
    
- **Tiêu đề rõ ràng**: dễ phân biệt các ví dụ khi cung cấp nhiều references.
    
- **Thẻ XML-style**: hữu ích khi cung cấp nhiều tài liệu phức tạp:
    

```
<example01>
Nội dung ví dụ thứ nhất
</example01>
```

- **Markdown tags** để giữ nguyên định dạng văn bản (ví dụ: `_in nghiêng_`, `**in đậm**`).
    

**Ví dụ prompt có references:**

> Viết đoạn mô tả sản phẩm cho một chiếc đồng hồ cao cấp chống trầy xước và chống nước đến 30 mét. Hãy dựa trên phong cách của các ví dụ sản phẩm dưới đây từ trang web:

**Kính râm:** Bộ sưu tập kính râm thủ công lấy cảm hứng cổ điển, với tròng kính chống tia UV, giá cả hợp lý.

**Ví đựng thẻ:** Làm từ da Ý cao cấp, thiết kế mỏng nhẹ, sản xuất tại Napoli.

(Lưu ý: thường chỉ cần 2-5 ví dụ tham khảo là đủ.)

### 4. Đánh giá đầu ra (Evaluate)

Do mỗi mô hình AI được huấn luyện trên dữ liệu khác nhau, nên cùng một prompt có thể tạo ra kết quả khác nhau mỗi lần chạy. Bạn cần luôn đánh giá xem kết quả thu được có chính xác, phù hợp, khách quan và nhất quán hay không.

- Nếu kết quả chưa như ý, bạn cần chuyển sang bước tiếp theo (Iterate).
    

### 5. Điều chỉnh và lặp lại (Iterate)

Luôn luôn điều chỉnh và cải tiến prompt nếu kết quả chưa đạt yêu cầu. Đây là quá trình lặp lại liên tục, giúp bạn nhận được kết quả tốt nhất.

- Phương pháp ABI (Always Be Iterating): luôn chủ động đánh giá và cải tiến cho đến khi hài lòng.
    

---

**Tóm tắt lại:**

- Xác định rõ nhiệm vụ (task), persona và format.
    
- Cung cấp đầy đủ ngữ cảnh (context).
    
- Thêm references rõ ràng và cụ thể.
    
- Đánh giá cẩn thận đầu ra.
    
- Liên tục điều chỉnh, cải thiện prompt (iterate).
    

Khung mẫu prompting này có thể áp dụng với mọi công cụ Gen AI.