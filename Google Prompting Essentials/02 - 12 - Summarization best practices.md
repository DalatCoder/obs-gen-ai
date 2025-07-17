# Thực hành Tốt nhất cho Tóm tắt với Trí tuệ nhân tạo tạo sinh (Gen AI)

## Tổng quan về Tóm tắt với Gen AI

Bạn đã bao giờ cần trích xuất thông tin từ một tài liệu khổng lồ chưa? Hoặc có thể gặp phải một chuỗi email cực kỳ dài mà bạn gặp khó khăn trong việc nắm bắt nội dung chính? Tin tốt: Các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) rất giỏi trong việc tóm tắt thông tin và tiết kiệm thời gian cho bạn.

## Cách thức hoạt động

Các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) sử dụng **nhận dạng mẫu** (pattern recognition) để phân tích các chuỗi văn bản và tinh chỉnh chúng thành các bản tóm tắt ngắn hơn. Để đảm bảo bản tóm tắt chứa đúng thông tin, đúng định dạng và độ sâu, hãy tạo một prompt mạnh mẽ với các chi tiết cụ thể về những gì bạn cần trong bản tóm tắt.

## Thực hành Tốt nhất cho Tóm tắt

## Điều chỉnh Khung Prompting Framework

Dưới đây là cách điều chỉnh các phần khác nhau của khung prompting khi hướng dẫn công cụ trí tuệ nhân tạo tạo sinh (Gen AI) tóm tắt thông tin:

## 1. Task (Nhiệm vụ)

**Nội dung cần bao gồm:**

- **Xác định nội dung** cần tóm tắt (một phần tài liệu hoặc chủ đề phụ cụ thể)
    
- **Định dạng mong muốn** (bullet points, đoạn văn, v.v.)
    
- **Độ dài** của bản tóm tắt
    
- **Giọng điệu** (tone) mong muốn
    
- **Persona** (ví dụ: phù hợp với trình độ đọc hiểu lớp 9)
    

## 2. Context (Ngữ cảnh)

**Thông tin bổ sung:**

- **Mục đích** của bản tóm tắt
    
- **Lý do** tạo ra nó
    
- Giúp công cụ trí tuệ nhân tạo tạo sinh (Gen AI) **neo phản hồi** vào điều gì đó cụ thể
    

## 3. References (Tài liệu tham khảo)

**Khi nào sử dụng:**

- Nếu có bản tóm tắt **khớp với yêu cầu**
    
- Cung cấp cả **bản tóm tắt** và **tài liệu gốc** làm tài liệu tham khảo
    
- Giúp công cụ biết **cách tiếp cận** cần thực hiện
    

## 4. Evaluate (Đánh giá)

**Tầm quan trọng:**

- Khi nhập **lượng lớn văn bản hoặc dữ liệu**, có nhiều thông tin để công cụ trí tuệ nhân tạo tạo sinh (Gen AI) xử lý
    
- Tăng khả năng **diễn giải sai**, **chuỗi suy nghĩ không liên quan** hoặc **hallucinations** (ảo giác)
    

**Phương pháp đánh giá:**

- Đánh giá dựa trên **nhiệm vụ** bạn đã nhập
    
- **Kiểm tra chéo** (cross-reference) kết quả
    
- Nhờ **chuyên gia chuyên môn** (subject matter expert) xem xét nếu có thể
    

## 5. Iterate (Lặp lại)

**Khi nào cần lặp lại:**

- Nếu công cụ trí tuệ nhân tạo tạo sinh (Gen AI) **không đưa ra bản tóm tắt hữu ích**
    
- Cần điều chỉnh **định dạng**, **độ dài** hoặc **chi tiết cụ thể**
    
- **Tiếp tục lặp lại** cho đến khi nhận được bản tóm tắt phục vụ mục đích
    

## Long Context 101 - Hiểu về Ngữ cảnh Dài

## Sự Cải tiến Liên tục

Các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) không ngừng cải tiến và một số hiện có khả năng xử lý các **đoạn văn bản và dữ liệu lớn hơn nhiều** trong một lần nhập. Điều này được thực hiện nhờ:

- Tăng **giới hạn token** (token limits) của các công cụ trí tuệ nhân tạo tạo sinh (Gen AI)
    
- Sử dụng **cửa sổ ngữ cảnh dài** (long context windows)
    

## AI Model và Token Limit

## Khái niệm Token

**Token** là các khối xây dựng cơ bản của văn bản mà các mô hình AI sử dụng để xử lý và hiểu ngôn ngữ. Token có thể là:

- **Một ký tự đơn**
    
- **Một phần của từ**
    
- **Nhiều từ**
    

**Ví dụ minh họa:** Nếu bạn đang xây một ngôi nhà bằng gạch, bạn có thể coi mỗi viên gạch như một token trong quá trình xây dựng.

