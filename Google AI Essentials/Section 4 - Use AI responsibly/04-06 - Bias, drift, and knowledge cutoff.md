## Thiên lệch, drift và giới hạn kiến thức trong AI

### Tổng quan

Hiểu biết sâu sắc về các khái niệm trong AI có trách nhiệm như **thiên lệch** (bias), **drift** và **giới hạn kiến thức** (knowledge cutoff) có thể giúp bạn sử dụng AI một cách có đạo đức hơn và có trách nhiệm giải trình cao hơn.

### Tác hại và thiên lệch (Harms and Biases)

**Thiên lệch dữ liệu** (Data biases) là hoàn cảnh mà lỗi hệ thống hoặc định kiến dẫn đến thông tin không công bằng hoặc không chính xác, dẫn đến đầu ra thiên lệch.

#### 1. Tác hại phân bổ (Allocative Harm)

**Định nghĩa:** Hành vi sai trái xảy ra khi việc sử dụng hoặc hành vi của hệ thống AI từ chối cơ hội, tài nguyên hoặc thông tin trong các lĩnh vực ảnh hưởng đến phúc lợi của một người.

**Ví dụ:**

- Quản lý bất động sản sử dụng AI tool để kiểm tra lý lịch và sàng lọc đơn xin thuê
- AI tool nhận dạng sai ứng viên và đánh giá họ là rủi ro vì điểm tín dụng thấp
- Ứng viên bị từ chối thuê nhà và mất phí đăng ký

**Cách giảm thiểu:**

- **Đánh giá tất cả nội dung do AI tạo ra** trước khi tích hợp vào công việc hoặc chia sẻ
- **Kiểm tra kép** đầu ra AI với các nguồn khác


#### 2. Tác hại chất lượng dịch vụ (Quality-of-Service Harm)

**Định nghĩa:** Hoàn cảnh mà các công cụ AI không hoạt động tốt cho một số nhóm người nhất định dựa trên danh tính của họ.

**Ví dụ:**

- Khi công nghệ nhận dạng giọng nói lần đầu được phát triển
- Dữ liệu huấn luyện không có nhiều mẫu giọng nói của người khuyết tật
- Thiết bị thường gặp khó khăn trong việc phân tích loại giọng nói này

**Cách giảm thiểu:**

- **Chỉ định tính đa dạng** bằng cách thêm ngôn ngữ bao gồm vào prompt
- Nếu AI tool không xem xét một số nhóm hoặc danh tính nhất định, hãy giải quyết vấn đề đó khi lặp lại prompt


#### 3. Tác hại đại diện (Representational Harm)

**Định nghĩa:** Việc AI tool củng cố sự phụ thuộc của các nhóm xã hội dựa trên danh tính của họ.

**Ví dụ:**

- Công nghệ dịch thuật ban đầu tạo ra đầu ra thiên lệch nam/nữ không chính xác
- Khi dịch từ "y tá" (nurse) và "xinh đẹp" (beautiful) → thiên về nữ tính
- Khi dịch từ "bác sĩ" (doctor) và "mạnh mẽ" (strong) → thiên về nam tính

**Cách giảm thiểu:**

- **Thách thức các giả định** (Challenge assumptions)
- Nếu AI tool đưa ra phản hồi thiên lệch, hãy xác định và giải quyết vấn đề khi lặp lại prompt
- Yêu cầu công cụ sửa thiên lệch


#### 4. Tác hại hệ thống xã hội (Social System Harm)

**Định nghĩa:** Các tác động cấp vĩ mô của xã hội làm khuếch đại sự khác biệt về giai cấp, quyền lực hoặc đặc quyền hiện có, hoặc gây tổn hại vật lý do phát triển hoặc sử dụng AI tools.

**Ví dụ:**

- **Deepfakes không mong muốn** - ảnh hoặc video giả do AI tạo ra về người thật nói hoặc làm những việc họ không hề nói hoặc làm

**Cách giảm thiểu:**

