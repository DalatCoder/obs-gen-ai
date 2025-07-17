# Prompt với Cá tính: Điều chỉnh Trí tuệ nhân tạo tạo sinh (Gen AI) theo Phong cách Viết của Bạn

## Cách Các Công cụ Gen AI Xử lý Giọng điệu và Phong cách

Bạn có từng nhận ra rằng đôi khi nội dung do AI tạo ra có thể nghe rất máy móc, nhưng đôi khi lại có cảm giác như đang trò chuyện với một người bạn hoặc giáo sư? Lý do của điều này nằm ở cách các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) xử lý giọng điệu (tone) và phong cách (style). Các công cụ này thực hiện điều này theo nhiều cách khác nhau, nhưng bài đọc này sẽ tập trung vào chỉ một phương pháp.

## Hiểu Biết Ngữ cảnh (Contextual Understanding)

Hãy tưởng tượng một chatbot Gen AI được huấn luyện trên một tập dữ liệu khổng lồ các cuộc trò chuyện hàng ngày. Khi bạn hỏi "What's up?" (Có gì hay ho không?), nó hiểu rằng bạn có lẽ đang hỏi về tình hình của nó. Nó nhận ra lời chào phổ biến này từ dữ liệu huấn luyện. Rất có thể, nó sẽ phản hồi một cách phù hợp với câu như "Not much, how about you?" (Không có gì đặc biệt, còn bạn thì sao?)

Điều này nhờ vào **hiểu biết ngữ cảnh (contextual understanding)**, cho phép công cụ Gen AI diễn giải thông tin trong một bối cảnh cụ thể và sử dụng sự hiểu biết đó để tạo ra đầu ra. Điều này giúp công cụ:

- **Xác định đối tượng** (identify audiences)
    
- **Nhận biết các tín hiệu ngôn ngữ** (recognize linguistic cues), như dấu chấm hỏi ở cuối câu
    
- **Học ngôn ngữ từ các tài liệu tham khảo** được cung cấp
    
- **Thích ứng với sở thích** của bạn
    
- **Duy trì tính nhất quán** trong ngôn ngữ sử dụng
    
- **Hiểu đầu vào và tạo đầu ra** theo giọng điệu và phong cách bạn cung cấp
    

## Chiến lược về Giọng điệu và Phong cách trong Prompting

Khi nói đến việc khớp giọng điệu và phong cách, hiểu biết ngữ cảnh của công cụ Gen AI là một thành phần quan trọng - nhưng nó không tạo nên toàn bộ công thức. Đó là lúc bạn tham gia vào. Dưới đây là một số cách để điều chỉnh các prompt của bạn nhằm tinh chỉnh giọng điệu và phong cách.

## 1. Xác định Giọng điệu và Phong cách của Bạn

Khi sử dụng khung prompting, hãy nhập giọng điệu và phong cách mong muốn vào phần nhiệm vụ (task).

Có thể bạn có một báo cáo muốn tóm tắt cho đồng nghiệp hoặc quản lý. Ví dụ, bạn có thể viết:

**Prompt cơ bản:**

text

`Summarize this report into three short paragraphs.`

_(Tóm tắt báo cáo này thành ba đoạn ngắn.)_

**Thay vào đó, hãy xác định giọng điệu trong prompt:**

text

`Summarize this report into three short paragraphs in a friendly, professional, and easy-to-comprehend tone.`

_(Tóm tắt báo cáo này thành ba đoạn ngắn với giọng điệu thân thiện, chuyên nghiệp và dễ hiểu.)_

Các đầu vào của bạn sẽ tiếp tục ảnh hưởng đến đầu ra khi bạn lặp lại trong cùng một chuỗi trò chuyện, vì vậy việc rõ ràng và chi tiết từ thiết lập ban đầu là quan trọng. **Điểm mấu chốt: Đừng để mọi thứ phụ thuộc vào sự diễn giải.** Càng cụ thể về giọng điệu bạn muốn, công cụ càng có thể khớp với kỳ vọng của bạn.

## Các Ví dụ về Giọng điệu Cụ thể

Thay vì sử dụng các thuật ngữ chung chung, hãy cụ thể hóa:

- **Academic** → "scholarly and in-depth, like a professor" _(học thuật và sâu sắc, như một giáo sư)_
    
- **Persuasive** → "compelling and convincing" _(thuyết phục và có sức thuyết phục)_
    
- **Sarcastic** → "dryly funny, like a wry comedian" _(hài hước khô khan, như một diễn viên hài châm biếm)_
    
- **Inspirational** → "motivating and uplifting" _(động viên và nâng đỡ)_
    
- **Simple** → "like you're a kindergarten teacher explaining this to their students" _(như bạn là cô giáo mẫu giáo giải thích điều này cho học sinh)_
    

Cuối cùng, bạn có thể muốn thêm các **ràng buộc (constraints)** trong prompt đầu tiên để đảm bảo ngôn ngữ đi đúng hướng, chẳng hạn như:

text

`avoid using jargon that would be confusing to people who are unfamiliar with the subject`

_(tránh sử dụng thuật ngữ chuyên ngành có thể gây nhầm lẫn cho những người không quen thuộc với chủ đề)_

