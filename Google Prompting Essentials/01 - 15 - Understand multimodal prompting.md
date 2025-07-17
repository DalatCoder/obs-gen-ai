# Hiểu về Prompting đa phương thức (Multimodal Prompting)

## Khái niệm cơ bản

## Ví dụ minh họa

Giống như một **nghệ sĩ có thể tạo ra kiệt tác chỉ với một màu sơn**, nhưng sử dụng nhiều màu sắc sẽ mang lại **sức mạnh lớn hơn** để tạo ra điều gì đó tuyệt vời. Điều tương tự cũng áp dụng cho prompt:

- **Prompt chỉ có văn bản** đã có thể làm được nhiều việc
    
- **Thêm các yếu tố khác** sẽ đưa prompt lên tầm cao mới
    
- **Prompting đa phương thức** mở ra **thế giới khả năng mới**
    

## Định nghĩa Multimodal Prompting

**Prompting đa phương thức (Multimodal Prompting)** là thuật ngữ lớn với ý nghĩa đơn giản:

- **Modalities (Phương thức)**: Các loại định dạng khác nhau như văn bản, hình ảnh, hoặc âm thanh có thể được sử dụng để hướng dẫn công cụ trí tuệ nhân tạo tạo sinh (Gen AI)
    
- **Multimodal Prompting**: Sử dụng **nhiều phương thức** trong cùng một prompt
    

## Tính hữu ích

Prompting đa phương thức cho phép thực hiện những tác vụ như:

- **Chuyển đổi hình ảnh** thành mô tả văn bản chi tiết cho người khiếm thị
    
- **Tạo đồ họa** dựa trên bản ghi âm mô tả chiến dịch marketing
    

## Lợi ích và cân nhắc

## Phản ánh thế giới thực

**Thế giới là đa phương thức (multimodal):**

- Khi thuyết trình tại công ty, bạn sử dụng văn bản, hình ảnh và giọng nói để giúp khán giả hiểu quan điểm
    
- **Prompting đa phương thức hoạt động tương tự**
    

**Cách thức hoạt động:**

- Phản ánh cách bạn trải nghiệm thế giới
    
- **Xây dựng kết nối** giữa văn bản, hình ảnh, âm thanh và các phương thức khác
    
- Giúp cung cấp **hướng dẫn rõ ràng hơn** cho công cụ Gen AI
    

## Cải thiện chất lượng prompt

**Không phải giải pháp phù hợp cho mọi trường hợp**, nhưng có thể cải thiện prompt:

**Ví dụ cụ thể:**

- Yêu cầu Gen AI viết thơ về hoàng hôn + kèm theo ảnh hoàng hôn
    
- Gen AI có thể sử dụng ảnh để mô tả màu sắc và chi tiết cụ thể
    
- **Kết quả**: Bài thơ **sinh động hơn nhiều**
    

## Hạn chế cần lưu ý

**Các công cụ Gen AI đôi khi gặp khó khăn với:**

- **Ý tưởng trừu tượng**
    
- **Xử lý kết hợp phức tạp** của các phương thức
    
- **Thông thức thường** (common sense)
    

**Ví dụ hạn chế:**

- Mặc dù luôn phát triển và cải thiện, prompting đa phương thức **chưa đáng tin cậy** cho việc đếm số lượng
    

## Ví dụ thực tế về Multimodal Prompting

## Nguyên tắc chung

Prompting đa phương thức **hiệu quả nhất** trong các tình huống cần **chuyển đổi thông tin từ phương tiện này sang phương tiện khác**.

## Các ví dụ cụ thể

**1. Gợi ý công thức nấu ăn**

- Yêu cầu Gen AI đề xuất công thức dựa trên ảnh nguyên liệu trong tủ lạnh
    

**2. Tạo teaser kỹ thuật số**

- Cần tạo teaser quảng bá sự kiện giữa hai thương hiệu trên mạng xã hội
    
- Input: Logo và màu sắc của cả hai thương hiệu
    
- Yêu cầu: Tạo visual cho sự kiện chung
    

**3. Viết truyện ngắn về rừng**

- Đang viết truyện ngắn về khu rừng vừa thăm
    
- Cần trợ giúp mô tả âm thanh và bầu không khí
    
- Input: File âm thanh ghi âm khi thăm rừng
    
- Yêu cầu: Sử dụng âm thanh để tạo cảm hứng cho bầu không khí và chi tiết câu chuyện
    

## Áp dụng Prompting Framework cho Multimodal

## Nguyên tắc cơ bản

Vẫn dựa trên framework **Thoughtfully Create Really Excellent Inputs (TCREI)**, nhưng có thể cần **điều chỉnh** dựa trên các phương thức đang sử dụng.

## Chi tiết từng thành phần

## **Task (Nhiệm vụ)**

- **Cụ thể về persona và format** như thường lệ
    
- **Cụ thể về cách sử dụng** các phương thức khác nhau
    
- **Giải thích lý do** đưa chúng vào nhiệm vụ
    

## **Context (Bối cảnh)**

- Thêm bối cảnh để Gen AI biết chính xác những gì cần làm
    
- **Cân nhắc các phương thức** đang sử dụng trong prompt
    
- **Ràng buộc hoặc cân nhắc cụ thể** cần bao gồm
    

**Ví dụ:**

- Input ảnh bên trong tủ lạnh
    
- Chỉ muốn Gen AI xem xét trái cây và rau trong ảnh
    
- Không xem xét các hàng đóng gói
    

## **References (Tài liệu tham khảo)**

- Chia sẻ tài liệu tham khảo **bằng văn bản, hình ảnh, hoặc âm thanh**
    
- Giúp Gen AI hiểu loại output đang cố gắng tạo ra
    
- **Lưu ý**: Không phải công cụ nào cũng hỗ trợ mọi loại tài liệu tham khảo
    

## **Evaluate (Đánh giá)**

- Chạy prompt như thường lệ
    
- **Chú ý đặc biệt** đến cách output trông như thế nào hoặc đọc như thế nào
    
- Do sử dụng các phương thức khác nhau, có thể cần **đánh giá chi tiết hơn** so với việc chỉ đánh giá phản hồi văn bản
    

## **Iterate (Lặp lại)**

Nếu output không đáp ứng nhu cầu, thử một trong **4 phương pháp lặp lại**:

1. **Xem lại prompting framework**
    
2. **Chia nhỏ prompt** thành các tác vụ ngắn hơn
    
3. **Giới thiệu ràng buộc**
    
4. **Điều chỉnh cách diễn đạt** hoặc chuyển sang tác vụ tương tự để kích hoạt phản hồi khác (có thể tốt hơn)
    

## Kết luận

**Prompting đa phương thức** là công cụ mạnh mẽ cho phép:

- **Chuyển đổi thông tin** sang các phương tiện khác nhau
    
- Tạo ra **khả năng vô tận** của các output
    

**Bạn là nghệ sĩ**, và **công cụ Gen AI là cọ vẽ** của bạn.