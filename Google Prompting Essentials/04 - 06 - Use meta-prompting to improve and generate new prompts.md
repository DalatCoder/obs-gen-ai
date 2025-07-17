# Sử dụng Meta-Prompting để Cải thiện và Tạo Prompt mới

## Giới thiệu về Meta-Prompting

Một nửa thử thách trong việc tận dụng tối đa các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) là biết cách đặt câu hỏi đúng. **Meta-prompting** là một kỹ thuật sử dụng Gen AI để giúp bạn tạo ra hoặc cải thiện các prompt - biến công cụ này thành một nhà thiết kế prompt cá nhân! Thay vì đoán xem prompt tốt nhất là gì, bạn có thể hỏi trực tiếp công cụ để có gợi ý về cách đạt được kết quả mong muốn.

## Tổng quan về Meta-Prompting

Các kỹ thuật meta-prompting đôi khi được gọi là **"automatic prompt engineering"** (kỹ thuật prompt tự động). Giống như khung prompting (Task, Context, References, Evaluate, Iterate) cung cấp nền tảng vững chắc cho việc thiết kế prompt, meta-prompting cũng có bộ thực hành tốt nhất riêng, hay các **chiến lược power-up**.

Meta-prompting được chia thành hai danh mục chính:

- **Prompt generation strategies** (Chiến lược tạo prompt): Giúp thiết kế prompt từ đầu
    
- **Prompt refinement strategies** (Chiến lược tinh chỉnh prompt): Tinh chỉnh các prompt đã thiết kế
    

## Chiến lược Tạo Prompt (Prompt Generation Strategies)

|Chiến lược|Mục đích sử dụng|Ví dụ prompt|
|---|---|---|
|**Direct generation** (Tạo trực tiếp)|Yêu cầu công cụ Gen AI tạo prompt cho bạn|Bạn là đại diện nhân sự phụ trách tuyển dụng và sẵn sàng chào đón đồng nghiệp mới.  <br>Bạn viết: `Generate a prompt that could help write a job offer letter to our top candidates.`  <br>(Tạo một prompt có thể giúp viết thư mời làm việc cho các ứng viên hàng đầu.)|
|**Template request** (Yêu cầu mẫu)|Yêu cầu công cụ Gen AI tạo outline để tổ chức nội dung prompt|Bạn là quản lý đội bóng chày chuẩn bị đi thi đấu xa.  <br>Bạn viết: `Create a template specifying the most important elements of a gen AI prompt meant to plan travel for a baseball team and its personnel.`  <br>(Tạo một mẫu chỉ định các yếu tố quan trọng nhất của prompt Gen AI dùng để lập kế hoạch du lịch cho đội bóng chày và nhân viên.)|
|**Image** (Sử dụng hình ảnh)|Sử dụng hình ảnh làm tham chiếu để tạo prompt hoặc định hình prompt đã thử|Bạn là chủ startup thức ăn cho chó, muốn logo gợi nhớ đến bức tranh sơn dầu cũ tìm thấy online.  <br>Bạn dán hình ảnh vào prompt và viết: `Generate a prompt I can use to create the perfect logo for my dog food company that evokes the style of the attached image.`  <br>(Tạo prompt để tạo logo hoàn hảo cho công ty thức ăn chó gợi nhớ phong cách hình ảnh đính kèm.)|
|**Text** (Sử dụng văn bản)|Sử dụng văn bản làm tham chiếu để tạo prompt hoặc định hình prompt đã thử|Bạn gặp khó khăn với hướng dẫn sử dụng máy tính mới.  <br>Bạn có thể tải manual bằng PDF hoặc dán văn bản vào prompt và viết: `Using the text, generate a prompt to begin an explanation of the most important concepts in this manual.`  <br>(Sử dụng văn bản này, tạo prompt để bắt đầu giải thích các khái niệm quan trọng nhất trong manual.)|
|**Meta-prompt chaining** (Chuỗi meta-prompt)|Chia quá trình tạo prompt thành chuỗi các sub-prompt|Bạn cần prompt để tạo đề xuất tài trợ, nhưng với nhiều chi tiết, direct generation không hiệu quả.  <br>Bạn viết: `Generate a prompt that identifies the most important qualities of an intelligent and accessible intro paragraph for a grant proposal.`  <br>(Tạo prompt xác định những phẩm chất quan trọng nhất của đoạn mở đầu thông minh và dễ hiểu cho đề xuất tài trợ.)  <br>Từ đó, bạn có thể sử dụng phản hồi để xây dựng các prompt bổ sung.|

## Chiến lược Tinh chỉnh Prompt (Prompt Refinement Strategies)

|Chiến lược|Mục đích sử dụng|Giải pháp|
|---|---|---|
|**Leveling up** (Nâng cấp)|Yêu cầu công cụ Gen AI trực tiếp nâng cao prompting của bạn|Bạn đang soạn bản sao cho chiến dịch quảng cáo của garage sửa xe địa phương, nhưng kết quả thiếu cảm giác nhanh và mạnh mẽ.  <br>**Từ:** `I'm working on an ad campaign for a local auto body shop's sale on tires and windshields. Generate an announcement for the sale.`  <br>(Tôi đang làm chiến dịch quảng cáo cho garage sửa xe địa phương về việc giảm giá lốp và kính chắn gió. Tạo thông báo về đợt giảm giá.)  <br>**Thành:** `How can I change my initial prompt to produce an ad campaign that uses more engaging language and creates a more memorable impression?`  <br>(Làm thế nào tôi có thể thay đổi prompt ban đầu để tạo chiến dịch quảng cáo sử dụng ngôn ngữ hấp dẫn hơn và tạo ấn tượng đáng nhớ hơn?)|
|**Remixing** (Trộn lại)|Yêu cầu công cụ Gen AI tổng hợp nhiều prompt đính kèm thành super-prompt bao gồm ngữ cảnh chính từ mỗi prompt|Bạn đang viết đoạn mở đầu để brief nhà thầu về dự án thiết kế đồ họa, nhưng kết quả của mỗi prompt đều thiếu một phần quan trọng nào đó.  <br>Bạn có thể copy tất cả prompt và hướng dẫn công cụ Gen AI kết hợp chúng thành một prompt duy nhất giữ lại những phần quan trọng nhất.|
|**Style swap** (Đổi phong cách)|Điều chỉnh tâm trạng và giọng điệu của prompt để tạo ra sản phẩm cuối cùng sống động và đầy màu sắc hơn|Prompt ban đầu yêu cầu mô tả nhạc dân gian Ireland trả về kết quả kỹ thuật. Thông tin đúng nhưng nhàm chán! Bạn muốn biết về linh hồn của âm nhạc.  <br>Bạn có thể hướng dẫn công cụ Gen AI viết lại prompt với trọng tâm về cảm xúc và sử dụng ngôn ngữ biểu cảm, đầy đam mê hơn để truyền đạt trải nghiệm âm nhạc.|

## Lợi ích của Meta-Prompting

Với meta-prompting, bạn có thể **nhờ Gen AI giúp thiết kế prompt hoàn hảo** hoặc đưa prompt đã viết lên tầm cao mới. Với các chiến lược power-up để hướng dẫn meta-prompting, bạn sẽ biết chính xác phải làm gì khi gặp khó khăn trong việc xây dựng prompt tốt nhất.

Trong thiết kế prompt, meta-prompting chính là **lộ trình dẫn đến kết quả thành công**.