## 2. Cung cấp Tài liệu Tham khảo về Giọng điệu và Phong cách

Bạn có thể xác định giọng điệu và phong cách của mình thậm chí còn cụ thể hơn bằng cách cung cấp tài liệu tham khảo cho công cụ Gen AI.

Giả sử bạn đang sử dụng prompt cho công cụ Gen AI để giúp viết mô tả cho một dòng sản phẩm mới:

**Prompt cơ bản:**

text

`Help me draft a description for a new line of rock climbing apparel. The target audience is young outdoor enthusiasts and climbers. I want the description to speak to the audience's desire for durable, attractive rock climbing apparel for indoor and outdoor climbing. Keep the language upbeat, informative, and inspiring. Imagine you're talking to a friend who's an avid rock climber.`

_(Giúp tôi soạn thảo mô tả cho dòng trang phục leo núi mới. Đối tượng mục tiêu là những người trẻ tuổi đam mê hoạt động ngoài trời và leo núi. Tôi muốn mô tả nói đến mong muốn của đối tượng về trang phục leo núi bền bỉ, hấp dẫn cho hoạt động leo núi trong nhà và ngoài trời. Giữ ngôn ngữ tích cực, thông tin và truyền cảm hứng. Hãy tưởng tượng bạn đang nói chuyện với một người bạn đam mê leo núi.)_

**Prompt với tài liệu tham khảo:**

text

`Consider the tone and style of interviews with history's most renowned climbers as a reference.`

_(Hãy xem xét giọng điệu và phong cách của các cuộc phỏng vấn với những nhà leo núi nổi tiếng nhất trong lịch sử làm tài liệu tham khảo.)_

## 3. Lặp lại về Giọng điệu và Phong cách

Nếu đầu ra ban đầu không cảm thấy hoàn toàn đúng, đó là thời điểm tốt để cụ thể hóa hơn bằng cách lặp lại prompt và thêm chi tiết và hướng dẫn.

**Prompt lặp lại cải tiến:**

text

`I need this product line description to speak to the heart of young climbers of all kinds. I want to evoke their passion for pushing limits both indoors and out. The shirts, jackets, pants, shorts, tanks, and carabiners enable climbers to express their personal style without sacrificing quality, comfort, or durability, ensuring they look sharp and climb smart. Channel the spirit of climbing legends, and inspire them to reach new heights. Make the language less cheeky and more reverent of the sport.`

_(Tôi cần mô tả dòng sản phẩm này nói đến trái tim của những người leo núi trẻ tuổi thuộc mọi loại hình. Tôi muốn khơi gợi niềm đam mê vượt qua giới hạn của họ cả trong nhà và ngoài trời. Áo sơ mi, áo khoác, quần dài, quần ngắn, áo tank và móc leo núi giúp các nhà leo núi thể hiện phong cách cá nhân mà không phải hy sinh chất lượng, sự thoải mái hay độ bền, đảm bảo họ trông thật sắc sảo và leo núi thông minh. Hãy thể hiện tinh thần của những huyền thoại leo núi, và truyền cảm hứng cho họ đạt đến những đỉnh cao mới. Làm cho ngôn ngữ ít táo bạo hơn và tôn kính môn thể thao hơn.)_

**Nhớ rằng: Luôn Luôn Lặp lại (Always Be Iterating)!** Việc tiếp tục tinh chỉnh prompt cung cấp cho công cụ Gen AI nhiều thông tin hơn để bạn có thể đến gần hơn với đầu ra cuối cùng phù hợp với nhu cầu của mình.

## Tại sao Prompting về Giọng điệu và Phong cách Quan trọng

Dù bạn đang soạn thảo một email chuyên nghiệp, bài đăng mạng xã hội vui vẻ, hay một bài luận thuyết phục, giọng điệu và phong cách phù hợp có thể tạo ra sự khác biệt lớn trong cách thông điệp của bạn được truyền đạt và tiếp nhận.

Khi bạn xác định giọng nói và giọng điệu trong prompt, công cụ Gen AI sẽ sử dụng hiểu biết ngữ cảnh để tìm hiểu ý nghĩa của bạn và khớp đầu ra với giọng nói bạn hy vọng. Nếu nó không phải là những gì bạn muốn, bạn luôn có thể cung cấp tài liệu tham khảo và lặp lại.

**Để có kết quả tốt nhất từ công cụ Gen AI, hãy đối xử với nó như bạn đang đưa ra chỉ dẫn cho một diễn viên** - càng rõ ràng hướng dẫn của bạn, diễn viên càng có thể thể hiện tốt nhân vật bạn hình dung.

## Kết luận

Tóm lại, **sự tinh tế quan trọng!** Và càng dạy các công cụ Gen AI về điều đó, chúng càng có thể hữu ích hơn. Vì vậy, hãy cụ thể với các prompt của bạn và tập trung vào cách bạn muốn đầu ra nghe có vẻ như thế nào. Bằng cách làm như vậy, bạn trang bị cho các công cụ Gen AI để phục vụ bạn tốt hơn, dù là với tư cách cá nhân hay trong bối cảnh độc đáo của nơi làm việc.