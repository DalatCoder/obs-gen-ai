# Ghi Chú Học Tập: Kỹ Thuật Prompting Từ Rachna

## Giới Thiệu

- **Tên và Vai Trò:** Rachna là kỹ sư phần mềm (software engineer) tại Google. Cô làm việc trong đội ngũ Quản Lý Kiến Thức Trung Tâm (Central Knowledge Management), chịu trách nhiệm đảm bảo lập trình viên tiếp cận thông tin cần thiết.
- **Tầm Quan Trọng Của Prompting:** Prompting là kỹ năng quan trọng trong AI, liên quan đến việc xác định văn bản đầu vào để nhận phản hồi mong muốn.

## Lặp Lại Nhanh Chóng Để Tìm Prompt Hiệu Quả

Một cách tìm prompt hiệu quả nhất cho mô hình ngôn ngữ lớn (large language models - LLMs) là lặp lại nhanh chóng và thử nhiều biến thể khác nhau. Ví dụ:

- Nếu phản hồi không đủ hài hước, thử prompt yêu cầu làm cho nó hài hước hơn.
- Nếu quá mơ hồ, sử dụng prompt chỉ định AI không được mơ hồ.  
   Thử nghiệm đa dạng thường mang lại kết quả tốt.

## Thay Đổi Ngữ Cảnh Để Điều Chỉnh Phản Hồi

Bạn có thể thay đổi cách sử dụng LLMs để làm cho phản hồi sáng tạo hơn hoặc cụ thể hơn bằng cách điều chỉnh lượng ngữ cảnh:

- Để phản hồi sáng tạo: Sử dụng prompt ngắn gọn.
- Để phản hồi cụ thể: Cung cấp nhiều ví dụ, giúp LLM tuân thủ chặt chẽ hơn theo các ví dụ đó.

## Kỹ Thuật Chain-of-Thought Prompting

Kỹ thuật prompting chuỗi suy nghĩ (chain-of-thought prompting) yêu cầu mô hình suy luận từng bước cho phản hồi của mình. Ví dụ:

- Khi yêu cầu giải toán, prompt mô hình phân tích thành các bước, thực hiện từng bước một.  
   Việc yêu cầu LLM thực hiện nhiều bước có thể tăng độ chính xác đáng kể.

## Kỹ Thuật Bất Ngờ: Yêu Cầu Mô Hình Phản Ứng Với Phản Hồi Của Chính Nó

Một kỹ thuật thú vị là yêu cầu mô hình đánh giá phản hồi của chính mình. Ví dụ:

- Hỏi mô hình cho phản hồi, sau đó hỏi: "Phản hồi này có mơ hồ không?"
- Nếu trả lời có, loại bỏ phản hồi đó.  
   Điều này cho phép mô hình hỗ trợ một phần công việc đánh giá.

## Lời Khuyên Kết Thúc

Hãy thử nghiệm càng nhiều và sáng tạo càng tốt để đạt kết quả tốt hơn. Theo kịp AI có thể giống như chạy trên máy chạy bộ ngày càng nhanh, với nhiều thay đổi mới, nhưng điều đó cũng làm cho nó thú vị.

---

## Navigation

⬅️ [[03 - 10 - Explore chain-of-thought prompting|Khám phá chain-of-thought prompting]] | [[03 - 12 - Wrap up|Tổng kết Module 3]] ➡️

🏠 [[README|Trang chủ khóa học]]

---

## Chủ Đề Liên Quan

- [[03 - 04 - Write clear and specific prompts|Viết prompt rõ ràng và cụ thể]]
- [[03 - 05 - Prompting best practices|Thực hành tốt nhất cho prompting]]
- [[03 - 08 - Improve AI output through iteration|Cải thiện đầu ra AI qua lặp lại]]
- [[03 - 09 - Discover few-shot prompting|Khám phá few-shot prompting]]
- [[03 - 10 - Explore chain-of-thought prompting|Khám phá chain-of-thought prompting]]

---

## Tóm Tắt Module 3

Thử nghiệm và khám phá các kỹ thuật prompting khác nhau giúp tối ưu hóa hiệu quả sử dụng AI.
