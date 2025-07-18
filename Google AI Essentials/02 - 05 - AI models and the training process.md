## Ghi Chú Học Tập: Mô Hình Trí Tuệ Nhân Tạo (AI Models) Và Quy Trình Huấn Luyện

## Giới Thiệu

- Bạn đã khám phá cách công cụ trí tuệ nhân tạo (AI tools) được cung cấp bởi mô hình trí tuệ nhân tạo (AI models).
- Bài đọc này giúp hiểu sâu hơn về cách phát triển mô hình trí tuệ nhân tạo (AI models), bao gồm quy trình lặp lại mà nhà thiết kế và kỹ sư trí tuệ nhân tạo (AI designers and engineers) sử dụng để huấn luyện mô hình từ dữ liệu, đảm bảo công cụ trí tuệ nhân tạo (AI tools) hoạt động đáng tin cậy.
- Hiểu về cơ chế nội tại của công cụ trí tuệ nhân tạo (AI tools) giúp thảo luận chính xác và tự tin hơn.

## Sự Khác Biệt Giữa Công Cụ Trí Tuệ Nhân Tạo (AI Tools) Và Mô Hình Trí Tuệ Nhân Tạo (AI Models)

- Công cụ trí tuệ nhân tạo (AI tools): Phần mềm được hỗ trợ bởi trí tuệ nhân tạo (AI-powered software) để tự động hóa hoặc hỗ trợ người dùng trong các nhiệm vụ đa dạng.
- Mô hình trí tuệ nhân tạo (AI models): Chương trình máy tính được huấn luyện trên tập dữ liệu để nhận diện mẫu và thực hiện nhiệm vụ cụ thể.
- So sánh ẩn dụ: Giống như xe hơi (công cụ trí tuệ nhân tạo - AI tool) và động cơ (mô hình trí tuệ nhân tạo - AI model).
  - Xe hơi có giao diện thân thiện (như tay lái và bảng điều khiển) đại diện cho công cụ trí tuệ nhân tạo (AI tool), giúp đạt mục tiêu (nhiệm vụ hoàn thành hoặc đầu ra mong muốn).
  - Động cơ ẩn dưới xử lý thông tin đầu vào, cho phép công cụ hoạt động.
- Công cụ trí tuệ nhân tạo (AI tools) được phát triển cho nhiều ứng dụng, như tạo văn bản sáng tạo, hình ảnh, video hoặc mã lập trình.
- Mô hình trí tuệ nhân tạo (AI models) là yếu tố cốt lõi thực hiện công việc nặng, cung cấp năng lực cho công cụ.
- Lưu ý: Một số công cụ trí tuệ nhân tạo (AI tools) sử dụng nhiều mô hình trí tuệ nhân tạo (AI models) hoạt động như "gia đình" để tăng tính linh hoạt và thực hiện nhiều nhiệm vụ. Mỗi mô hình có thể chuyên biệt cho một subtasks. Các công cụ đa phương thức (multimodal tools) sẽ được khám phá sau trong khóa học.

## Quy Trình Huấn Luyện Mô Hình Trí Tuệ Nhân Tạo (AI Models)

- Nhà thiết kế và kỹ sư trí tuệ nhân tạo (AI designers and engineers) phát triển mô hình qua quy trình gọi là huấn luyện (training).
- Ví dụ: Xây dựng mô hình dự đoán mưa để giúp mọi người tránh ướt khi đi làm.
- Các bước điển hình:
  1. **Xác định vấn đề cần giải quyết (Define the problem)**: Xem xét khả năng và hạn chế của trí tuệ nhân tạo (AI) để xác định giải pháp, ví dụ dự đoán mưa để tránh ướt khi di chuyển.
  2. **Thu thập dữ liệu liên quan (Collect relevant data)**: Thu thập dữ liệu lịch sử về ngày mưa và không mưa trong 50 năm qua.
  3. **Chuẩn bị dữ liệu (Prepare the data)**: Gắn nhãn các đặc trưng quan trọng (như nhiệt độ ngoài trời, độ ẩm, áp suất không khí) và ghi chú liệu có mưa hay không. Phân chia dữ liệu thành tập huấn luyện (training set) và tập xác thực (validation set) để kiểm tra sau.
  4. **Huấn luyện mô hình (Train the model)**: Áp dụng chương trình học máy (machine learning - ML programs) vào dữ liệu huấn luyện. Chương trình học cách nhận diện mẫu, như sự kết hợp nhiệt độ cao, áp suất thấp và độ ẩm cao chỉ báo mưa.
  5. **Đánh giá mô hình (Evaluate the model)**: Sử dụng tập xác thực để kiểm tra độ chính xác và đáng tin cậy. Phân tích hiệu suất để phát hiện vấn đề như dữ liệu huấn luyện không đủ hoặc thiên kiến (biased). Nếu có vấn đề, quay lại bước trước để điều chỉnh.
  6. **Triển khai mô hình (Deploy the model)**: Khi hài lòng, tích hợp vào công cụ trí tuệ nhân tạo (AI tool) để sử dụng thực tế, ví dụ giúp mọi người tránh mưa khi đi làm.
- Quy trình huấn luyện là lặp lại (iterative process): Lặp lại các bước và điều chỉnh để tạo mô hình tốt nhất.
- Sau triển khai: Giám sát liên tục, thu thập phản hồi từ người dùng để xử lý thách thức mới, đảm bảo hiệu suất đáng tin cậy và cải thiện.
- Kết quả: Quy trình tinh chỉnh liên tục làm mô hình chính xác và linh hoạt, dẫn đến công cụ trí tuệ nhân tạo (AI tools) hiệu quả và đáng tin cậy.
- Lợi ích: Hiểu quy trình giúp quyết định thông minh về thời điểm và cách sử dụng công cụ trí tuệ nhân tạo (AI tools) để đạt mục tiêu.

---

## Chủ Đề Liên Quan

- **ML fundamentals:** [[01 - 06 - Explore how AI uses machine learning]]
- **Training data & bias:** [[04 - 02 - Understand bias in AI]]
- **AI tools work:** [[02 - 04 - Understand how AI tools work]]
- **Model improvement:** [[02 - 11 - Explore how people improve AI models]]
- **LLM training:** [[03 - 02 - Understand large language models]]

---

## Điều Hướng

**⬅️ Quay lại:** [[02 - 04 - Understand how AI tools work]]

**➡️ Tiếp theo:** [[02 - 06 - Transform your work with generative AI]]

**🏠 Trang chủ:** [[01 - 01 - Introduction to Google AI Essentials]]