## Quá trình Xử lý

1. Khi bạn đưa ra một prompt cho công cụ trí tuệ nhân tạo tạo sinh (Gen AI), nó **chia nhỏ thành tokens**
    
2. **Prompt càng dài** = **càng cần nhiều tokens** để tạo ra đầu ra
    
3. Điều quan trọng là hiểu **mô hình AI** bạn đang sử dụng và **giới hạn token** của nó
    

## Sự Phát triển của Token Limits

**Trước đây:** Các mô hình AI chỉ có thể xử lý **vài nghìn tokens** cùng lúc  
**Hiện tại:** Một số mô hình có thể xử lý **hàng triệu tokens**

**Tác động:** Khi các nhà phát triển tìm ra cách tăng giới hạn token, các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) ngày càng có khả năng xử lý **lượng dữ liệu lớn hơn** trong một prompt duy nhất.

## Long Context Windows - Cửa sổ Ngữ cảnh Dài

## Định nghĩa và Khả năng

**Long context windows** cho phép các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) xử lý **lượng lớn thông tin** hoặc **lượng lớn tokens** theo các định dạng khác nhau cùng một lúc.

## Lợi ích

**Chia sẻ nhiều ngữ cảnh hơn:**

- Có thể chia sẻ **nhiều ngữ cảnh và thông tin nền** hơn trong đầu vào
    
- Cho phép hoàn thành **các tác vụ phức tạp hơn** với nhiều chi tiết tinh tế
    

**Ví dụ ứng dụng:**

- Tạo **chiến dịch marketing đa phần** (multi-part marketing campaign)
    
- Xây dựng **kế hoạch kinh doanh toàn diện** (thorough business plan)
    

## Phản hồi Tốt hơn

Với **nhiều ngữ cảnh và thông tin chi tiết** về nhiệm vụ, công cụ trí tuệ nhân tạo tạo sinh (Gen AI) có thể:

- Hiểu và tạo ra **phản hồi toàn diện hơn**
    
- **Cá nhân hóa** kết quả
    
- Đưa ra **phản hồi liên quan hơn**
    

## Ví dụ Thực tế

**Tình huống:** Xử lý một báo cáo PDF dài với hàng chục trang, đồ thị và minh họa

**Khả năng với long context window:**

- Xử lý **toàn bộ tài liệu** trong một lần nhập
    
- Tạo ra **bản tóm tắt** dựa trên yêu cầu cụ thể
    
- **Tiết kiệm thời gian** bằng cách loại bỏ nhu cầu chia nhỏ văn bản thủ công
    

## Working Memory - Bộ nhớ Làm việc

## Vấn đề Ghi nhớ

**Ví dụ thường gặp:** Bạn có bao giờ quên một điều gì đó, như món ăn bạn đã gọi tuần trước hoặc tên của ai đó giữa cuộc trò chuyện?

**Thách thức tương tự với Gen AI:** Việc nhớ lại các chi tiết trong quá khứ có thể khó khăn đối với các công cụ trí tuệ nhân tạo tạo sinh (Gen AI).

## Giải pháp Long Context Windows

**Chức năng như bộ nhớ làm việc:**

- Hoạt động như **working memory** cho các công cụ trí tuệ nhân tạo tạo sinh (Gen AI)
    
- Giúp chúng **nhớ** những gì bạn đã chia sẻ trước đó trong cùng một chuỗi trò chuyện
    

**Ví dụ minh họa:** Giống như nói chuyện với ai đó **đã quen thuộc** với vấn đề bạn đang cố gắng giải quyết thay vì giải thích tình huống cho một **người lạ không có ngữ cảnh**.

## Lưu ý Quan trọng về Giới hạn

**Phạm vi ghi nhớ:** Hầu hết các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) chỉ **nhớ** những gì bạn đưa vào long context window trong:

- **Cùng một chuỗi trò chuyện** (conversation thread)
    
- **Chuỗi prompt** (prompt chain)
    

**Hạn chế:** Nếu bạn **đóng cửa sổ** và **mở lại** sau khi nhập tài liệu (ví dụ: kịch bản), công cụ sẽ **không nhớ** và bạn cần nhập lại tài liệu trước khi công cụ có thể cung cấp đầu ra liên quan.

## Kết luận

Tóm tắt với trí tuệ nhân tạo tạo sinh (Gen AI) là một kỹ năng quan trọng trong thời đại số. Bằng cách áp dụng các thực hành tốt nhất về prompting framework và hiểu rõ về long context windows, bạn có thể tối ưu hóa hiệu quả và chất lượng của các bản tóm tắt từ các công cụ AI, tiết kiệm thời gian và nâng cao năng suất làm việc.