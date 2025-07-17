# [[Glossary - Thuật ngữ Gen AI#Prompt Chaining|Prompt Chaining]] - Kỹ thuật Chuỗi Prompt

> 🧭 **Navigation**: [[04 - 01 - Use AI to untangle complex tasks|← Trước]] | [[MOC - Google Prompting Essentials|📚 Mục lục]] | [[04 - 03 - Explore Chain-of-thought and Tree-of-though prompting|Tiếp theo →]]

---

## Khái niệm cơ bản

**Prompt chaining** (chuỗi prompt) giống như việc ghép tranh xếp hình - bạn không thể đổ tất cả mảnh ghép ra và hy vọng may mắn. Thay vào đó, bạn cần có kế hoạch cụ thể: tìm các mảnh góc, xây dựng viền trước, sau đó làm phần giữa, hoặc hoàn thành từng phần nhỏ rồi kết nối chúng lại.

Prompt chaining là kỹ thuật **hướng dẫn trí tuệ nhân tạo tạo sinh (Gen AI)** thông qua một chuỗi các prompt liên kết với nhau, mỗi bước đều bổ sung thêm ngữ cảnh hoặc nhiệm vụ mới. Cuối cùng, các prompt liên kết này giúp công cụ AI giải quyết các vấn đề phức tạp từng bước một.

## Ví dụ ứng dụng thực tế

Khi bạn nghỉ phép và cần cập nhật công việc:

1. **Bước 1**: Prompt AI tóm tắt email và tài liệu nhận được
2. **Bước 2**: Sau khi xem xét đầu ra, prompt tiếp để tập trung vào các yêu cầu cấp thiết
3. **Bước 3**: Nếu phát hiện vấn đề khẩn cấp, prompt thêm để tìm giải pháp xử lý

**Điểm khác biệt**: Với kỹ thuật này, bạn không chỉ đơn thuần lặp lại, mà **mỗi prompt và phản hồi đều xây dựng dựa trên cái trước đó**, tạo thành một chuỗi prompt liên tiếp trong một chuỗi duy nhất.

## Thực hành với Google AI Studio

## Bối cảnh: Tiếp thị một cuốn tiểu thuyết

Giả sử bạn vừa hoàn thành một cuốn tiểu thuyết và cần tạo kế hoạch tiếp thị. Chúng ta sẽ sử dụng **Google AI Studio** vì nó cho phép truy cập các mô hình Gemini với **long context window** (cửa sổ ngữ cảnh dài).

## Bước 1: Tạo tagline hấp dẫn

**Prompt:**

text

`Generate three options for a one sentence summary of this novel manuscript. The manuscript will provide the story's background information directly, so let's just specify the tone. The summary should be similar in voice and tone to the manuscript, but more catchy and engaging.`

_(Tạo ba lựa chọn cho bản tóm tắt một câu của bản thảo tiểu thuyết này. Bản thảo sẽ cung cấp trực tiếp thông tin bối cảnh câu chuyện, vì vậy chúng ta chỉ cần chỉ định giọng điệu. Bản tóm tắt nên có giọng điệu tương tự bản thảo nhưng hấp dẫn và cuốn hút hơn.)_

## Bước 2: Tinh chỉnh tagline

**Prompt:**

text

`Create a tagline that is a combination of the previous three options with a special focus on the exciting plot twists and mystery of the book. There's the new context. Find the catchiest and most impactful combination. The tagline should be concise and leave the reader hooked and wanting to read more.`

_(Tạo một tagline kết hợp ba lựa chọn trước đó với trọng tâm đặc biệt vào những tình tiết bất ngờ thú vị và bí ẩn của cuốn sách. Đây là ngữ cảnh mới. Tìm sự kết hợp hấp dẫn và có tác động nhất. Tagline nên ngắn gọn và khiến độc giả bị cuốn hút, muốn đọc tiếp.)_

## Bước 3: Tạo nội dung bìa sau

**Prompt:**

text

`Create a five sentence summary of the entire manuscript below that expands on the one sentence summary.`

_(Tạo bản tóm tắt năm câu cho toàn bộ bản thảo dưới đây, mở rộng từ bản tóm tắt một câu.)_

## Bước 4: Lên kế hoạch book tour

**Prompt:**

text

`Generate a six week promotional plan for a book tour, including what locations I should visit and what channels I should utilize to promote each stop on the tour.`

_(Tạo kế hoạch quảng bá sáu tuần cho book tour, bao gồm những địa điểm tôi nên ghé thăm và những kênh nào tôi nên sử dụng để quảng bá cho mỗi điểm dừng trong tour.)_

## Điểm khác biệt quan trọng

**Prompt chaining khác với iteration:**

- **Iteration** (lặp lại): Tập trung vào việc điều chỉnh một prompt cụ thể để cải thiện kết quả
- **Prompt chaining**: Sử dụng đầu ra của AI làm **khối xây dựng** cho các yêu cầu phức tạp hơn, mở rộng dựa trên những gì AI đã tạo ra trước đó

## Lợi ích của kỹ thuật này

Với chỉ một chuỗi prompt, bạn có thể hướng dẫn mô hình [[Glossary - Thuật ngữ Gen AI#Gemini|Gemini]] trong [[Glossary - Thuật ngữ Gen AI#Google AI Studio|AI Studio]] tạo ra:

- **Tagline** hấp dẫn
- **Bản tóm tắt** chi tiết
- **Kế hoạch book tour** hoàn chỉnh

---

> 📚 **Thuật ngữ liên quan**: [[Glossary - Thuật ngữ Gen AI#Prompt Chaining|Prompt Chaining]] | [[Glossary - Thuật ngữ Gen AI#Long Context Window|Long Context Window]] | [[Glossary - Thuật ngữ Gen AI#Sequential Prompting|Sequential Prompting]]
>
> 🔗 **Xem thêm**: [[04 - 03 - Explore Chain-of-thought and Tree-of-though prompting|Chain-of-thought prompting]] | [[04 - 04 - Simplify multi-step projects with prompt chaining|Multi-step projects]]
>
> 🎯 **Thực hành**: [[01 - 09 - Practice 4 iteration methods|Phương pháp iteration]] | [[04 - 06 - Use meta-prompting to improve and generate new prompts|Meta-prompting]]

Tất cả đều được xây dựng dựa trên **long context window** (cửa sổ ngữ cảnh dài), giúp mô hình ghi nhớ cuộc hội thoại và phân tích bản thảo một cách liên tục.

_Lưu ý: Bạn vẫn có thể lặp lại (iterate) bất kỳ prompt nào nếu không hài lòng với kết quả mà công cụ trí tuệ nhân tạo tạo sinh (Gen AI) cung cấp._
