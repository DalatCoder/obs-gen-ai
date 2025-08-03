## Prompt với Cá tính: Điều chỉnh AI Sinh tạo theo Phong cách Viết của Bạn

### Cách AI Sinh tạo tiếp cận Tone và Style

#### Hiện tượng AI "robot" vs "thân thiện"

- Một số nội dung do AI tạo ra nghe có vẻ **máy móc** (robotic)
- Đôi khi lại cảm giác như đang **trò chuyện với bạn bè hoặc giáo sư**
- Nguyên nhân nằm ở cách AI tools xử lý **tone và style**


#### Contextual Understanding (Hiểu theo ngữ cảnh)

**Ví dụ thực tế:**

- AI chatbot được training trên dataset cuộc trò chuyện hàng ngày
- Khi bạn hỏi "What's up?", AI hiểu đây là **lời chào thông thường**
- AI sẽ phản hồi phù hợp: "Not much, how about you?"

**Khả năng của Contextual Understanding:**

- **Nhận diện audience** (đối tượng)
- **Nhận biết linguistic cues** (dấu hiệu ngôn ngữ) như dấu chấm hỏi
- **Học ngôn ngữ** từ tài liệu tham khảo được cung cấp
- **Thích ứng với preferences** (sở thích) của người dùng
- **Duy trì tính nhất quán** trong ngôn ngữ sử dụng
- **Hiểu input và tạo output** theo tone và style bạn cung cấp


### Chiến lược điều chỉnh Tone và Style trong Prompting

#### 1. Chỉ định rõ ràng Tone và Style

**Ví dụ cơ bản:**

```
Summarize this report into three short paragraphs.
```

**Ví dụ cải tiến:**

```
Summarize this report into three short paragraphs in a friendly, professional, and easy-to-comprehend tone.
```

**Nguyên tắc quan trọng:**

- **Đừng để mở** (Don't leave things to interpretation)
- **Càng cụ thể càng tốt** về tone mong muốn
- **Input ban đầu** sẽ ảnh hưởng đến toàn bộ conversation thread


#### 2. Sử dụng từ ngữ mô tả cụ thể

**Thay vì chung chung → Dùng mô tả chi tiết:**


| Chung chung | Cụ thể |
| :-- | :-- |
| Humorous | Witty banter (châm biếm dí dỏm) |
| Casual | Like talking to a friend |
| Academic | Scholarly and in-depth, like a professor |
| Persuasive | Compelling and convincing |
| Sarcastic | Dryly funny, like a wry comedian |
| Inspirational | Motivating and uplifting |
| Simple | Like you're a kindergarten teacher explaining this to their students |

**Thêm constraints (ràng buộc):**

```
Avoid using jargon that would be confusing to people who are unfamiliar with the subject.
```


#### 3. Cung cấp References (Tài liệu tham khảo)

**Ví dụ prompt với reference:**

```
Help me draft a description for a new line of rock climbing apparel. The target audience is young outdoor enthusiasts and climbers. I want the description to speak to the audience's desire for durable, attractive rock climbing apparel for indoor and outdoor climbing. Keep the language upbeat, informative, and inspiring. Imagine you're talking to a friend who's an avid rock climber.

Consider the tone and style of interviews with history's most renowned climbers as a reference.
```

**Các cách sử dụng reference:**

- **Thêm ngay từ đầu**: Để có direction rõ ràng
- **Thêm sau khi đánh giá output**: Nếu kết quả chưa như ý
- **Sử dụng output làm reference**: Cho lần iterate tiếp theo


#### 4. Iterate để tinh chỉnh Tone và Style

**Khi nào cần iterate:**

- Output quá **nhạt nhẽo** (bland)
- Ngôn ngữ **không appeal** đến target audience
- Tone **không đúng như mong đợi**

**Ví dụ iterate cải tiến:**

```
I need this product line description to speak to the heart of young climbers of all kinds. I want to evoke their passion for pushing limits both indoors and out. The shirts, jackets, pants, shorts, tanks, and carabiners enable climbers to express their personal style without sacrificing quality, comfort, or durability, ensuring they look sharp and climb smart. Channel the spirit of climbing legends, and inspire them to reach new heights. Make the language less cheeky and more reverent of the sport.
```

**Nguyên tắc:** **Always Be Iterating!** - Tiếp tục tinh chỉnh prompt để có kết quả phù hợp

### Tại sao Prompting cho Tone và Style quan trọng

#### Ảnh hưởng đến communication

- **Professional email**: Tone trang trọng, chuyên nghiệp
- **Social media post**: Tone vui vẻ, thân thiện
- **Persuasive essay**: Tone thuyết phục, có logic


#### Cách tiếp cận hiệu quả

- **Coi AI như một diễn viên**: Càng hướng dẫn rõ ràng, diễn viên càng thể hiện tốt vai diễn
- **Contextual understanding** giúp AI hiểu ý định
- **References và iteration** giúp tinh chỉnh kết quả


#### Tầm quan trọng của Nuance (sắc thái)

- **Sắc thái rất quan trọng** trong giao tiếp
- **Càng dạy AI nhiều** về nuance, AI càng hữu ích
- **Specific prompts** giúp thu hẹp đúng tone mong muốn
- Giúp AI **phục vụ tốt hơn** cả cá nhân và workplace context


### Takeaway chính

- **Tone và style** quyết định cách message được truyền tải và tiếp nhận
- **Contextual understanding** là nền tảng để AI hiểu tone/style
- **Specific descriptors** hiệu quả hơn từ ngữ chung chung
- **References** cung cấp mẫu cụ thể cho AI học theo
- **Iteration** là chìa khóa để đạt kết quả hoàn hảo
- **Treat AI như director hướng dẫn diễn viên** - càng chi tiết càng tốt

**Liên kết:** [[Contextual Understanding]], [[Prompt Framework]], [[Tone Adjustment]], [[Style Matching]], [[AI Communication]], [[Iterative Prompting]], [[Voice and Tone]], [[Reference-based Prompting]], [[Audience Targeting]]

