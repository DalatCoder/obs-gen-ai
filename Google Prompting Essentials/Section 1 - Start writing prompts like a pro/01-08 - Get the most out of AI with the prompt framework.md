## Tối ưu hóa AI với khung prompt TCREI

### Khái niệm cốt lõi

[[Generative AI]] hoạt động dựa trên nguyên lý đầu vào (input) và đầu ra (output). Để sử dụng hiệu quả các công cụ AI sinh tạo, cần hiểu rõ:

- **Đầu ra mong muốn**: Kết quả bạn muốn nhận từ công cụ AI
- **Đầu vào phù hợp**: Loại prompt nào sẽ giúp đạt được kết quả đó


### Khung prompt TCREI

**Thoughtfully Create Really Excellent Inputs** = **Task, Context, References, Evaluate, Iterate**

Đây là khung làm việc đơn giản giúp cung cấp hướng dẫn rõ ràng và cụ thể cho bất kỳ công cụ AI sinh tạo nào.

### 1. Xác định nhiệm vụ (Task)

Nhiệm vụ là nền tảng của mọi prompt - đó là điều bạn yêu cầu công cụ AI thực hiện.

**Các ví dụ nhiệm vụ cơ bản:**

- Viết một danh sách
- Soạn thảo bài phát biểu
- Tạo hình ảnh

**Yêu cầu quan trọng:**

- Phải rõ ràng và cụ thể
- Tránh mơ hồ để không nhận được kết quả kém

**Bổ sung persona và định dạng:**

**Persona (Vai trò)**: Hướng dẫn AI rút kinh nghiệm từ lĩnh vực cụ thể

- Ví dụ: chuyên gia khoa học, nhà phân tích ngành, hướng đến đối tượng cụ thể

**Format (Định dạng)**: Cách thức trình bày kết quả

- Danh sách có dấu đầu dòng
- Bảng so sánh
- Đoạn văn mô tả

**Ví dụ prompt hoàn chỉnh:**

```
Bạn là một nhà phê bình phim chuyên về điện ảnh Ý. Tạo một bảng chứa những bộ phim Ý vĩ đại nhất của thập niên 1970, phân chia theo thể loại như phim kinh dị, chính kịch và hài kịch. Cung cấp tóm tắt 100 từ cho mỗi bộ phim cùng thông tin sản xuất bao gồm đạo diễn và năm phát hành.
```


### 2. Cung cấp bối cảnh (Context)

[[Context]] là thông tin nền giúp mô hình hiểu rõ hơn về yêu cầu của bạn.

**Các thành phần bối cảnh:**

- Mục tiêu của bạn
- Lý do thực hiện nhiệm vụ
- Những gì đã thử trước đó
- Thông tin nền liên quan

**Ví dụ so sánh:**

❌ **Prompt kém:** "DNA được khám phá như thế nào?"

✅ **Prompt tốt:**

```
Bạn là chuyên gia khoa học đang phát triển chương trình giảng dạy mới tại một trường cao đẳng địa phương. Hãy kể cho tôi trong vài đoạn văn hấp dẫn về cách DNA được khám phá và tác động của nó đến thế giới. Viết theo cách mà những người không quen thuộc với khoa học có thể hiểu được. Bạn đã nhận được phản hồi từ sinh viên rằng khóa học này trước đây khô khan và khó hiểu, vì vậy bạn muốn đảm bảo lời giải thích thu hút sự chú ý và tạo ấn tượng tốt.
```


### 3. Cung cấp tài liệu tham khảo (References)

[[References]] là các ví dụ hoặc tài nguyên bổ sung hướng dẫn AI tạo ra đầu ra mong muốn.

**Các loại tham khảo:**

- Văn bản
- Hình ảnh
- Âm thanh (tùy công cụ AI)

**Kỹ thuật cấu trúc tài liệu tham khảo:**

**1. Cụm từ chuyển tiếp:**

```
Tham khảo những tài liệu này...
Sử dụng các ví dụ sau...
```

**2. Tiêu đề phân loại:**

```
Viết mô tả sản phẩm một đoạn văn cho đồng hồ cao cấp... Dựa trên phong cách từ các ví dụ trên website:

Kính mát: Bộ sưu tập mới nhất...
Ví đựng thẻ: Được chế tác từ da Ý mềm mại...
```

**3. Thẻ XML:**

```
<example01>
[Văn bản ví dụ đầu tiên]
</example01>

<example02>
[Văn bản ví dụ thứ hai]
</example02>
```

**4. Thẻ Markdown:**

- `_text_` để in nghiêng
- `**text**` để in đậm

**Lưu ý:** 2-5 ví dụ tham khảo là đủ, không cần quá nhiều.

### 4. Đánh giá kết quả (Evaluate)

Các mô hình AI khác nhau được huấn luyện trên dữ liệu và kỹ thuật lập trình khác nhau, dẫn đến:

- Một số mô hình phù hợp với việc viết code
- Một số tốt cho brainstorming ý tưởng
- Cùng một prompt có thể cho kết quả khác nhau mỗi lần chạy

**Tiêu chí đánh giá đầu ra:**

- Tính chính xác (Accurate)
- Không thiên vị (Unbiased)
- Liên quan (Relevant)
- Nhất quán (Consistent)


### 5. Lặp lại và cải thiện (Iterate)

**Nguyên tắc ABI: Always Be Iterating**

Khi kết quả không đạt yêu cầu:

- Tiếp tục làm rõ những gì bạn cần
- Điều chỉnh prompt cho đến khi có kết quả phù hợp
- Không ngừng tối ưu hóa đầu vào


### Ứng dụng thực tiễn

Khung TCREI có thể áp dụng cho:

- Mọi loại công cụ AI sinh tạo
- Các mô hình AI khác nhau
- Đa dạng nhiệm vụ và mục đích sử dụng

**Quy trình thực hiện:**

1. Xác định rõ nhiệm vụ
2. Cung cấp bối cảnh chi tiết
3. Đưa ra tài liệu tham khảo
4. Đánh giá kết quả đầu ra
5. Lặp lại và cải thiện prompt

**Liên kết:** [[Generative AI]], [[Prompting]], [[Context]], [[References]], [[AI Output Evaluation]], [[Iterative Design]]

