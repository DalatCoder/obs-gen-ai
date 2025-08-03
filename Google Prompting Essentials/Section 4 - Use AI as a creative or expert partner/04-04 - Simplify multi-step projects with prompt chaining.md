## Đơn giản hóa dự án đa bước với Prompt Chaining

### Khái niệm Prompt Chaining

**Prompt Chaining** (chuỗi prompt) là kỹ thuật kết nối các prompt với nhau bằng cách sử dụng đầu ra của prompt này làm ngữ cảnh (context) cho prompt tiếp theo. Quá trình này giống như kết nối các mắt xích trong một chuỗi.

**Lợi ích chính:**

- Chia nhỏ nhiệm vụ phức tạp thành các bước đơn giản hơn
- Duy trì kiểm soát của con người trong quy trình (human-in-the-loop)
- Giúp phát hiện và xử lý các hallucination (ảo giác AI)
- Tăng tính chính xác và kiểm soát chất lượng đầu ra


### Ví dụ thực tế: Thiết kế khóa đào tạo nhân viên mới

**Bước 1: Tạo outline tổng quan**

```
Prompt đầu vào:
Tôi là trưởng phòng nhân sự của một công ty quảng cáo và đang thiết kế khóa đào tạo cho nhân viên mới. Hãy tạo một outline chi tiết các phần quan trọng nhất của khóa đào tạo cho nhân viên entry-level.
```

**Đầu ra mẫu:**

- Giới thiệu văn hóa và giá trị công ty
- Tóm tắt nhiệm vụ và trách nhiệm
- Giải thích các nguyên tắc cơ bản của ngành quảng cáo
- Phân tích các công cụ và công nghệ của công ty
- Chi tiết về mối quan hệ khách hàng và thực hành giao tiếp
- Xem xét các chính sách và quy trình của công ty
- Khuyến khích phát triển chuyên môn và tăng trưởng

**Bước 2: Mở rộng chi tiết một mục cụ thể**

```
Prompt đầu vào:
Hãy mở rộng mục số 2 từ outline đính kèm thành một đoạn văn 100 từ, bao gồm cả kỳ vọng cho năm đầu tiên của họ.
```

**Bước 3: Tạo quiz kiểm tra**

```
Prompt đầu vào:
Sử dụng đoạn văn đính kèm, hãy đề xuất một bài quiz 3 câu hỏi để kiểm tra sự hiểu biết của người đọc về nội dung.
```

**Bước 4: Thiết kế hình ảnh minh họa**

```
Prompt đầu vào:
Dựa trên đoạn văn đính kèm, tạo một đồ họa năng động để chúc mừng người đọc khi trả lời đúng, có hình ảnh đồ dùng nghệ thuật và máy tính.
```


### Các loại Prompt Chaining nâng cao

#### Chain-of-thought Prompting (Chuỗi suy nghĩ)

**Định nghĩa:** Kỹ thuật yêu cầu [[AI]] giải thích từng bước lý luận từ đầu vào đến đầu ra.

**Cách sử dụng:**

- Sử dụng cụm từ khóa: "explain your reasoning" (giải thích lý luận của bạn)
- "go step by step" (đi từng bước một)

**Ví dụ:**

```
Prompt:
Soạn một đoạn văn khoảng 100 từ chi tiết về các nhiệm vụ và trách nhiệm chính của nhân viên thiết kế entry-level tại công ty quảng cáo. Hãy giải thích lý luận từng bước.
```

**Lợi ích:**

- Hiểu được cách [[AI]] đưa ra kết luận
- Phát hiện điểm yếu trong quá trình lý luận
- Có thể can thiệp và điều chỉnh tại bước cụ thể


#### Tree-of-thought Prompting (Cây suy nghĩ)

**Định nghĩa:** Kỹ thuật khám phá nhiều giải pháp có thể cùng lúc, giúp tìm ra cách tiếp cận hiệu quả nhất.

**Cách thức hoạt động:**

- Tạo nhiều phản hồi cho một prompt
- Đánh giá và chọn ra những phương án tốt nhất
- Có thể quay lại nhánh trước đó nếu không hài lòng

**Ví dụ:**

```
Prompt:
Hãy tưởng tượng có ba nhà thiết kế khác nhau đang trình bày ý tưởng của họ với tôi.

Tất cả các nhà thiết kế sẽ viết ra một bước trong suy nghĩ của họ, sau đó chia sẻ với nhóm. Sau đó tất cả các chuyên gia sẽ chuyển sang bước tiếp theo, v.v. Nếu bất kỳ chuyên gia nào nhận ra họ sai tại bất kỳ thời điểm nào, thì họ rời khỏi.

Câu hỏi là: Tạo một hình ảnh năng động và có hình ảnh đồ dùng nghệ thuật cũng như máy tính. Cho tôi thấy ba gợi ý với các phong cách rất khác nhau từ đơn giản đến chi tiết và phức tạp.
```


### Kết hợp các kỹ thuật

**Chain-of-thought + Tree-of-thought:** Khi cần hiểu biết sâu về lý luận của [[AI]] và muốn có nhiều lựa chọn khác nhau, hai kỹ thuật này có thể hoạt động hoàn hảo cùng nhau.

### Lưu ý quan trọng

- Một số mô hình [[AI]] không tự động giữ lại ngữ cảnh từ prompt này sang prompt khác
- Có thể cần nhập lại thông tin liên quan vào prompt mới
- Các mô hình [[AI]] nâng cao có thể tự động phát hiện cơ hội cho chain-of-thought hoặc tree-of-thought
- Thử nghiệm với nhiều mô hình khác nhau để so sánh kết quả


### Ghi chú thêm

[[Prompt chaining]] giúp biến các dự án khó thành dễ dàng hơn bằng cách chia nhỏ nhiệm vụ lớn thành các prompt tuần tự đơn giản. Tuy nhiên, quá trình này vẫn cần kỹ năng tư duy phản biện của con người để hoạt động tốt nhất.

**Liên kết:** [[Generative AI]], [[Prompt Engineering]], [[Chain-of-thought]], [[Tree-of-thought]], [[Human-in-the-loop]], [[Context]], [[Hallucination]]

