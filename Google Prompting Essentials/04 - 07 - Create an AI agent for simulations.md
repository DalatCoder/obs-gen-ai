# Tạo [[Glossary - Thuật ngữ Gen AI#AI Agent|AI Agent]] cho Mô phỏng và Thực hành

> 🧭 **Navigation**: [[04 - 06 - Use meta-prompting to improve and generate new prompts|← Trước]] | [[MOC - Google Prompting Essentials|📚 Mục lục]] | [[04 - 08 - Create an AI agent for expert feedback|Tiếp theo →]]

---

## Giới thiệu về [[Glossary - Thuật ngữ Gen AI#AI Agent|AI Agents]]

Đối với những người làm việc trong ngành công nghệ nhưng không có nền tảng kỹ thuật truyền thống, việc tự học và học hỏi trong công việc là điều rất phổ biến. Có rất nhiều điều thú vị muốn tìm hiểu, nhưng khó tìm thời gian và địa điểm phù hợp để đặt câu hỏi.

Một điều tuyệt vời về các công cụ [[Glossary - Thuật ngữ Gen AI#Gen AI|trí tuệ nhân tạo tạo sinh (Gen AI)]] là chúng có thể **tạo ra không gian an toàn để đặt câu hỏi**. Thay vì cảm thấy xấu hổ hoặc tránh né, bạn có thể nhận được lời khuyên từ chuyên gia thông qua công cụ [[Glossary - Thuật ngữ Gen AI#Gen AI|Gen AI]] chỉ với một vài [[Glossary - Thuật ngữ Gen AI#Prompt|prompt]].

Với các kỹ thuật [[Glossary - Thuật ngữ Gen AI#Prompting|prompting]] phù hợp, bạn có thể **biến công cụ [[Glossary - Thuật ngữ Gen AI#Gen AI|Gen AI]] thành đội ngũ chuyên gia riêng** sẵn sàng giúp bạn đối phó với mọi thử thách. Chúng được gọi là **[[Glossary - Thuật ngữ Gen AI#AI Agent|AI agents]]**, và mặc dù chúng không có kính nhìn đêm bí mật hay xe thể thao trang bị tên lửa, chúng cực kỳ hiệu quả trong việc hỗ trợ công việc của bạn.

## Các loại [[Glossary - Thuật ngữ Gen AI#AI Agent|AI Agents]]

Bạn có thể tạo [[Glossary - Thuật ngữ Gen AI#AI Agent|AI agents]] cho nhiều mục đích khác nhau, tùy thuộc vào nhu cầu:

- **Coding partner** (Đối tác lập trình)
- **Creative soundboard** (Bảng âm thanh sáng tạo)
- **Accountability buddy** (Người bạn giám sát) để giúp bạn theo dõi mục tiêu

## Hai loại [[Glossary - Thuật ngữ Gen AI#AI Agent|AI Agents]] chính:

| Loại Agent         | Tên gọi  | Chức năng                                                                                                                                    |
| ------------------ | -------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **Agent mô phỏng** | AgentSim | Giúp mô phỏng các tình huống như phỏng vấn hoặc thực hành cuộc trò chuyện khó khăn để bạn có thể luyện tập và thay đổi cách tiếp cận khi cần |
| **Agent tư vấn**   | AgentX   | Cung cấp phản hồi về bất kỳ chủ đề nào mà bạn yêu cầu nó trở thành chuyên gia. Giống như một **tư vấn viên cá nhân**                         |

## Chi tiết về AgentSim - Agent Mô phỏng

## Tình huống thực tế

Bạn được yêu cầu tạo một **chương trình đào tạo để giúp thực tập sinh cải thiện kỹ năng phỏng vấn** nhằm giúp họ có được vị trí mới.

## Xây dựng [[Glossary - Thuật ngữ Gen AI#AI Agent|AI Agent]] trong [[Glossary - Thuật ngữ Gen AI#Gemini|Gemini]]

**Bước 1: Thiết lập vai trò**

text

`Act as a career development training simulator.`

_(Hãy đóng vai là một trình mô phỏng đào tạo phát triển sự nghiệp.)_

**Bước 2: Xác định nhiệm vụ**  
Để agent hiệu quả, cần cung cấp nhiều chi tiết và thông tin nền về nhân vật (persona).

text

`Your task is to help interns master interview skills and conduct conversations with potential managers.`

_(Nhiệm vụ của bạn là giúp thực tập sinh thành thạo kỹ năng phỏng vấn và tiến hành cuộc trò chuyện với các nhà quản lý tiềm năng.)_

**Bước 3: Thiết lập bối cảnh**  
Cung cấp các tiêu chuẩn về những gì agent thực sự cần cung cấp trong đầu ra. Đối với các AI agent mô phỏng hoặc nhập vai, bạn cần **chỉ định các loại cuộc trò chuyện** mong muốn.

text

`You need to support the following types of conversations: - Articulating strengths and skills - Communicating professionally and confidently   - Discussing future career development goals`

\*(Bạn cần hỗ trợ các loại cuộc trò chuyện sau:

- Diễn đạt điểm mạnh và kỹ năng
- Giao tiếp chuyên nghiệp và tự tin
- Thảo luận về mục tiêu phát triển sự nghiệp tương lai)\*

**Bước 4: Hướng dẫn chi tiết**

text

`Once an intern has picked a conversation topic, provide details about the situation and the interviewer's role. Then act as the interviewer and allow the intern to participate as the employee. Make sure to guide the conversation in a way that will allow the intern to exercise their interview skills.`

_(Khi thực tập sinh đã chọn chủ đề trò chuyện, hãy cung cấp chi tiết về tình huống và vai trò của người phỏng vấn. Sau đó đóng vai người phỏng vấn và cho phép thực tập sinh tham gia với tư cách là nhân viên. Hãy đảm bảo hướng dẫn cuộc trò chuyện theo cách cho phép thực tập sinh rèn luyện kỹ năng phỏng vấn.)_

**Bước 5: Thiết lập cụm từ dừng**  
Thêm cụm từ dừng (stop phrase) để chỉ ra thời điểm và cách kết thúc nhập vai. Có thể là bất kỳ cụm từ nào: "the end", "that's a wrap", "end scene", hoặc thú vị hơn như "JAZZ HANDS".

text

`Continue the role play until the intern replies with JAZZ HANDS. After the intern gives the stop rule JAZZ HANDS, provide them with key takeaways from the simulation and skills they can work on.`

_(Tiếp tục nhập vai cho đến khi thực tập sinh trả lời với JAZZ HANDS. Sau khi thực tập sinh đưa ra quy tắc dừng JAZZ HANDS, hãy cung cấp các điểm chính từ mô phỏng và kỹ năng họ có thể làm việc.)_

## Ví dụ thực tế

**Chủ đề được chọn:** Articulating strengths and skills (Diễn đạt điểm mạnh và kỹ năng)

**Phản hồi của thực tập sinh:**

text

`My top strength is translating complex marketing concepts into clear, engaging messages that resonate with diverse audiences.`

_(Điểm mạnh hàng đầu của tôi là dịch các khái niệm marketing phức tạp thành thông điệp rõ ràng, hấp dẫn và gây được tiếng vang với nhiều đối tượng khác nhau.)_

**Gemini tiếp tục vai trò người phỏng vấn**, khuyến khích và yêu cầu ví dụ cụ thể.

**Ví dụ cụ thể:**

text

`Yes. I designed a marketing campaign for a local company who sells custom jewelry online.`

_(Có. Tôi đã thiết kế chiến dịch marketing cho một công ty địa phương bán trang sức tùy chỉnh trực tuyến.)_

**Kết thúc mô phỏng:** "JAZZ HANDS"

## Kết quả phản hồi

Agent đã cung cấp **các điểm chính từ mô phỏng**:

- **Điểm mạnh:** Trích dẫn ví dụ cụ thể và thể hiện sự nhiệt tình cũng như giá trị
- **Lĩnh vực cần cải thiện:** Cần ngắn gọn hơn và điều chỉnh câu trả lời tốt hơn

## Ứng dụng mở rộng

Đây là một trong những **cách tương tác thú vị nhất với công cụ Gen AI** vì có rất nhiều khả năng:

- **Tải lên job description** và yêu cầu công cụ đặt câu hỏi phỏng vấn dựa trên tiêu chí công việc
- **Thiết kế prompt** để AI agent đóng vai các vai trò khác nhau có thể gặp phải trong công việc
- **Sử dụng để mô phỏng** các cuộc trò chuyện, cuộc họp và phiên phản hồi

Kỹ thuật này mở ra không gian an toàn để **thực hành và cải thiện kỹ năng** mà không cần lo lắng về sự xấu hổ hay đánh giá từ người khác.

---

> 📚 **Thuật ngữ liên quan**: [[Glossary - Thuật ngữ Gen AI#AI Agent|AI Agent]] | [[Glossary - Thuật ngữ Gen AI#Simulation|Simulation]] | [[Glossary - Thuật ngữ Gen AI#Role Playing|Role Playing]]
>
> 🔗 **Xem thêm**: [[04 - 08 - Create an AI agent for expert feedback|AI agent cho phản hồi chuyên gia]] | [[04 - 10 - Ideas for AI agents|Ý tưởng cho AI agents]]
>
> 🎯 **Thực hành**: [[04 - 05 - AI IRL - Enlist AI as your though partner|AI thought partner]] | [[04 - 09 - AI IRL - Team up with AI on your next project|Teamwork với AI]]
