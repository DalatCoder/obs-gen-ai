# Sử dụng trí tuệ nhân tạo tạo sinh một cách có trách nhiệm

## Tổng quan

Các công cụ **trí tuệ nhân tạo tạo sinh (Gen AI)** rất mạnh mẽ, nhưng giống như bất kỳ công cụ nào, điều quan trọng là phải sử dụng chúng một cách có trách nhiệm, đặc biệt là trong môi trường làm việc.

## Ba nguyên tắc cơ bản của việc sử dụng có trách nhiệm

## 1. Xem xét vấn đề và sự phù hợp

**Trước khi sử dụng Gen AI, hãy tự hỏi:**

- Vấn đề bạn đang sử dụng Gen AI để giải quyết có **phù hợp với mục tiêu** của bạn không?
    
- Có **phù hợp với nghĩa vụ** đối với khách hàng và đồng nghiệp không?
    
- **Chính sách của tổ chức** và **luật pháp địa phương** có cho phép sử dụng Gen AI cho loại tác vụ này không?
    

**Nếu không phù hợp:** Cần suy nghĩ lại quy trình và xem Gen AI có phù hợp với công việc hay không.

## 2. Tuân thủ chính sách và bảo mật dữ liệu

## Đối với môi trường công việc

- **Tham khảo quy tắc hoặc chính sách** của công ty trước khi nhập dữ liệu bí mật hoặc nhạy cảm vào các công cụ Gen AI
    
- **Kiểm tra** xem công ty có phiên bản doanh nghiệp (enterprise version) của công cụ Gen AI được phép sử dụng cho các mục đích khác hay không
    

## Đối với việc sử dụng cá nhân

- **Tránh nhập thông tin cá nhân hoặc bí mật** về bản thân vào các công cụ có sẵn công khai
    
- **Luôn kiểm tra** cách dữ liệu bạn nhập có thể được sử dụng
    

## 3. Đánh giá kết quả đầu ra và tiết lộ việc sử dụng

**Trách nhiệm của người dùng Gen AI có trách nhiệm:**

- **Đánh giá kết quả đầu ra** về khả năng thiên vị (bias) và lỗi
    
- **Tiết lộ việc sử dụng Gen AI** khi chia sẻ nội dung với người khác
    
- **Đánh giá độ chính xác** của kết quả đầu ra như bạn làm với bất kỳ kết quả nào
    

## Hiện tượng Hallucinations (Ảo giác AI)

## Định nghĩa và đặc điểm

**Hallucinations (Ảo giác AI)** là khi công cụ Gen AI cung cấp kết quả đầu ra:

- **Không nhất quán** (inconsistent)
    
- **Không chính xác** (incorrect)
    
- **Vô nghĩa** (nonsensical)
    

## Nguyên nhân chính

**Ảo giác AI thường xảy ra khi:**

1. **Hướng dẫn mơ hồ hoặc không rõ ràng**: Người dùng đưa ra prompt thiếu cụ thể
    
2. **Đoán mò câu trả lời**: Công cụ cố gắng trả lời điều mà nó không thực sự hiểu
    

## Tính khó nhận biết

- **Ảo giác AI có thể khó nhận ra**
    
- Vì vậy, việc **kiểm tra sự thật và tham chiếu chéo** (fact check và cross-reference) kết quả đầu ra là rất quan trọng
    
- Cần xác nhận xem một sự thật hoặc tuyên bố trong kết quả đầu ra có đúng hay không
    

## Phương pháp "Human in the Loop" (Con người trong vòng lặp)

## Nguyên tắc cơ bản

- **Các công cụ Gen AI không tư duy phản biện** như con người có thể
    
- Quan trọng là duy trì cách tiếp cận **"human in the loop"**
    
- **Ý nghĩa**: Con người cần xác minh kết quả đầu ra của Gen AI trước khi sử dụng
    

## Ví dụ thực tế: Tạo hình ảnh mèo trên tên lửa

**Tình huống:**

- Muốn tạo hình ảnh **những chú mèo trên tên lửa bay lên mặt trăng** cho bài thuyết trình
    
- **Kết quả ban đầu**: Mèo ở **trên đỉnh tên lửa** thay vì bên trong
    
- **Vấn đề**: Điều này không an toàn cho mèo
    

**Giải pháp:**

- Mặc dù đã viết trong prompt rằng "mèo cần ở trên tên lửa", nhưng công cụ hiểu theo nghĩa đen
    
- **Lặp lại (iterate)** và chỉ định cụ thể: mèo nên xuất hiện **an toàn bên trong tên lửa** thay vì trên đỉnh
    

## Công cụ kiểm tra sự thật tích hợp

## Tính năng của Gemini

- Một số công cụ Gen AI như **Gemini có bộ kiểm tra sự thật tích hợp** (built-in fact checker)
    
- Cho phép **tham chiếu chéo kết quả đầu ra** bằng cách sử dụng Google Search
    
- **So sánh kết quả đầu ra** cạnh nhau giúp dễ dàng xác định độ chính xác của kết quả ban đầu
    
- Tìm ra bất kỳ **sự khác biệt** nào
    

## Tránh thiên vị (Bias) trong Gen AI

## Nhận biết và hậu quả

**Cần cố gắng nhận biết thiên vị trong kết quả đầu ra:**

- Thiên vị có thể xuất hiện dưới dạng **định kiến** (stereotypes)
    
- **Đại diện không công bằng** của một nhóm người
    
- **Hậu quả tiêu cực** mà chúng có thể gây ra
    

## Phương pháp tránh thiên vị

## 1. Cải thiện prompt

- **Tránh thiên vị** bắt đầu từ việc nhập **prompt cụ thể, chi tiết**
    
- **Lặp lại khi cần thiết** (iterating as needed)
    

## 2. Sử dụng ngôn ngữ bao trùm

**Sử dụng ngôn ngữ bao gồm:**

- Người từ **mọi nền tảng** (all backgrounds)
    
- **Mọi giới tính** (genders)
    
- **Mọi dân tộc** (ethnicities)
    

**Tránh:**

- **Định kiến** (stereotypes)
    
- **Khái quát hóa** (generalizations) trong input
    

## 3. Ví dụ thực tế: Viết mô tả tuyển dụng

**Tránh các thuật ngữ có tính giới:**

- không nên dùng **"serviceman"** hoặc **"workman"**
    
- nên dùng **"service person"** hoặc **"worker"**
    

**Lý do:**

- Để công cụ không viết mô tả chỉ hướng đến người tự nhận là nam giới
    

## Kết luận quan trọng

## Bản chất của các công cụ Gen AI

- **Các công cụ Gen AI chỉ là công cụ**
    
- Chúng **không tư duy phản biện** và **không thể hiểu được sắc thái** như con người
    
- **Nhiệm vụ của bạn** là mang góc nhìn con người vào mỗi lần sử dụng công cụ Gen AI
    

## Trách nhiệm của người dùng

Sử dụng Gen AI có trách nhiệm đòi hỏi:

1. **Xem xét sự phù hợp** với mục tiêu và nghĩa vụ
    
2. **Tuân thủ chính sách** và bảo vệ dữ liệu nhạy cảm
    
3. **Đánh giá kết quả đầu ra** về độ chính xác và thiên vị
    
4. **Duy trì cách tiếp cận "human in the loop"**
    
5. **Tiết lộ việc sử dụng Gen AI** một cách minh bạch