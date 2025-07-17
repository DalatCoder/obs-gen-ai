# Hướng dẫn Prompting có trách nhiệm

## Tổng quan

Đôi khi các công cụ **trí tuệ nhân tạo tạo sinh (Gen AI)** không thể đưa ra kết quả đầu ra mà bạn cần. Có lý do cho điều này. Các công cụ Gen AI rất giỏi trong việc xử lý thông tin và nhận dạng mẫu (pattern recognition), nhưng thiếu **kỹ năng tư duy phản biện** (critical-thinking skills) và **nhận thức con người** (human awareness). Đó là lý do tại sao việc học cách prompting có trách nhiệm khi sử dụng các công cụ Gen AI là quan trọng.

## Rủi ro đạo đức và hạn chế của AI

## Nhận thức về không hoàn hảo

Các công cụ Gen AI **không hoàn hảo**. Đôi khi, kết quả đầu ra của chúng có thể chứa:

- **Sai lầm** (mistakes)
    
- **Thiên vị** (bias)
    
- **Định kiến** (stereotypes)
    
- **Thông tin sai lệch** (misleading information)
    
- **Nội dung có hại khác** (harmful content)
    

## Tầm quan trọng của phương pháp "Human-in-the-loop"

Đây là lý do tại sao cách tiếp cận **"con người trong vòng lặp" (human-in-the-loop)** rất quan trọng - bạn **phải xác minh kết quả đầu ra** của Gen AI trước khi sử dụng chúng.

## Xử lý thiên vị và định kiến

## Nguyên nhân và tác động

Các công cụ Gen AI đôi khi có thể **tái tạo thiên vị hiện có** về một số nhóm người, như kết nối các hoạt động cụ thể với độ tuổi nhất định. Điều này **củng cố các định kiến có hại** (harmful stereotypes).

## Chiến lược tránh thiên vị

## 1. Chỉ định sự đa dạng (Specify diversity)

**Thêm ngôn ngữ bao trùm** (inclusive language) vào prompt của bạn.

**Ví dụ:**

- **Thay vì:** "một bàn thức ăn ngon"
    
- **Nên viết:** "một bàn thức ăn ngon từ khắp nơi trên thế giới"
    
- **Hoặc:** Mô tả thức ăn từ một khu vực địa lý hoặc ẩm thực cụ thể
    

**Lợi ích:**

- Tạo ra kết quả đầu ra tốt hơn
    
- Có nhiều quyền kiểm soát hơn
    

## 2. Thách thức các giả định (Challenge assumptions)

**Khi Gen AI đưa ra phản hồi thiên vị:**

- **Chỉ ra định kiến** khi bạn lặp lại (iterate) prompt
    
- **Yêu cầu công cụ sửa chữa thiên vị**
    

**Ví dụ thực tế:**

- Prompt tạo hình ảnh thức ăn ngon → nhận được nhiều món ăn từ cùng một khu vực thế giới
    
- **Hành động:** Chỉ ra sự thiếu đa dạng trong hình ảnh
    
- **Lặp lại:** Yêu cầu hình ảnh đa dạng hơn
    

**Ví dụ cụ thể:**

- Nhận thấy hầu hết thức ăn trong hình là món Đông Nam Á
    
- **Phản hồi:** Yêu cầu Gen AI bao gồm thêm thức ăn từ Tây Phi hoặc Bắc Âu
    

**Lợi ích thêm:** Việc cung cấp phản hồi cũng có thể giúp cải thiện các kết quả đầu ra trong tương lai của công cụ Gen AI.

## Xử lý ảo giác AI (Hallucinations)

## Định nghĩa và nguyên nhân

**Ảo giác AI (Hallucinations)** là khi công cụ Gen AI cung cấp kết quả đầu ra có **thông tin sai**.

**Ảo giác có thể xảy ra:**

- Bất cứ lúc nào
    
- Khi Gen AI nhận được **hướng dẫn mơ hồ hoặc không rõ ràng**
    
- Khi tạo ra kết quả đầu ra về thứ gì đó mà nó **chưa được đào tạo tốt**
    

**Ví dụ:**

- Tính toán sai bài toán
    
- Bao gồm thành phần không chính xác cho công thức nấu ăn
    

## Chiến lược xử lý ảo giác

