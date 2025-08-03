## AgentX - AI Agent tư vấn chuyên gia

### Khái niệm AgentX

**AgentX** là loại [[AI Agent]] thứ hai hoạt động như một **consultant cá nhân** (personalized consultant). Với prompt phù hợp, bạn có thể hướng dẫn agent trở thành chuyên gia về bất kỳ lĩnh vực nào bạn cần.

**Đặc điểm chính:**

- Cung cấp phản hồi chuyên môn chi tiết
- Có thể đóng vai trò khách hàng hoặc đối tác kinh doanh
- Phù hợp cho việc luyện tập thuyết trình và nhận feedback


### Ví dụ thực tế: Tạo AgentX để đánh giá pitch

**Tình huống:** Cần [[AI Agent]] cung cấp phản hồi chuyên môn về bài thuyết trình (pitch) cho khách hàng tiềm năng - công ty xe thể thao nổi tiếng.

#### Bước 1: Thiết lập persona và vai trò

```
You are my potential client, the VP of advertising at a world famous sports car company known for its innovation, performance, and engineering excellence.
```


#### Bước 2: Thiết lập bối cảnh cụ thể

```
You're considering hiring a creative agency to develop a new campaign that will attract a younger generation of buyers.

You are in a meeting with me, the design director of a creative agency that's pitching a new campaign for your company.
```


#### Bước 3: Hướng dẫn tương tác

```
Act as my potential client when I provide answers, critique the answers if needed, ask follow up questions.

Continue the conversation until I give the stop rule "BREAK".

Then give me a summary of the whole conversation highlighting ways I can improve my pitch.
```


#### Bước 4: Cung cấp context chi tiết

```
I've included the brief the car company provided me that has all the relevant information for this project. Use the information from this brief to inform your answers.
```


### Sử dụng Long Context Window

**Lý do cần Long Context Window:**

- Prompt chứa nhiều ngữ cảnh và thông tin về khách hàng tiềm năng
- Cho phép [[Generative AI]] giữ lại và sử dụng nhiều thông tin hơn
- Dẫn đến phản hồi chất lượng tốt hơn

**Công cụ sử dụng:** Google AI Studio (thay vì Gemini thông thường)

### Quy trình hoạt động

#### 1. Bắt đầu cuộc trò chuyện

- [[AI Agent]] đóng vai VP of advertising
- Đặt câu hỏi chi tiết về campaign
- Yêu cầu thêm thông tin cụ thể


#### 2. Đánh giá và phản hồi

- Phân tích từng điểm trong pitch
- Chỉ ra những điểm cần được giải quyết
- Đặt câu hỏi follow-up để làm rõ


#### 3. Tổng kết và đưa ra khuyến nghị

- Sử dụng stop rule "BREAK" để kết thúc
- Nhận summary toàn bộ cuộc trò chuyện
- Highlighted các cách cải thiện pitch


### Lợi ích của AgentX

**Luyện tập an toàn:**

- Môi trường không có áp lực thực tế
- Có thể thử nhiều approach khác nhau
- Nhận feedback chi tiết và xây dựng

**Tiết kiệm thời gian:**

- Không cần chờ đến meeting thực tế
- Có thể luyện tập bất cứ lúc nào
- Refine pitch nhiều lần trước khi gặp khách hàng thật

**Feedback chất lượng:**

- Dựa trên brief và context cụ thể
- Quan điểm từ góc độ khách hàng
- Suggestions cải thiện cụ thể


### GEMS - Customized Versions của Gemini

**Khái niệm:** GEMS là các phiên bản tùy chỉnh của Gemini được thiết kế cho nhu cầu cụ thể.

**Cách tạo GEMS:**

- Mô tả chức năng bạn muốn GEM thực hiện
- Chỉ định cách bạn muốn nó phản hồi
- Gemini sẽ sử dụng instructions để tạo ra GEM phù hợp

**Lợi ích:**

- Lưu trữ và tái sử dụng prompt phức tạp
- Có thể quay lại conversation sau khi revise pitch
- Test nhiều ý tưởng khác nhau cho đến khi hoàn thiện


### Ghi chú thêm

AgentX đặc biệt hữu ích cho việc chuẩn bị các presentation quan trọng, negotiation, hoặc bất kỳ tình huống nào cần feedback từ perspektive của đối tác. Việc sử dụng **long context window** đảm bảo [[AI]] có đủ thông tin để đưa ra phản hồi chính xác và có giá trị.

**Liên kết:** [[AI Agent]], [[AgentSim]], [[Long Context Window]], [[Google AI Studio]], [[Personalized Consultant]], [[Pitch]], [[Feedback]], [[GEMS]], [[Generative AI]]

