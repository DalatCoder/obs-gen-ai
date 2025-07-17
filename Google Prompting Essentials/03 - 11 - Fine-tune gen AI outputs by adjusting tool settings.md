# Tinh chỉnh Kết quả [[Glossary - Thuật ngữ Gen AI#Gen AI|Gen AI]] bằng Điều chỉnh Cài đặt Công cụ

> 🧭 **Navigation**: [[03 - 10 - AI IRL - Explore the capabilities and limitations of AI|← Trước]] | [[MOC - Google Prompting Essentials|📚 Mục lục]] | [[04 - 01 - Harness the power of advanced prompting|Tiếp theo →]]

---

## Giới thiệu

Bạn đã bao giờ nhận thấy rằng cùng một prompt có thể tạo ra những kết quả khác nhau không? Điều này xảy ra bởi vì các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) sử dụng sự kết hợp giữa **các mẫu đã học** và **xác suất** để quyết định từ tiếp theo. Nó giống như việc tung xúc xắc để chọn từ, nhưng điều gì sẽ xảy ra nếu bạn có thể **tác động đến kết quả** của lần tung xúc xắc đó?

Một số công cụ như **Google AI Studio** cung cấp bảng điều khiển cho phép bạn điều chỉnh các cài đặt này, thường được gọi là **tham số lấy mẫu** (sampling parameters). Hãy nghĩ về chúng như những **rào chắn hướng dẫn** cho việc lựa chọn từ của AI. Biết khi nào và cách tinh chỉnh những cài đặt này có thể giúp bạn tạo ra kết quả tốt hơn và phù hợp hơn.

## Ba Tham số Chính

## 1. Temperature (Nhiệt độ)

**Temperature** là cài đặt phổ biến nhất và có tác động mạnh nhất trên bảng điều khiển. Hãy nghĩ về nó như **núm điều chỉnh độ sáng tạo** của AI:

## Tăng Temperature

- Tạo ra những phản hồi **sáng tạo và bất ngờ** hơn
- Phù hợp cho các nhiệm vụ nghệ thuật như **brainstorming ý tưởng** hoặc **viết truyện ngắn**

## Giảm Temperature

- Tạo ra kết quả **có thể dự đoán và nhất quán** hơn
- Hữu ích cho các nhiệm vụ đòi hỏi phản hồi **chính xác, dựa trên sự thật** như **tóm tắt báo cáo** hoặc **tạo dòng thời gian**

## Ví dụ Minh họa

Hãy tưởng tượng việc đưa ra prompt cho AI bằng phần đầu của câu: **"This morning, I went to the..."** (Sáng nay, tôi đã đi đến...)

AI phải quyết định từ tiếp theo để hoàn thành câu. Dựa trên việc đào tạo, nó tạo ra danh sách xếp hạng các lựa chọn có khả năng nhất, mỗi từ có điểm xác suất:

- **Cài đặt temperature thấp**: AI trở nên **thận trọng**, chọn từ có điểm số cao nhất, rõ ràng nhất - trong trường hợp này là "grocery store" (cửa hàng tạp hóa)
- **Cài đặt temperature cao**: Khuyến khích AI **chấp nhận rủi ro**, cho các từ có điểm số thấp hơn, bất ngờ hơn như "haunted house" (nhà ma) hoặc "moon" (mặt trăng) cơ hội được chọn

## 2. Top-k và Top-p

Trong khi **temperature** đóng vai trò như núm điều chỉnh sáng tạo chính, hai cài đặt khác giúp bạn tinh chỉnh **nhóm từ** mà công cụ AI có thể chọn: **top-k** và **top-p**.

Hãy nghĩ về chúng như những **núm điều chỉnh tiêu điểm** (focus dials). Chúng hoạt động bằng cách tạo ra danh sách nhỏ hơn, phù hợp hơn về các từ tiềm năng trước khi cài đặt temperature đưa ra lựa chọn sáng tạo.

## Top-k

- Đặt **số lượng từ cố định** mà công cụ có thể chọn
- Ví dụ: đặt top-k = 10 sẽ hướng dẫn công cụ chỉ chọn từ trong top 10 tùy chọn có khả năng nhất

## Top-p

