## Cách Viết Prompt Để Tạo Ra Kết Quả Hữu Ích

Chất lượng đầu vào ảnh hưởng lớn đến chất lượng đầu ra. Ví dụ, trong nấu ăn, nguyên liệu tươi ngon, chất lượng cao giúp tạo ra bữa ăn tuyệt vời; ngược lại, nguyên liệu kém hoặc thiếu sẽ dẫn đến kết quả không tốt. Tương tự, chất lượng prompt (lệnh) đưa vào công cụ AI hội thoại (conversational AI tool) ảnh hưởng đến chất lượng kết quả.

## Kỹ Thuật Thiết Kế Prompt (Prompt Engineering)

Kỹ thuật thiết kế prompt (prompt engineering) liên quan đến việc tạo ra prompt tốt nhất để đạt được kết quả mong muốn từ mô hình ngôn ngữ lớn (LLM). Bao gồm việc viết prompt rõ ràng, cụ thể và cung cấp ngữ cảnh liên quan.

## So Sánh Phản Hồi Của Con Người Và LLM

Giả sử một người ăn chay hỏi bạn bè: "What restaurant should I go to in San Francisco?"  
(Bạn bè sẽ gợi ý nhà hàng có lựa chọn ăn chay tốt, dựa trên kiến thức trước đó về người hỏi.)

Tuy nhiên, LLM có thể gợi ý nhà hàng không phù hợp vì thiếu kiến thức nền. Để LLM trả lời đúng, prompt phải cụ thể hơn, ví dụ đề cập đến "nhà hàng có lựa chọn ăn chay tốt".

## Ví Dụ: Sử Dụng Kỹ Thuật Thiết Kế Prompt Để Cải Thiện Kết Quả

Nhiệm vụ: Lập kế hoạch sự kiện công ty, tìm chủ đề cho hội nghị sắp tới.

Prompt ban đầu: "Generate a list of five potential themes for an event."  
(Dịch: Tạo danh sách năm chủ đề tiềm năng cho một sự kiện.)

Kết quả: Danh sách chủ đề giống tiệc tùng hơn là hội nghị chuyên nghiệp, do thiếu ngữ cảnh.

Prompt cải tiến: "Generate a list of five potential themes for a professional conference on customer experience in the hospitality industry."  
(Dịch: Tạo danh sách năm chủ đề tiềm năng cho một hội nghị chuyên nghiệp về trải nghiệm khách hàng trong ngành khách sạn.)

Kết quả: Tốt hơn, vì prompt cụ thể về hội nghị chuyên nghiệp, trải nghiệm khách hàng và ngành khách sạn.

Bạn có thể sử dụng prompt tương tự trong Gemini, ChatGPT, Microsoft Copilot hoặc các công cụ AI hội thoại khác.

## Lời Khuyên Để Tạo Kết Quả Hữu Ích

- Cung cấp hướng dẫn rõ ràng, cụ thể và bao gồm ngữ cảnh cần thiết để LLM tạo ra kết quả hữu ích.
    
- Lưu ý hạn chế của LLM: Đôi khi không thể có kết quả chất lượng dù prompt tốt, ví dụ nếu yêu cầu thông tin về sự kiện hiện tại mà LLM không tiếp cận được.
    
- Kỹ thuật thiết kế prompt thường là quá trình lặp lại (iterative process). Nếu prompt đầu không hiệu quả, chỉnh sửa để cải thiện. Trong ví dụ, lần lặp thứ hai cung cấp hướng dẫn rõ ràng hơn, dẫn đến kết quả hữu ích.