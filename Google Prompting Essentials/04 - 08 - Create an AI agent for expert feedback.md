# AgentX - AI Agent Tư vấn Chuyên nghiệp

## Giới thiệu về AgentX

Sau khi hoàn thành với AgentSim, chúng ta chuyển sang loại AI agent thứ hai - **AgentX**. Hãy nghĩ về AgentX như **tư vấn viên cá nhân** (personalized consultant) của bạn. Với prompt phù hợp, bạn có thể hướng dẫn agent trở thành chuyên gia về bất kỳ điều gì bạn cần.

## Đặc điểm của AgentX

## Long Context Window (Cửa sổ ngữ cảnh dài)

Khi sử dụng AgentX, prompt thường bao gồm **nhiều ngữ cảnh và thông tin** về chủ đề cần tư vấn. Do đó, cần sử dụng **long context window** (cửa sổ ngữ cảnh dài) cho phép công cụ trí tuệ nhân tạo tạo sinh (Gen AI) giữ lại và sử dụng nhiều thông tin hơn, dẫn đến phản hồi tốt hơn.

Trong trường hợp này, chúng ta sẽ **chuyển sang Google AI Studio** thay vì Gemini thông thường.

## Ví dụ thực tế: Phản hồi chuyên gia về Pitch

## Tình huống

Cần AI agent cung cấp **phản hồi chuyên gia về bài thuyết trình** (pitch) cho khách hàng tiềm năng.

## Xây dựng Prompt chi tiết

**Bước 1: Thiết lập persona và background**

text

`You are my potential client, the VP of advertising at a world famous sports car company known for its innovation, performance, and engineering excellence.`

_(Bạn là khách hàng tiềm năng của tôi, Phó chủ tịch quảng cáo tại một công ty xe thể thao nổi tiếng thế giới được biết đến với sự đổi mới, hiệu suất và sự xuất sắc trong kỹ thuật.)_

**Bước 2: Thiết lập bối cảnh tương tác**

text

`You're considering hiring a creative agency to develop a new campaign that will attract a younger generation of buyers. You are in a meeting with me, the design director of a creative agency that's pitching a new campaign for your company.`

_(Bạn đang cân nhắc thuê một agency sáng tạo để phát triển chiến dịch mới nhằm thu hút thế hệ người mua trẻ tuổi. Bạn đang trong cuộc họp với tôi, giám đốc thiết kế của agency sáng tạo đang thuyết trình chiến dịch mới cho công ty của bạn.)_

**Bước 3: Xác định hành động cụ thể**

text

`Act as my potential client when I provide answers, critique the answers if needed, ask follow up questions. Continue the conversation until I give the stop rule "BREAK". Then give me a summary of the whole conversation highlighting ways I can improve my pitch.`

_(Hãy đóng vai khách hàng tiềm năng của tôi khi tôi cung cấp câu trả lời, phản biện các câu trả lời nếu cần, đặt câu hỏi tiếp theo. Tiếp tục cuộc trò chuyện cho đến khi tôi đưa ra quy tắc dừng "BREAK". Sau đó hãy tóm tắt toàn bộ cuộc trò chuyện, làm nổi bật các cách tôi có thể cải thiện bài thuyết trình.)_

**Bước 4: Tích hợp tài liệu tham khảo**

text

`I've included the brief the car company provided me that has all the relevant information for this project. Use the information from this brief to inform your answers.`

_(Tôi đã bao gồm brief mà công ty xe hơi cung cấp có tất cả thông tin liên quan cho dự án này. Sử dụng thông tin từ brief này để thông báo cho câu trả lời của bạn.)_

## Phân tích Prompt theo Framework

## Cấu trúc Prompt

1. **Role** (Vai trò): Thiết lập vai trò của VP quảng cáo
    
2. **Task** (Nhiệm vụ): Xác định việc cần thực hiện - phản biện pitch và đặt câu hỏi tiếp theo
    
3. **Intended Outcome** (Kết quả mong muốn): Làm nổi bật các cách cải thiện bài thuyết trình
    

## Yếu tố quan trọng

- **Persona chi tiết**: VP của công ty xe thể thao nổi tiếng
    
- **Bối cảnh rõ ràng**: Cuộc họp thuyết trình agency
    
- **Hành động cụ thể**: Phản biện, đặt câu hỏi, tóm tắt
    
- **Stop rule**: "BREAK" để kết thúc
    
- **Tài liệu tham khảo**: Brief từ khách hàng
    

## Kết quả thực tế

## Trong quá trình tương tác

- **AI agent yêu cầu thêm chi tiết** và đặt câu hỏi sâu hơn
    
- **Xuất hiện những lo ngại** cần được giải quyết
    
- **Phản hồi hữu ích** cho vòng thực hành
    

## Sau khi sử dụng stop rule "BREAK"

AI agent cung cấp:

- **Tóm tắt cuộc trò chuyện** đến thời điểm hiện tại
    
- **Những điểm hiệu quả** và cần cải thiện
    
- **Khuyến nghị cụ thể** để củng cố bài thuyết trình
    

## Ứng dụng mở rộng

## Lợi ích của việc sử dụng AgentX

- **Tiếp tục yêu cầu phản hồi** sau khi công cụ Gen AI đóng vai khách hàng
    
- **Lưu prompt** để quay lại cuộc trò chuyện sau khi chỉnh sửa bài thuyết trình
    
- **Kiểm thử thêm ý tưởng** khi hoàn thiện phiên bản cuối cùng
    

## Tùy chỉnh với GEMS

Bạn có thể tạo **phiên bản Gemini tùy chỉnh** được gọi là **GEMS**:

1. **Mô tả những gì bạn muốn GEM thực hiện**
    
2. **Chỉ định cách bạn muốn nó phản hồi**
    
3. **Gemini sẽ nhận các hướng dẫn** và giúp tạo GEM cho nhu cầu cụ thể của bạn
    

## Tóm tắt

AgentX hoạt động như một **tư vấn viên chuyên nghiệp cá nhân**, có khả năng:

- Đóng vai bất kỳ chuyên gia nào bạn cần
    
- Cung cấp phản hồi chi tiết và có căn cứ
    
- Duy trì cuộc trò chuyện tương tác dài
    
- Tóm tắt và đưa ra khuyến nghị cải thiện
    
- Tùy chỉnh thành công cụ chuyên biệt thông qua GEMS