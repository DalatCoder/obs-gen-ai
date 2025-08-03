## Mẹo để tạo prompt có trách nhiệm (Responsible Prompting)

### Rủi ro đạo đức và hạn chế của AI

Các công cụ AI tạo sinh (generative AI) không hoàn hảo và thiếu kỹ năng tư duy phản biện cũng như nhận thức con người. Kết quả đầu ra có thể chứa:

- Sai lầm và thông tin sai lệch
- Thiên kiến (bias) và khuôn mẫu (stereotypes)
- Nội dung có hại

**Quan trọng:** Luôn áp dụng phương pháp "con người trong vòng lặp" (human-in-the-loop) - phải xác minh kết quả AI trước khi sử dụng.

### Thiên kiến và khuôn mẫu (Biases and Stereotypes)

AI có thể tái tạo các thiên kiến hiện có về nhóm người cụ thể, gây ra kỳ thị về tuổi tác, chủng tộc, hay giới tính.

**Cách tránh:**

- **Chỉ định tính đa dạng:** Thêm ngôn ngữ bao hàm vào prompt
    - Thay vì: "một bàn thức ăn ngon"
    - Nên viết: "một bàn thức ăn ngon từ khắp nơi trên thế giới"
- **Thách thức các giả định:** Khi AI đưa ra phản hồi thiên kiến, hãy chỉ ra khuôn mẫu và yêu cầu sửa lại
    - Ví dụ: Nếu hình ảnh chỉ hiển thị món ăn Đông Nam Á, yêu cầu bổ sung món ăn từ Tây Phi hoặc Bắc Âu


### Ảo giác (Hallucinations)

Khi AI cung cấp thông tin sai lệch được gọi là "ảo giác". Thường xảy ra khi:

- Nhận được hướng dẫn mơ hồ, không rõ ràng
- Tạo ra nội dung về chủ đề chưa được đào tạo tốt

**Cách xử lý:**

- **Kiểm tra chéo thông tin:** Sử dụng công cụ tìm kiếm hoặc tham khảo chuyên gia để xác minh
- **Chạy prompt qua nhiều nguồn:** Giúp phát hiện các sự khác biệt trong kết quả
- **Sử dụng ngôn ngữ rõ ràng hơn:** Tránh nhập liệu sai hoặc mơ hồ
    - Ví dụ sai: "Tại sao Toronto là thủ đô Canada?" (thực tế Ottawa mới là thủ đô)


### Sự không nhất quán và vấn đề liên quan (Inconsistencies)

AI có thể hiểu sai ngữ cảnh hoặc diễn giải theo nghĩa đen các thành ngữ.

**Giải pháp:**

- **Cung cấp tài liệu tham khảo:** Sử dụng bước References trong framework prompting
- **Bổ sung ngữ cảnh:** Diễn đạt lại prompt rõ ràng hơn
    - Thay vì: "think outside the box"
    - Nên viết: "xem xét các cách tiếp cận độc đáo, không theo lối mòn"


### Cân nhắc khi sử dụng trong công việc

Trước khi sử dụng AI cho công việc, cần tự hỏi:

- Việc này có phù hợp với mục tiêu và nghĩa vụ với đồng nghiệp, khách hàng?
- Chính sách công ty về việc sử dụng AI là gì?
- Có rủi ro rò rỉ dữ liệu nhạy cảm không?
- Công cụ AI này là nội bộ riêng tư hay công khai?


### Danh sách kiểm tra sử dụng AI có trách nhiệm

- **Đánh giá tác động:** Cân nhắc hiệu ứng khi sử dụng AI, có gây thiên kiến hay tổn hại không
- **Xin phép sử dụng:** Được sự đồng ý từ cấp có thẩm quyền trước khi dùng AI cho dự án
- **Xem xét bảo mật:** Kiểm tra tính riêng tư và bảo mật của công cụ AI
- **Đánh giá nội dung:** Xác minh tất cả nội dung do AI tạo trước khi sử dụng
- **Minh bạch:** Tiết lộ việc sử dụng AI với nhóm và khách hàng


### Xóa bộ nhớ (Clearing Memory)

Định kỳ xóa bộ nhớ AI mang lại nhiều lợi ích:

- **Bảo vệ quyền riêng tư:** Loại bỏ thông tin nhạy cảm từ các tương tác trước
- **Tránh thiên kiến:** Ngăn AI mang theo các giả định từ prompt cũ
- **Giảm nhầm lẫn:** Đảm bảo AI tập trung vào nhiệm vụ hiện tại
- **Khắc phục sự cố:** Làm mới khi AI bị "kẹt" hoặc cho kết quả bất thường

**Lưu ý:** Một số công cụ tự động xóa bộ nhớ mỗi lần mở, do đó không ghi nhớ các câu hỏi trước.

**Liên kết:** [[Generative AI]], [[Human-in-the-loop]], [[Bias]], [[Hallucinations]], [[Responsible AI]], [[Prompting Framework]], [[Context]], [[References]], [[Critical Thinking]]