## 1. Kiểm tra sự thật và tham chiếu chéo (Fact-check and cross-reference)

**Các phương pháp:**

- **Sử dụng tính năng tích hợp:** Một số công cụ Gen AI có tính năng cung cấp nguồn thông tin
    
- **Kiểm tra bằng công cụ tìm kiếm:** Sử dụng search engine để xác nhận thông tin
    
- **Tham khảo chuyên gia:** Nhờ sự giúp đỡ của chuyên gia nếu có thể
    
- **Chạy prompt qua nhiều nguồn:** Giúp xác định sự khác biệt có thể có trong kết quả đầu ra
    

## 2. Sử dụng ngôn ngữ rõ ràng và chi tiết hơn

**Vấn đề có thể xảy ra:**

- Gen AI hiểu sai thứ gì đó trong input của bạn
    
- Input sai có thể ảnh hưởng đến cách Gen AI xử lý nó
    

**Ví dụ về input sai:**

- **Câu hỏi:** "Tại sao Toronto là thủ đô của Canada?"
    
- **Kết quả:** Gen AI có thể sử dụng input như thể nó đúng và đưa ra lịch sử sai về việc Canada chọn Toronto thay vì Ottawa làm trung tâm chính phủ
    

## Xử lý sự không nhất quán và vấn đề liên quan

## Nguyên nhân

Mặc dù các công cụ Gen AI đang phát triển nhanh chóng, đôi khi chúng sẽ:

- **Diễn giải sai input** của bạn
    
- **Hiểu sai bối cảnh** của yêu cầu
    

## Ví dụ về hiểu sai

**Thành ngữ hoặc cụm từ thông tục:**

- **Input:** "think outside the box"
    
- **Vấn đề:** Gen AI có thể hiểu cụm từ bóng bẩy này theo nghĩa đen
    
- **Kết quả:** Đề xuất các giải pháp về mặt ngoài của hộp
    

## Chiến lược xử lý

## 1. Cung cấp tài liệu tham khảo (Provide references)

- Đây là nơi bước **References** trong prompting framework thực sự hữu ích
    
- **Lưu ý:** Đảm bảo các tài liệu tham khảo bạn cung cấp **đại diện cho kết quả đầu ra mong muốn**
    

## 2. Cung cấp thêm bối cảnh (Provide more context)

**Có thể cần:**

- Cung cấp thêm **bối cảnh và chi tiết**
    
- **Diễn đạt lại** prompt của bạn
    

**Ví dụ cải thiện:**

- **Thay vì:** "think outside the box"
    
- **Nên viết:** "xem xét các cách tiếp cận độc đáo, không thông thường" về chủ đề đang bàn
    

## Prompting có trách nhiệm và cân nhắc nơi làm việc

## Đánh giá sự phù hợp

Các công cụ Gen AI **không phù hợp cho mọi tình huống**. Quan trọng là cần xem xét một số điều trước khi thiết kế prompt để giúp việc liên quan đến công việc.

## Các câu hỏi cần tự hỏi

**Về vấn đề và mục tiêu:**

- Vấn đề bạn đang sử dụng Gen AI để giải quyết có **phù hợp với mục tiêu và nghĩa vụ** đối với đồng nghiệp và khách hàng không?
    

**Về chính sách công ty:**

- **Chính sách công ty** về việc sử dụng AI là gì?
    

**Về bảo mật:**

- Bạn có **đang đặt dữ liệu nhạy cảm vào tình huống rủi ro** không?
    
- Công cụ Gen AI bạn đang sử dụng là **công cụ nội bộ riêng tư hay công cụ công cộng**?
    

## Nguyên tắc cơ bản

**Luôn giữ cách tiếp cận "human-in-the-loop"** ở vị trí hàng đầu trong cách bạn sử dụng AI. Điều này có nghĩa là **con người xác minh kết quả đầu ra** của công cụ Gen AI trước khi chúng được sử dụng ở bất kỳ đâu - dù ở nhà, ở nơi làm việc, hay nơi khác.

## Danh sách kiểm tra sử dụng Gen AI có trách nhiệm tại nơi làm việc

## 1. Xem xét tác động và sử dụng phán đoán tốt nhất

- **Xem xét tác động** của việc sử dụng AI để giải quyết vấn đề hoặc nhiệm vụ
    
