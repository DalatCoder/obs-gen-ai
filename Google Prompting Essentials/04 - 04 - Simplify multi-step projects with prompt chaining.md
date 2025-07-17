# Đơn giản hóa các dự án đa bước với Prompt Chaining

## Tổng quan về Prompt Chaining

Một số dự án **quá lớn để hoàn thành cùng lúc** - công việc nhiều phần thường được hoàn thành từng bước một. Khi làm việc với các công cụ trí tuệ nhân tạo tạo sinh (Gen AI), một số thách thức được giải quyết tốt nhất bằng cách **chia nhỏ thành các nhiệm vụ nhỏ hơn và liên kết với nhau**. Việc thực hiện từng bước cũng duy trì **cách tiếp cận có con người tham gia** (human-in-the-loop approach), giúp bạn đánh giá các prompt và kết quả khi tiếp tục kết nối chúng để phát hiện các ảo giác (hallucinations).

## Khái niệm cốt lõi

**Prompt chaining** (chuỗi prompt) là quá trình lấy đầu ra của một công cụ trí tuệ nhân tạo tạo sinh (Gen AI) và sử dụng nó làm ngữ cảnh cho một prompt mới. Việc kết nối các prompt giống như **nối các khoen trong một chuỗi xích** - đó là lý do tại sao quá trình này được gọi là prompt chaining.

> **Nguyên tắc thành công**: Một chuỗi prompt tốt chỉ mạnh bằng các prompt bên trong nó, và **tính cụ thể là bí quyết thành công**.

## Ví dụ thực hành: Thiết kế khóa đào tạo nhân viên mới

## Bối cảnh

Bạn là **trưởng phòng nhân sự** của một công ty quảng cáo và được giao nhiệm vụ thiết kế khóa đào tạo cho nhân viên mới. Tạo chương trình từ đầu bao gồm nhiều thành phần, vì vậy bạn sẽ sử dụng prompt chaining để **giữ khối lượng công việc có thể quản lý**.

## Bước 1: Tạo dàn ý khóa đào tạo

**Prompt:**

text

`I'm the head of human resources for an advertising agency, and I'm designing an onboarding course for new hires. Generate an outline specifying the most important parts of an onboarding course for an entry-level hire.`

_(Tôi là trưởng phòng nhân sự của một công ty quảng cáo và đang thiết kế khóa đào tạo cho nhân viên mới. Tạo dàn ý nêu rõ những phần quan trọng nhất của khóa đào tạo cho nhân viên cấp cơ sở.)_

**Kết quả mẫu:**

text

`Onboarding Course Outline for Entry-Level Hires at an Advertising Agency • Introduce agency culture and values • Summarize duties and responsibilities   • Explain advertising industry fundamentals • Break down agency tools and technology • Detail client relationships and communication practices • Review agency policies and procedures • Encourage professional development and growth`

## Bước 2: Mở rộng nội dung cụ thể

**Lưu ý quan trọng**: Một số mô hình trí tuệ nhân tạo tạo sinh (Gen AI) **không tự động giữ ngữ cảnh** từ prompt này sang prompt khác và có thể yêu cầu bạn nhập lại thông tin liên quan.

**Prompt:**

text

`Expand the second bullet point from the attached outline into a paragraph of 100 words, including expectations for their first year.`

_(Mở rộng điểm thứ hai từ dàn ý đính kèm thành một đoạn văn 100 từ, bao gồm kỳ vọng cho năm đầu tiên của họ.)_

**Kết quả mẫu:**

text

`As a new entry-level design hire at our ad agency, you will primarily focus on assisting our senior designers and art directors with various projects. Your responsibilities will include: researching design trends and industry best practices, creating concept sketches and mood boards, preparing presentation materials, and assisting with file organization and management. In your first year, we expect you to develop a strong foundation in design principles and software applications. Additionally, you will have the opportunity to contribute to client projects and gradually take on more independent design tasks.`

## Bước 3: Tạo hoạt động tương tác

**Prompt:**

text

`Using the attached text, suggest a three-question quiz to test the reader's familiarity with the content.`

_(Sử dụng văn bản đính kèm, đề xuất một bài kiểm tra ba câu hỏi để kiểm tra độ quen thuộc của người đọc với nội dung.)_

**Kết quả mẫu:**

text

`Question 1: What is the primary responsibility of the new design hire? A) Managing the agency's design and copywriting resources B) Creating visually appealing designs for advertising materials   C) Writing creative copy for advertisements Question 2: With whom will the new design hire collaborate? A) Clients only B) Copywriters and account managers C) Designers from other agencies Question 3: What is expected of the new design hire in terms of professional development? A) Staying steady in their current skills B) Avoiding industry trends C) Continuously learning and improving their design abilities`

## Bước 4: Tạo nội dung hình ảnh

**Prompt:**

text

`Based on the attached text, generate a visually energetic graphic that congratulates the reader on a correct answer, and features images of art supplies and computers.`

_(Dựa trên văn bản đính kèm, tạo một đồ họa tràn đầy năng lượng thể hiện sự chúc mừng người đọc trả lời đúng, và có hình ảnh đồ dùng nghệ thuật và máy tính.)_

## Khả năng mở rộng

**Chuỗi có thể tiếp tục vô hạn** - giới hạn duy nhất là sự sáng tạo của bạn. Bạn thậm chí có thể **quay lại và sử dụng các đầu ra đã chuỗi** trong các prompt khác nhau, chẳng hạn như tạo khóa đào tạo cho các phòng ban khác.

## Các kỹ thuật Prompt Chaining nâng cao

