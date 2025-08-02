## Thực hành Tốt nhất trong Prompting - Framework TCREI

### Tầm quan trọng của Prompting

**Prompting** là kỹ năng thiết yếu để tận dụng tối đa **Generative AI**. Để đạt kết quả tốt nhất từ công cụ AI, bạn cần tạo ra một prompt chất lượng.

**Framework prompting hiệu quả:** **Task, Context, References, Evaluate, and Iterate (TCREI)**

### 1. Specify the Task (Xác định rõ Nhiệm vụ)

**Nguyên tắc cơ bản:**

- **Mô tả chi tiết** những gì bạn muốn công cụ AI thực hiện
- **Rõ ràng và tránh mơ hồ** - hướng dẫn mơ hồ có thể dẫn đến output không liên quan hoặc sai
- **Nền tảng của mọi prompt** hiệu quả

**Thành phần của Task:**

#### Task (Nhiệm vụ)

- **Hành động cụ thể** bạn muốn công cụ hỗ trợ
- **Ví dụ:** Viết email, tạo hình ảnh, phân tích dữ liệu


#### Persona (Vai trò chuyên môn)

- **Chuyên môn** bạn muốn AI áp dụng
- **Đối tượng** mà output hướng đến
- **Ví dụ:** Chuyên gia IT, viết cho manager hoặc team


#### Format (Định dạng)

- **Cách thức trình bày** output mong muốn
- **Ví dụ:** Danh sách có bullet points, bảng so sánh, đoạn văn

**Ví dụ prompt hoàn chỉnh:**

```
Bạn là một concert promoter chuyên về tăng doanh số vé trong ngành nhạc alternative rock. Tạo một bài đăng mạng xã hội về festival âm nhạc sắp tới, hướng đến cộng đồng âm nhạc địa phương đồng thời thu hút những người tham gia từ ngoài bang. Giới hạn bài đăng trong 125 ký tự. Bao gồm 5 hashtags liên quan.
```


### 2. Provide Necessary Context (Cung cấp Ngữ cảnh cần thiết)

**Mục đích:** Thu hẹp tiêu điểm của công cụ AI, cho phép tạo ra output phù hợp và hiệu quả hơn.

**Thông tin ngữ cảnh bao gồm:**

- **Lý do và mục tiêu** thực hiện nhiệm vụ
- **Quy tắc hoặc hướng dẫn** mà output phải tuân theo
- **Thông tin nền liên quan** công cụ nên xem xét

**Ví dụ prompt có context:**

```
Bạn là một concert promoter chuyên về tăng doanh số vé trong ngành nhạc alternative rock. Tạo một bài đăng mạng xã hội về festival âm nhạc sắp tới, hướng đến cộng đồng âm nhạc địa phương đồng thời thu hút những người tham gia từ ngoài bang. Giới hạn bài đăng trong 125 ký tự. Bao gồm 5 hashtags liên quan. 

Đối tượng địa phương chủ yếu là sinh viên đại học và chuyên gia trẻ (21-35 tuổi) theo dõi indie rock. Festival có 12 ban nhạc trong 2 ngày, với lựa chọn cắm trại và các nhà cung cấp thức ăn địa phương.
```

**Lợi ích:** Tạo ra output hấp dẫn và hiệu quả hơn, phù hợp với đối tượng cụ thể mà không cần thời gian thêm để điều chỉnh prompt ban đầu.

### 3. Include References as Examples (Bao gồm Tham chiếu làm Ví dụ)

**Định nghĩa:** References cung cấp ví dụ hoặc tài nguyên minh họa những gì bạn muốn công cụ AI tạo ra.

**Chức năng:**

- Xác định chi tiết về output mong muốn: **style, tone, format**
- Có thể bao gồm: text, images, audio, hoặc video (tùy công cụ AI)

**Gợi ý khi sử dụng references:**