- **Luôn sử dụng phán đoán tốt nhất** và kỹ năng tư duy phản biện
    
- **Tự hỏi:** AI có phù hợp cho nhiệm vụ bạn đang làm không?
    

**Ví dụ cân nhắc:**

- Công cụ Gen AI có **củng cố hoặc duy trì thiên vị** có thể gây tổn hại cho một nhóm người cụ thể không?
    

## 2. Xin phê duyệt

**Xin phê duyệt** sử dụng AI từ những người thích hợp trong công ty trước khi sử dụng Gen AI cho các dự án hoặc với khách hàng.

## 3. Cân nhắc về quyền riêng tư và bảo mật

**Xem xét ý nghĩa về quyền riêng tư và bảo mật** của công cụ Gen AI bạn đang sử dụng:

- Công cụ công cộng hay độc quyền?
    
- **Kiểm tra** xem công ty có phiên bản doanh nghiệp (enterprise version) của công cụ Gen AI cho phép sử dụng trong các trường hợp khác không
    

## 4. Đánh giá tất cả nội dung do AI tạo ra

**Đánh giá tất cả nội dung do AI tạo ra** trước khi đưa vào công việc hoặc chia sẻ với bất kỳ ai.

## 5. Tiết lộ việc sử dụng AI

**Tiết lộ việc sử dụng AI** của bạn cho team và khách hàng, và **minh bạch** về cách bạn sử dụng nó.

## Khi nghi ngờ, hãy xóa bộ nhớ

## Lợi ích của việc xóa bộ nhớ

**Định kỳ xóa bộ nhớ** (clearing memory) của công cụ Gen AI là một cách tuyệt vời khác để cải thiện độ chính xác và tính liên quan của kết quả đầu ra.

**Xóa bộ nhớ mang lại:**

- **Khởi đầu mới** cho công cụ
    
- Cho phép tiếp cận prompts mới với **bảng trắng** (clean slate)
    

## Các lợi ích khác của việc xóa bộ nhớ

## 1. Bảo vệ quyền riêng tư (Protecting privacy)

- Loại bỏ thông tin nhạy cảm có thể có từ các tương tác trước đó
    

## 2. Tránh thiên vị (Avoiding bias)

- Ngăn công cụ mang theo các giả định hoặc định kiến từ các prompts trước đó
    

## 3. Giảm nhầm lẫn (Reducing confusion)

- Đảm bảo công cụ chỉ tập trung vào nhiệm vụ và bối cảnh hiện tại
    

## 4. Khắc phục sự cố (Troubleshooting)

- Làm mới công cụ khi nó có vẻ bị kẹt hoặc tạo ra kết quả bất ngờ
    

## Hướng dẫn thực hiện

**Các công cụ khác nhau** có hướng dẫn khác nhau để xóa bộ nhớ:

- **Kiểm tra cài đặt** (settings) để tìm hướng dẫn về cách thực hiện
    

**Lưu ý quan trọng:**

- Một số công cụ **tự động xóa bộ nhớ** mỗi khi bạn mở nó
    
- Do đó không nhớ những gì bạn đã hỏi trước đó
    

## Kết luận

**AI là một công cụ mạnh mẽ** - đó là lý do tại sao việc sử dụng nó một cách **cẩn thận và có trách nhiệm** là quan trọng.

## Các nguyên tắc cốt lõi

**Sử dụng AI có trách nhiệm có nghĩa là:**

- **Chú ý đến các rủi ro đạo đức** (ethical risks)
    
- **Thừa nhận các hạn chế của AI** (AI limitations)
    
- **Tính đến thiên vị** (biases)
    

## Công thức thành công

**Kết quả tốt nhất** đến từ sự kết hợp giữa:

- **Sự khéo léo của con người** (human ingenuity)
    
- **Khả năng của công cụ Gen AI** (gen AI tool's capabilities)
    

## Lời khuyên cuối cùng

**Tiếp tục:**

- **Đặt câu hỏi sâu sắc** (asking insightful questions)
    
- **Tinh chỉnh prompts** (refining prompts)
    
- **Sử dụng kỹ năng tư duy phản biện** (critical-thinking skills)
    

**Mục tiêu:** Đóng góp vào một tương lai nơi **AI phục vụ mọi người một cách có trách nhiệm và đạo đức**.