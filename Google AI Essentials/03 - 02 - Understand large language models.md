## Giới thiệu về Mô hình Ngôn ngữ Lớn (LLM)

Hiểu cách hoạt động của mô hình ngôn ngữ lớn (large language model, hoặc LLM) và nhận thức về hạn chế của chúng rất hữu ích. LLM là một mô hình trí tuệ nhân tạo (AI model) được huấn luyện trên lượng lớn văn bản để xác định mẫu hình giữa từ ngữ, khái niệm và cụm từ, từ đó tạo ra phản hồi cho các lệnh (prompt).

## Cách LLM Học và Tạo Phản hồi

LLM được huấn luyện trên hàng triệu nguồn văn bản, bao gồm sách, bài báo, trang web và nhiều hơn nữa. Quá trình huấn luyện giúp mô hình học các mẫu hình và mối quan hệ trong ngôn ngữ con người. Nói chung, dữ liệu chất lượng cao càng nhiều, hiệu suất của mô hình càng tốt.

LLM có khả năng dự đoán từ tiếp theo có khả năng cao nhất trong chuỗi từ, dựa trên việc xác định nhiều mẫu hình trong ngôn ngữ.

## Ví dụ Dự Đoán Từ Tiếp Theo

Xem xét câu chưa hoàn chỉnh: "After it rained, the street was...".  
LLM tính toán xác suất cho các từ có thể tiếp theo:

- "Wet" có xác suất cao.
- "Clean" có xác suất thấp hơn.
- "Dry" có xác suất cực thấp.

Mô hình có thể hoàn thành câu bằng từ có xác suất cao nhất, như "wet" hoặc "damp". Phản hồi của LLM có thể thay đổi mỗi lần sử dụng cùng lệnh.

LLM sử dụng thống kê để phân tích mối quan hệ giữa các từ trong chuỗi và tính xác suất cho hàng nghìn từ có thể tiếp theo. Khả năng dự đoán này cho phép LLM trả lời câu hỏi hoặc yêu cầu, từ việc hoàn thành câu đơn giản đến tạo câu chuyện hấp dẫn cho sản phẩm mới hoặc chiến dịch quảng cáo.

## Hạn Chế của LLM

Mặc dù mạnh mẽ, LLM không phải lúc nào cũng cho kết quả mong muốn do hạn chế trong dữ liệu huấn luyện.

## Thiên Kiến (Bias)

Kết quả của LLM có thể bị thiên kiến vì dữ liệu huấn luyện chứa thiên kiến, chẳng hạn từ bài báo và trang web phản ánh sự thiên vị không công bằng trong xã hội. Ví dụ, LLM có thể liên kết nghề nghiệp chuyên môn với vai trò giới tính cụ thể.

## Hạn Chế Dữ Liệu

LLM có thể không tạo đủ nội dung về lĩnh vực hoặc chủ đề cụ thể nếu dữ liệu huấn luyện thiếu thông tin về chủ đề đó.

## Ảo Giác (Hallucinations)

LLM có xu hướng tạo ra kết quả không đúng sự thật (hallucinations), tức là văn bản không chính xác về mặt sự kiện. Ví dụ, khi tóm tắt lịch sử công ty, LLM có thể đưa ra thông tin sai về ngày thành lập hoặc số lượng nhân viên hiện tại. Các yếu tố góp phần bao gồm chất lượng dữ liệu huấn luyện, cách diễn đạt lệnh, hoặc phương pháp phân tích văn bản và dự đoán từ tiếp theo.

## Đánh Giá và Sử Dụng Hiệu Quả

Vì hạn chế của LLM, cần đánh giá nghiêm ngặt mọi kết quả để kiểm tra tính chính xác sự kiện, không thiên kiến, liên quan đến yêu cầu cụ thể và đầy đủ thông tin. Dù sử dụng AI để tóm tắt báo cáo dài, tạo ý tưởng tiếp thị sản phẩm hay phác thảo kế hoạch dự án, hãy kiểm tra chất lượng kết quả cẩn thận.

Không nên giả định về khả năng của LLM. Ví dụ, nếu nó tạo kết quả chất lượng cao cho thư thuyết phục khách hàng, đừng cho rằng sẽ nhận được kết quả tương tự khi sử dụng lại cùng lệnh trong tương lai.

LLM là công cụ mạnh mẽ cần sự hướng dẫn từ con người để sử dụng hiệu quả. Nhận thức về hạn chế giúp đạt kết quả tốt nhất.

---

## Chủ Đề Liên Quan

- **Cơ bản về AI:** [[01 - 06 - Explore how AI uses machine learning]]
- **Thực hành prompt:** [[03 - 04 - Write clear and specific prompts]]
- **Vấn đề thiên kiến:** [[04 - 02 - Understand bias in AI]]
- **Cải thiện prompt:** [[03 - 08 - Improve AI output through iteration]]

---

## Điều Hướng

**⬅️ Quay lại:** [[03 - 01 - Module 3 introduction - Discover the art of prompting]]

**➡️ Tiếp theo:** [[03 - 03 - Experiment with prompting]]

**🏠 Trang chủ:** [[01 - 01 - Introduction to Google AI Essentials]]