- **Giải thích ngắn gọn** cách references liên quan đến nhiệm vụ
- **Sử dụng 2-5 ví dụ chất lượng cao** phù hợp với nhu cầu
- **Bao gồm công việc của bạn** hoặc ví dụ open-source nếu liên quan

**Ví dụ prompt có references:**

```
[Task và Context như trên]

Đây là các ví dụ về bài đăng thành công từ sự kiện tương tự:

- Ví dụ 1: "Where mountains meet music: Indie Rocks Festival returns! Your favorite local bands + national acts. Good eats & Sleep under the stars! #IndieRocks #SupportLocalMusic"
- Ví dụ 2: "Join Indie Fest under the desert skies! 2 nights of raw sound 2 move you + camping vibes #RoadTrip #CampLife #RockOn"
```


### 4. Evaluate Your Output (Đánh giá Output)

**Thực tế về công cụ AI:**

- Các công cụ AI khác nhau về **training và capabilities**
- Mỗi công cụ có **điểm mạnh và hạn chế riêng** ảnh hưởng đến chất lượng output

**Quy trình đánh giá:**

- **Đánh giá cẩn thận** chất lượng và hiệu quả của nội dung AI tạo ra
- **Trước khi sử dụng** hoặc chia sẻ với người khác

**Tiêu chí đánh giá output:**

- **Accuracy (Độ chính xác)**
- **Bias (Thiên kiến)**
- **Relevancy (Tính liên quan)**
- **Consistency (Tính nhất quán)**

**Nguyên tắc quan trọng:**

- **AI-generated content = starting point**, không phải sản phẩm cuối cùng
- Nếu output không thể chấp nhận hoặc không hữu ích → chuyển sang bước tiếp theo


### 5. Iterate for Better Results (Lặp lại để có Kết quả tốt hơn)

**Thực tế:** Ngay cả prompt được tạo tốt cũng có thể không cho kết quả lý tưởng ở lần đầu tiên.

**Iteration Process (Quá trình lặp lại):**

- **Quá trình tinh chỉnh prompt** dựa trên output của AI
- **Giống như cuộc trò chuyện qua lại** với công cụ AI

**Chu trình iteration:**

1. **Cung cấp prompt ban đầu**
2. **AI tool phản hồi** với output
3. **Đánh giá hiệu quả** của phản hồi AI tạo ra
4. **Tinh chỉnh yêu cầu** dựa trên những gì hiệu quả và không hiệu quả
5. **Lặp lại chu trình** cho đến khi đạt kết quả mong muốn

**Mindset hiệu quả:**

- **Không phải về việc đạt kết quả hoàn hảo ngay lần đầu**
- **Về việc sẵn sàng tinh chỉnh và cải thiện** approach
- **Kiên nhẫn, cung cấp feedback rõ ràng**, tiếp tục prompting đến khi đạt mục tiêu


### Pro Tips và Lời khuyên Thực tế

**Lưu trữ Prompt hiệu quả:**

- **Save prompt hiệu quả** cho các nhiệm vụ cụ thể
- **Sử dụng làm templates** cho các use cases và nhu cầu khác nhau
- **Giúp tái tạo AI-output thành công** một cách nhất quán mà không cần bắt đầu từ đầu

**Phát triển kỹ năng:**

- **Prompting hiệu quả** là kỹ năng cần thực hành
- **Framework TCREI** cung cấp cấu trúc có hệ thống
- **Iteration là chìa khóa** cho kết quả chất lượng cao


### Ghi chú thêm

**Khóa học mở rộng:**

- **Google Prompting Essentials** - khóa học tiếp theo sau Google AI Essentials
- **Dưới 10 giờ, tự học**, không yêu cầu kinh nghiệm trước
- **Áp dụng across industries**: content generation, data analysis, information summarization

**Liên kết:** [[Prompting]], [[Generative AI]], [[Task Specification]], [[Context]], [[References]], [[Iteration]], [[AI Output Evaluation]], [[Framework]], [[Google AI Essentials]]

