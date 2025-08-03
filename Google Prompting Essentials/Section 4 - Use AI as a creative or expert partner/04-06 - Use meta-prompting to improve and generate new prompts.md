## Sử dụng Meta-prompting để cải thiện và tạo prompts mới

### Khái niệm Meta-prompting

**Meta-prompting** là kỹ thuật sử dụng [[Generative AI]] để giúp bạn tạo ra hoặc cải thiện các prompts - biến công cụ [[AI]] thành một "nhà thiết kế prompt cá nhân". Thay vì đoán xem prompt tốt nhất là gì, bạn có thể hỏi trực tiếp công cụ để được gợi ý cách đạt được kết quả mong muốn.

**Tên gọi khác:** Automatic prompt engineering (kỹ thuật prompt tự động)

**Mục đích chính:**

- Thiết kế prompts tốt hơn để tạo ra đầu ra chất lượng cao hơn
- Giải quyết thách thức "biết cách đặt câu hỏi đúng"
- Tối ưu hóa quá trình tương tác với [[AI]]


### Hai loại chiến lược Meta-prompting

#### Prompt Generation Strategies (Chiến lược tạo prompts)

*Giúp thiết kế prompt từ đầu*

#### Prompt Refinement Strategies (Chiến lược cải thiện prompts)

*Tinh chỉnh những prompts đã có sẵn*

### Chiến lược tạo prompts (Prompt Generation Strategies)

#### 1. Direct Generation (Tạo trực tiếp)

**Định nghĩa:** Yêu cầu [[AI]] tạo ra prompt cho bạn.

**Ví dụ:**

- **Tình huống:** Bạn là đại diện nhân sự phụ trách tuyển dụng và sẵn sàng chào đón thành viên mới.
- **Prompt:** `Generate a prompt that could help write a job offer letter to our top candidates.`


#### 2. Template Request (Yêu cầu mẫu)

**Định nghĩa:** Yêu cầu [[AI]] tạo outline để tổ chức nội dung prompts.

**Ví dụ:**

- **Tình huống:** Bạn là quản lý đội bóng chày và cần lên kế hoạch cho các trận đấu xa nhà.
- **Prompt:** `Create a template specifying the most important elements of a gen AI prompt meant to plan travel for a baseball team and its personnel.`


#### 3. Image (Sử dụng hình ảnh)

**Định nghĩa:** Sử dụng hình ảnh làm tham chiếu để tạo prompt hoặc định hình prompt đã thử.

**Ví dụ:**

- **Tình huống:** Bạn sở hữu startup thức ăn cho chó và muốn logo gợi nhớ đến một bức tranh sơn dầu cũ, nhưng việc mô tả bằng lời không hiệu quả.
- **Prompt:** `Generate a prompt I can use to create the perfect logo for my dog food company that evokes the style of the attached image.`


#### 4. Text (Sử dụng văn bản)

**Định nghĩa:** Sử dụng văn bản làm tham chiếu để tạo prompt hoặc định hình prompt đã thử.

**Ví dụ:**

- **Tình huống:** Bạn gặp khó khăn với hướng dẫn sử dụng máy tính mới.
- **Prompt:** `Using the text, generate a prompt to begin an explanation of the most important concepts in this manual.`


#### 5. Meta-prompt Chaining (Chuỗi meta-prompt)

**Định nghĩa:** Chia quá trình soạn thảo prompt thành một chuỗi các sub-prompts.

**Ví dụ:**

- **Tình huống:** Bạn cần prompt để tạo đề xuất tài trợ, nhưng với tất cả chi tiết liên quan, việc tạo trực tiếp không hiệu quả.
- **Prompt:** `Generate a prompt that identifies the most important qualities of an intelligent and accessible intro paragraph for a grant proposal.`
- **Tiếp theo:** Sử dụng phản hồi để xây dựng các prompts bổ sung cho đề xuất.


### Chiến lược cải thiện prompts (Prompt Refinement Strategies)

#### 1. Leveling Up (Nâng cấp)

**Định nghĩa:** Yêu cầu [[AI]] trực tiếp nâng cao khả năng prompting của bạn.

**Ví dụ:**

- **Tình huống:** Bạn đang soạn nội dung cho chiến dịch quảng cáo của tiệm sửa xe, nhưng đầu ra thiếu cảm giác "nhanh và mạnh".
- **Từ:** `I'm working on an ad campaign for a local auto body shop's sale on tires and windshields. Generate an announcement for the sale.`
- **Thành:** `How can I change my initial prompt to produce an ad campaign that uses more engaging language and creates a more memorable impression?`


#### 2. Remixing (Kết hợp lại)

**Định nghĩa:** Yêu cầu [[AI]] tổng hợp nhiều prompts đính kèm thành một super-prompt bao gồm ngữ cảnh chính từ mỗi prompt.

**Ví dụ:**

- **Tình huống:** Bạn đang làm đoạn giới thiệu để brief các nhà thầu về dự án thiết kế đồ họa, nhưng mỗi kết quả prompt đều thiếu một phần quan trọng nào đó.
- **Giải pháp:** Copy tất cả prompts và hướng dẫn [[AI]] kết hợp chúng thành một prompt duy nhất giữ lại những phần quan trọng nhất.


#### 3. Style Swap (Đổi phong cách)

**Định nghĩa:** Chỉ định mood và tone cho prompt để tạo ra sản phẩm cuối cùng màu sắc và sinh động hơn.

**Ví dụ:**

- **Tình huống:** Prompt ban đầu yêu cầu mô tả nhạc dân gian Ireland trả về kết quả kỹ thuật. Thông tin đúng nhưng nhàm chán! Bạn muốn biết về "linh hồn" của âm nhạc.
- **Giải pháp:** Hướng dẫn [[AI]] viết lại prompt với trọng tâm vào cảm xúc, sử dụng ngôn ngữ biểu cảm và đam mê hơn để truyền đạt trải nghiệm âm nhạc.


### Ghi chú thêm

Meta-prompting cho phép bạn tranh thủ sự trợ giúp của [[Generative AI]] để thiết kế prompt hoàn hảo, hoặc đưa những prompt đã viết lên tầm cao mới. Với các chiến lược power-up để hướng dẫn meta-prompting, bạn sẽ biết chính xác phải làm gì khi gặp khó khăn trong việc xây dựng prompt tốt nhất có thể.

Trong thiết kế prompt, **meta-prompting chính là lộ trình dẫn đến đầu ra thành công**.

**Liên kết:** [[Generative AI]], [[Prompt Engineering]], [[Prompt Chaining]], [[Automatic Prompt Engineering]], [[Template Request]], [[Direct Generation]], [[Style Swap]], [[Leveling Up]], [[Meta-prompt Chaining]]