- **Kiểm tra sự thật và tham chiếu chéo** đầu ra
- Sử dụng các tính năng cung cấp nguồn thông tin (nếu có)
- Kiểm tra sự thật bằng công cụ tìm kiếm để xác nhận thông tin
- Hỏi chuyên gia để được trợ giúp
- **Chạy prompt qua hai hoặc nhiều nguồn** để xác định đầu ra có thể không chính xác


#### 5. Tác hại giữa các cá nhân (Interpersonal Harm)

**Định nghĩa:** Việc sử dụng công nghệ để tạo bất lợi cho một số người nhất định, ảnh hưởng tiêu cực đến mối quan hệ của họ với người khác hoặc gây mất ý thức về bản thân và quyền tự chủ.

**Ví dụ:**

- Ai đó kiểm soát thiết bị thông minh tại căn hộ cũ để chơi khăm người bạn cùng phòng cũ
- Hành động này có thể dẫn đến mất ý thức về bản thân và quyền tự chủ

**Cách giảm thiểu:**

- **Xem xét tác động của việc sử dụng AI**
- Luôn sử dụng **phán đoán tốt nhất và kỹ năng tư duy phản biện**
- Tự hỏi liệu AI có phù hợp với nhiệm vụ bạn đang làm không
- **Trách nhiệm của người dùng** đảm bảo không gây tổn hại khi sử dụng AI


### Drift và giới hạn kiến thức (Drift vs Knowledge Cutoff)

#### Khái niệm Drift

**Drift** là sự suy giảm độ chính xác của mô hình AI trong dự đoán do những thay đổi theo thời gian không được phản ánh trong dữ liệu huấn luyện.

#### Khái niệm Knowledge Cutoff

**Giới hạn kiến thức** (Knowledge cutoff) là khái niệm rằng một mô hình được huấn luyện tại một thời điểm cụ thể, vì vậy nó không có kiến thức về các sự kiện hoặc thông tin sau ngày đó.

#### Ví dụ thực tế

**Nhà thiết kế thời trang muốn theo dõi xu hướng chi tiêu:**

- Sử dụng mô hình được huấn luyện lần cuối về xu hướng thời trang và thói quen tiêu dùng từ năm 2015
- Mô hình có thể không tạo ra đầu ra hữu ích vì hai yếu tố này có thể đã thay đổi theo thời gian
- Sở thích tiêu dùng năm 2015 rất có thể khác với xu hướng ngày nay
- **Kết quả:** Dự đoán của mô hình đã drift từ chính xác tại thời điểm huấn luyện thành ít chính xác ở hiện tại


### Các yếu tố gây ra Drift

- **Thiên lệch trong dữ liệu mới** (Biases in new data)
- **Thay đổi trong cách con người hành xử và sử dụng công nghệ**
- **Các sự kiện lớn trên thế giới** có thể ảnh hưởng đến mô hình


### Giải pháp duy trì hiệu quả AI

**Để giữ mô hình AI hoạt động tốt:**

- **Giám sát thường xuyên** hiệu suất của nó
- **Giải quyết giới hạn kiến thức** bằng cách tiếp cận **human-in-the-loop** (có con người tham gia vào vòng lặp)


### Tài nguyên tham khảo

**Google PAIR Explorables:**

- **What Have Language Models Learned?** - Tương tác với BERT (một trong những LLM đầu tiên)
- Khám phá cách các mối tương quan trong dữ liệu có thể dẫn đến thiên lệch có vấn đề trong kết quả
- Các **PAIR AI Explorables** khác để tìm hiểu thêm về AI có trách nhiệm

**Liên kết:** [[Responsible AI]], [[Data Bias]], [[Allocative Harm]], [[Quality-of-Service Harm]], [[Representational Harm]], [[Social System Harm]], [[Interpersonal Harm]], [[Drift]], [[Knowledge Cutoff]], [[BERT]], [[LLM]], [[Human-in-the-loop]], [[Deepfakes]], [[Google PAIR]], [[Critical Thinking]], [[Fact-checking]]