- Đặt **số lượng từ động** mà công cụ có thể chọn
- Hướng dẫn công cụ tự động **thu hẹp hoặc mở rộng** danh sách tùy chọn dựa trên mức độ có thể dự đoán của từ tiếp theo
- Ví dụ: đặt top-p cao (p=0.9) hoạt động như **bộ lọc chất lượng**, hướng dẫn công cụ chỉ xem xét những lựa chọn có khả năng nhất

## Khuyến nghị Sử dụng

- **Top-p** được khuyến nghị điều chỉnh cho hầu hết các trường hợp sử dụng vì nó sẽ **thích ứng với ngữ cảnh** của tình huống
- **Sự khác biệt chính**: top-k sử dụng danh sách có **kích thước cố định**, trong khi top-p sử dụng danh sách có **kích thước linh hoạt**

**Mẹo chuyên nghiệp**: Khi sử dụng top-p, tốt nhất là **để top-k ở cài đặt mặc định**.

## Công thức Thành công

## Công thức 1: Phân tích Tập trung (Focused Analysis)

**Nhiệm vụ**: Tạo ra câu trả lời **dựa trên sự thật, nhất quán và có thể dự đoán**

**Trường hợp sử dụng**:

- Tóm tắt báo cáo
- Trích xuất thông tin chi tiết từ dữ liệu
- Viết tài liệu kỹ thuật
- Tạo code

**Cài đặt**:

- **Temperature**: Thấp (ví dụ: 0.1 đến 0.4)
- **Top-k hoặc Top-p**: Để ở mặc định, vì temperature thấp đã làm cho kết quả rất tập trung

## Công thức 2: Brainstorming Sáng tạo (Creative Brainstorming)

**Nhiệm vụ**: Tạo ra kết quả **đáng ngạc nhiên, đa dạng hoặc sáng tạo**

**Trường hợp sử dụng**:

- Brainstorming ý tưởng mới
- Soạn thảo tài liệu marketing
- Viết truyện hư cấu

**Cài đặt**:

- **Temperature**: Cao (ví dụ: 0.8 đến 1.0)
- **Top-k hoặc Top-p**: Giá trị cao (như 0.95 cho top-p) có thể hữu ích để cho công cụ AI **tự do sáng tạo** trong khi vẫn lọc ra các tùy chọn không liên quan

## Lưu ý Quan trọng

## Về Hallucinations (Ảo giác)

Với cả ba cài đặt, **điểm số cao** có thể tạo ra những **insight đáng ngạc nhiên**, nhưng chúng cũng **tăng khả năng tạo ra thông tin không chính xác** hoặc **ảo giác** (hallucinations).

**Quan trọng**: Luôn **xem xét và kiểm tra sự thật** của kết quả, đặc biệt khi sử dụng các cấu hình sáng tạo.

## Kết luận

Một **prompt tuyệt vời chỉ là điểm khởi đầu** - không phải điểm đến. Chìa khóa là tìm ra **sự cân bằng phù hợp** giữa câu trả lời sáng tạo và có thể dự đoán.

- **[[Glossary - Thuật ngữ Gen AI#Temperature|Temperature]]** là núm điều chỉnh độ sáng tạo của bạn

---

> 📚 **Thuật ngữ liên quan**: [[Glossary - Thuật ngữ Gen AI#Temperature|Temperature]] | [[Glossary - Thuật ngữ Gen AI#Sampling Parameters|Sampling Parameters]] | [[Glossary - Thuật ngữ Gen AI#Top-k|Top-k]] | [[Glossary - Thuật ngữ Gen AI#Top-p|Top-p]]
>
> 🔗 **Xem thêm**: [[01 - 17 - AI IRL - Discover strategies to mitigate hallucinations|Giảm thiểu hallucinations]] | [[04 - 01 - Harness the power of advanced prompting|Advanced prompting]]
>
> 🎯 **Thực hành**: [[01 - 05 - Use the 5-step prompt framework|Framework prompting]] | [[01 - 16 - Use gen Ai responsibly|Sử dụng AI có trách nhiệm]]

- **Top-p và top-k** giúp bạn giữ cho sự sáng tạo đó **tập trung**

Bằng cách học cách sử dụng những điều khiển đơn giản này, bạn có thể **vượt xa prompting tuyệt vời** để tạo ra kết quả tốt hơn cho bất kỳ nhiệm vụ nào.
