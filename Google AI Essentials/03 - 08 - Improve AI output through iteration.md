## Quy Trình Lặp Lại Trong Thiết Kế Prompt (Iterative Process in Prompt Engineering)

Quy trình lặp lại (iterative process) liên quan đến việc tạo phiên bản đầu tiên, đánh giá và cải thiện để đạt kết quả mong muốn. Ví dụ, khi phát triển đề xuất, báo cáo hoặc tài liệu, bạn có thể tạo nhiều bản nháp và cải thiện từng bản đến khi hài lòng. Cách tiếp cận này hiệu quả để giải quyết vấn đề hoặc phát triển sản phẩm.

Trong kỹ thuật thiết kế prompt (prompt engineering), quy trình lặp lại cũng rất hiệu quả, thường yêu cầu nhiều lần thử để có kết quả tối ưu. Nếu lần đầu không thành công, đừng nản lòng; hãy đánh giá kết quả để xác định lý do và chỉnh sửa prompt.

## Lý Do Có Thể Không Nhận Được Kết Quả Hữu Ích Dù Prompt Rõ Ràng

1. **Sự Khác Biệt Giữa Các Mô Hình Ngôn Ngữ Lớn (LLM)**: Mỗi mô hình ngôn ngữ lớn (LLM) được phát triển với dữ liệu huấn luyện và kỹ thuật lập trình độc đáo, dẫn đến kiến thức nền khác nhau về các lĩnh vực cụ thể. Do đó, các mô hình có thể phản hồi khác nhau với prompt tương tự và có thể không cung cấp phản hồi đầy đủ.
2. **Hạn Chế Của LLM**: Kết quả có thể không chính xác, thiên kiến, thiếu thông tin, không liên quan hoặc không nhất quán.

## Đánh Giá Kết Quả LLM

Đánh giá nghiêm ngặt mọi kết quả bằng cách tự hỏi:

- Kết quả có chính xác không?
- Kết quả có không thiên kiến không?
- Kết quả có đủ thông tin không?
- Kết quả có liên quan đến dự án hoặc nhiệm vụ không?
- Kết quả có nhất quán nếu sử dụng cùng prompt nhiều lần không?

Nếu phát hiện vấn đề, lặp lại prompt để giải quyết và cải thiện kết quả.

## Cải Thiện Prompt Thông Qua Lặp Lại

- Nếu thiếu ngữ cảnh, hãy thêm vào prompt.
- Lựa chọn từ ngữ ảnh hưởng lớn đến kết quả; thử nghiệm cách diễn đạt khác nhau để có phản hồi tốt hơn.  
   Sử dụng quy trình lặp lại với LLM cụ thể để đạt kết quả tốt nhất.

## Ví Dụ: Tìm Kiếm Các Trường Đại Học Ở Pennsylvania Với Chương Trình Hoạt Hình

Giả sử bạn là điều phối viên nhân sự tại công ty sản xuất video ở Pennsylvania, Mỹ. Công ty muốn phát triển chương trình thực tập cho sinh viên khám phá sự nghiệp trong thiết kế đồ họa chuyển động và hoạt hình, hợp tác với các trường đại học địa phương. Bước đầu: Tạo danh sách các trường ở Pennsylvania có chương trình hoạt hình, với chi tiết cần thiết và định dạng dễ xem xét.

Prompt ban đầu (sử dụng Gemini): "Help me find colleges with animation programs in Pennsylvania."  
(Dịch: Giúp tôi tìm các trường đại học có chương trình hoạt hình ở Pennsylvania.)

Kết quả: Danh sách các trường và thông tin chương trình, nhưng không có cấu trúc, khó tham khảo nhanh (ví dụ cho quản lý bận rộn).

Prompt lặp lại: "Show these options as a table."  
(Dịch: Hiển thị các lựa chọn này dưới dạng bảng.)

Kết quả: Bảng với thông tin về vị trí trường và loại bằng cấp, dễ theo dõi hơn.

Prompt lặp lại tiếp theo: "Can you add a column showing whether they're public or private?"  
(Dịch: Bạn có thể thêm cột hiển thị xem chúng là công lập hay tư thục không?)

Kết quả: Bảng bổ sung cột công lập/tư thục. Để chia sẻ, sử dụng tính năng Export to Sheets để đội ngũ dễ truy cập và phân tích dữ liệu.

## Lời Khuyên Thêm

Áp dụng cách tiếp cận lặp lại cho các nhiệm vụ khác. Lưu ý rằng prompt trước trong cùng cuộc trò chuyện có thể ảnh hưởng đến kết quả prompt mới; nếu vậy, bắt đầu cuộc trò chuyện mới.

Quy trình lặp lại là phần quan trọng của kỹ thuật thiết kế prompt, giúp tận dụng LLM để có kết quả hữu ích nhất.

---

## Navigation

⬅️ [[03 - 07 - Prompts for different purposes|Prompts cho các mục đích khác nhau]] | [[03 - 09 - Discover few-shot prompting|Khám phá few-shot prompting]] ➡️

🏠 [[README|Trang chủ khóa học]]

---

## Chủ Đề Liên Quan

- [[02 - 10 - Leverage the human-in-the-loop approach to AI|Tận dụng cách tiếp cận human-in-the-loop]]
- [[03 - 04 - Write clear and specific prompts|Viết prompt rõ ràng và cụ thể]]
- [[03 - 05 - Prompting best practices|Thực hành tốt nhất cho prompting]]
- [[03 - 07 - Prompts for different purposes|Prompts cho các mục đích khác nhau]]
- [[03 - 11 - Improve prompts through exploration|Cải thiện prompts thông qua khám phá]]

---

## Tóm Tắt Module 3

Lặp lại và cải thiện prompt là kỹ năng quan trọng để tối đa hóa hiệu quả của AI trong công việc.
