## Khám Phá Kỹ Thuật Prompt Theo Chuỗi Suy Nghĩ (Chain-of-Thought Prompting)

Phân tích nhiệm vụ phức tạp thành các bước dễ quản lý có thể khó khăn, đặc biệt khi gặp lần đầu. Kỹ thuật prompt theo chuỗi suy nghĩ (chain-of-thought prompting) là một kỹ thuật prompt nâng cao giúp tận dụng khả năng giải quyết vấn đề của trí tuệ nhân tạo (AI) để xử lý công việc phức tạp từng bước một.

## Tận Dụng AI Cho Nhiệm Vụ Phức Tạp

Kỹ thuật prompt theo chuỗi suy nghĩ (chain-of-thought prompting) yêu cầu mô hình ngôn ngữ lớn (large language model) giải thích quá trình suy luận của nó. Nó khuyến khích công cụ AI (AI tool) theo dõi đường lối suy nghĩ từng bước từ đầu vào đến đầu ra.

Để sử dụng, thêm các cụm từ chính vào prompt như:

- Explain your reasoning
- Go step by step

Những bổ sung này khuyến khích AI trình bày quá trình suy nghĩ, làm cho kết quả thông tin hơn và giúp xác thực tính chính xác, độ tin cậy của kết quả.

## Ví Dụ Ứng Dụng

Giả sử quản lý nhân sự đang phát triển tài liệu onboarding cho bộ phận.

Prompt mẫu: "Create a bulleted list outlining the major duties and responsibilities of a new entry-level design hire at an ad agency. Explain your reasoning step by step."  
(Dịch: Tạo danh sách dấu đầu dòng phác thảo các nhiệm vụ và trách nhiệm chính của nhân viên thiết kế cấp độ 入门 mới tại agency quảng cáo. Giải thích suy luận của bạn từng bước một.)

Bằng cách phân tích quy trình onboarding thành các giai đoạn và hoạt động cụ thể, AI cung cấp kế hoạch có cấu trúc, toàn diện, giúp xác định khoảng trống và cải thiện quy trình.

## Kỹ Thuật Kết Nối Prompt (Prompt Chaining)

Kỹ thuật kết nối prompt (prompt chaining) liên kết các prompt liên quan như các mắt xích trong chuỗi, hữu ích cho việc giải quyết nhiệm vụ phức tạp. Thay vì dùng một prompt duy nhất, nó xây dựng dựa trên quy trình lặp lại (iteration) để nâng cao tương tác AI.

Quy trình gồm ba bước:

1. **Phân tích nhiệm vụ (Task Analysis)**: Phân tích nhiệm vụ phức tạp thành các bước logic.
2. **Prompt ban đầu (Initial Prompting)**: Tạo prompt xử lý bước đầu tiên hiệu quả.
3. **Luồng đầu vào/đầu ra (Input/Output Flow)**: Sử dụng kết quả từ prompt trước làm đầu vào cho prompt tiếp theo, lặp lại đến khi hoàn thành nhiệm vụ.

## Kết Hợp Kỹ Thuật Kết Nối Prompt Với Chuỗi Suy Nghĩ

Kết hợp kỹ thuật kết nối prompt (prompt chaining) với chuỗi suy nghĩ (chain-of-thought) nâng cao quá trình giải quyết vấn đề.

Ví dụ, quản lý nhân sự phát triển tài liệu onboarding cho nhân viên thiết kế cấp độ 入门 tại agency quảng cáo.

Kết quả prompt ban đầu:  
"Onboarding Course Outline for Entry-Level Hires at an Advertising Agency  
Introduce agency culture and values  
Summarize duties and responsibilities  
Explain advertising industry fundamentals  
Break down agency tools and technology  
Detail client relationships and communication practices"

Prompt tiếp theo (áp dụng kết nối): "Based on your initial breakdown, let's focus on understanding the role of an entry-level designer at an ad agency. What are the key responsibilities and skills required for this position? Please provide a detailed list."  
(Dịch: Dựa trên phân tích ban đầu của bạn, hãy tập trung vào việc hiểu vai trò của nhà thiết kế cấp độ 入门 tại agency quảng cáo. Các trách nhiệm và kỹ năng chính cần thiết cho vị trí này là gì? Hãy cung cấp danh sách chi tiết.)

Quy trình lặp lại này tiếp tục đến khi tất cả khía cạnh được xử lý, giúp giải quyết vấn đề khó khăn với kết quả chính xác hơn.

## Mẹo Chuyên Nghiệp

Khi sử dụng kỹ thuật kết nối prompt (prompt chaining), theo dõi các kết quả có thể liên quan ở bước sau để duy trì tính nhất quán. Sử dụng chuỗi suy nghĩ (chain-of-thought) ở bất kỳ bước nào để xác thực tính chính xác và liên quan của kết quả công cụ AI (AI tool).

## Hạn Chế Cần Xem Xét

Kỹ thuật kết nối prompt (prompt chaining) hữu ích nhưng có thách thức, đặc biệt với chuỗi dài. Công cụ AI (AI tool) có thể khó nhớ ngữ cảnh từ phần đầu, dẫn đến:

- Phản hồi không nhất quán.
- Bỏ qua chi tiết quan trọng từ prompt trước.
- Khó duy trì mục tiêu tổng thể.

## Chiến Lược Khắc Phục

- **Sử dụng điểm kiểm tra (Checkpoints)**: Thỉnh thoảng yêu cầu AI tóm tắt ngắn gọn mục tiêu tổng thể.
- **Làm việc trên nhiệm vụ phụ (Sub-Tasks)**: Phân chia nhiệm vụ rất phức tạp thành các nhiệm vụ phụ nhỏ hơn, xử lý từng cái như chuỗi ngắn trước khi chuyển sang cái tiếp theo.
- **Tóm tắt và điều hướng lại (Recap and Redirect)**: Nếu AI lệch hướng, cung cấp tóm tắt thông tin thiết yếu và hướng dẫn lại về mục tiêu chính.

Những chiến lược này đảm bảo kết quả chính xác, liên quan hơn. Như các kỹ thuật prompt khác, kỹ thuật kết nối prompt (prompt chaining) cần cân bằng giữa cung cấp ngữ cảnh cần thiết và tránh quá tải thông tin.

---

## Navigation

⬅️ [[03 - 09 - Discover few-shot prompting|Khám phá few-shot prompting]] | [[03 - 11 - Improve prompts through exploration|Cải thiện prompts thông qua khám phá]] ➡️

🏠 [[README|Trang chủ khóa học]]

---

## Chủ Đề Liên Quan

- [[03 - 04 - Write clear and specific prompts|Viết prompt rõ ràng và cụ thể]]
- [[03 - 05 - Prompting best practices|Thực hành tốt nhất cho prompting]]
- [[03 - 08 - Improve AI output through iteration|Cải thiện đầu ra AI qua lặp lại]]
- [[03 - 09 - Discover few-shot prompting|Khám phá few-shot prompting]]
- [[03 - 11 - Improve prompts through exploration|Cải thiện prompts thông qua khám phá]]

---

## Tóm Tắt Module 3

Chain-of-thought prompting giúp giải quyết các vấn đề phức tạp bằng cách chia nhỏ thành các bước logic.