## 1. Chain-of-Thought Prompting (C-O-T)

**Chain-of-thought prompting** cho phép bạn **hiểu chi tiết về cách một công cụ trí tuệ nhân tạo tạo sinh (Gen AI) đạt đến kết luận**. Với kỹ thuật này, bạn có thể yêu cầu công cụ **truy ngược con đường từ đầu vào đến đầu ra**, liệt kê từng bước lý luận đằng sau phản hồi.

## Cách sử dụng

Sử dụng các **cụm từ khóa** như:

- `"explain your reasoning"` (giải thích lý luận của bạn)
    
- `"go step by step"` (thực hiện từng bước)
    

## Ví dụ thực hành

**Prompt:**

text

`Draft a paragraph of approximately 100 words detailing the major duties and responsibilities of a new entry-level design hire at an ad agency. Explain your reasoning step by step.`

_(Soạn thảo một đoạn văn khoảng 100 từ nêu chi tiết các nhiệm vụ và trách nhiệm chính của một nhân viên thiết kế cấp cơ sở mới tại một công ty quảng cáo. Giải thích lý luận của bạn từng bước.)_

**Kết quả mẫu:**

text

`Reasoning: Step 1: Identify Core Responsibilities Step 2: Highlight Essential Skills   Step 3: Emphasize Collaboration Step 4: Address Industry Standards Paragraph: As a new entry-level design hire at our ad agency, you will primarily focus on assisting our senior designers and art directors with various projects. Your responsibilities will include: researching design trends and industry best practices, creating concept sketches and mood boards, preparing presentation materials, and assisting with file organization and management. In your first year, we expect you to develop a strong foundation in design principles and software applications. Additionally, you will have the opportunity to contribute to client projects and gradually take on more independent design tasks.`

## Lợi ích

- **Điều chỉnh hướng quyết định** từ một bước cụ thể
    
- **Xác định nguồn gốc nhầm lẫn** khi kết quả không đạt mục tiêu
    
- **Hiểu lý do** tại sao trí tuệ nhân tạo tạo sinh (Gen AI) đưa ra những quyết định như vậy
    

## 2. Tree-of-Thought Prompting (TOT)

**Tree-of-thought prompting** là kỹ thuật **khám phá nhiều giải pháp có thể cùng lúc**, giúp bạn tìm ra cách tiếp cận hiệu quả nhất. Thay vì theo một chuỗi suy nghĩ duy nhất, bạn **tạo ra nhiều phản hồi cho prompt**, sau đó đánh giá và chọn những cái tốt nhất để theo đuổi.

## Cách thức hoạt động

- **Tạo ra nhiều nhánh** giải pháp
    
- **Đánh giá và chọn lọc** những nhánh tốt nhất
    
- **Quay lại nhánh trước** nếu không hài lòng với kết quả
    

## Ví dụ thực hành

**Prompt:**

text

`Imagine three different designers are pitching their design to me. All designers will write down one step of their thinking, then share it with the group. Then all experts will go on to the next step, etc. If any expert realizes they're wrong at any point, then they leave. The question is: Generate an image that's visually energetic, and features images of art supplies and computers. Show me three suggestions in very different styles from simple to detailed and complex.`

*(Hãy tưởng tượng ba nhà thiết kế khác nhau đang trình bày thiết kế của họ cho tôi.

Tất cả các nhà thiết kế sẽ viết ra một bước suy nghĩ của họ, sau đó chia sẻ với nhóm. Sau đó tất cả các chuyên gia sẽ chuyển sang bước tiếp theo, v.v. Nếu bất kỳ chuyên gia nào nhận ra họ đang sai vào bất kỳ thời điểm nào, thì họ sẽ rời khỏi.

Câu hỏi là: Tạo một hình ảnh tràn đầy năng lượng và có hình ảnh đồ dùng nghệ thuật và máy tính. Cho tôi xem ba đề xuất theo phong cách rất khác nhau từ đơn giản đến chi tiết và phức tạp.)*

## Kết hợp kỹ thuật

**Trong một số trường hợp, việc kết hợp tree-of-thought với chain-of-thought** có thể mang lại hiệu quả tối ưu. Khi bạn cần hiểu biết về lý luận của công cụ và các lựa chọn khác trong lý luận đó, hai kỹ thuật này có thể hoạt động hoàn hảo cùng nhau.

## Lưu ý quan trọng

## Sự khác biệt giữa các mô hình

**Prompt chaining nâng cao có thể hoạt động khác nhau** trong các mô hình trí tuệ nhân tạo tạo sinh (Gen AI) khác nhau. Một số mô hình AI tiên tiến hơn sẽ **tự động phát hiện cơ hội** cho lý luận chain-of-thought hoặc tree-of-thought mà không cần hướng dẫn cụ thể.

## Phương pháp tối ưu

- **Thử nghiệm xác nhận kết quả tốt nhất**
    
- **Lặp lại prompt với các mô hình khác nhau**
    
- **So sánh đầu ra** của chúng
    

## Kết luận

**Prompt chaining giúp các dự án khó khăn trở nên dễ dàng hơn** bằng cách chia một nhiệm vụ lớn thành các prompt tuần tự đơn giản hơn. Tuy nhiên, hãy nhớ rằng **quá trình này vẫn cần kỹ năng tư duy phản biện của con người** để hoạt động tốt nhất. Với sự hướng dẫn của bạn, prompt chaining có thể giúp bạn đánh giá, chỉ đạo và điều chỉnh quá trình prompting, để bạn có thể **đáp ứng thời hạn một cách dễ dàng**.