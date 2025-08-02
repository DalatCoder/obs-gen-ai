## AI Models và Quy trình Huấn luyện (Training Process)

### Phân biệt AI Tools và AI Models

Các thuật ngữ [[AI Tools]] và [[AI Models]] có thể gây nhầm lẫn vì chúng nghe tương tự nhưng lại chỉ những thứ khác nhau:

- **[[AI Tool]]**: Phần mềm được hỗ trợ bởi AI có thể tự động hóa hoặc hỗ trợ người dùng thực hiện nhiều tác vụ khác nhau
- **[[AI Model]]**: Chương trình máy tính được huấn luyện trên các tập dữ liệu để nhận dạng patterns và thực hiện các tác vụ cụ thể


### Ẩn dụ Xe hơi và Động cơ

**Mối quan hệ giữa AI Tool và AI Model:**

#### AI Tool = Chiếc xe

- Giao diện thân thiện với người dùng (vô lăng, bảng điều khiển)
- Giúp bạn đến đích (hoàn thành tác vụ hoặc đạt được output mong muốn)
- Được thiết kế với các tính năng cụ thể cho từng mục đích sử dụng


#### AI Model = Động cơ

- Nằm "bên trong nắp capô" - không thể nhìn thấy trực tiếp
- Xử lý thông tin bạn cung cấp (như input vào phần mềm chỉnh sửa ảnh)
- Cho phép AI tool hoạt động


#### Đa dạng ứng dụng:

- **Sedan**: Cho việc lái xe hàng ngày
- **Pickup truck**: Cho việc chở hàng nặng
- **AI Tools**: Được phát triển cho nhiều ứng dụng khác nhau (tạo văn bản, hình ảnh, video, viết code)


### Multimodal Tools

**Ghi chú quan trọng:** Một số [[AI Tools]] sử dụng nhiều [[AI Models]] làm việc cùng nhau như một "gia đình" (family) để:

- Đạt được tính linh hoạt cao hơn
- Thực hiện phạm vi tác vụ rộng hơn
- Mỗi model trong gia đình chuyên biệt cho một subtask cụ thể
- Đóng góp vào chức năng tổng thể của AI tool


### Quy trình Huấn luyện AI Models

[[Training Process]] là quy trình lặp đi lặp lại (iterative process) mà các AI designers và engineers sử dụng để phát triển [[AI Models]].

#### Ví dụ thực tế: Xây dựng Model Dự báo Mưa

**Bước 1: Định nghĩa vấn đề cần giải quyết**

- Mục tiêu: Dự báo mưa để giúp mọi người khô ráo khi đi làm
- Xem xét khả năng và hạn chế của AI trước khi xác định giải pháp AI

**Bước 2: Thu thập dữ liệu liên quan để huấn luyện model**

- Thu thập dữ liệu lịch sử về những ngày có mưa và không mưa trong 50 năm qua
- Dữ liệu phải đủ đa dạng và phong phú

**Bước 3: Chuẩn bị dữ liệu cho quá trình huấn luyện**

- **Gán nhãn (labeling)** các đặc trưng quan trọng:
    - Nhiệt độ ngoài trời (outdoor temperature)
    - Độ ẩm (humidity)
    - Áp suất không khí (air pressure)
- Ghi chú có mưa hay không
- Chia dữ liệu thành hai tập riêng biệt:
    - **Training set**: Để huấn luyện
    - **Validation set**: Để kiểm tra sau này

**Bước 4: Huấn luyện model**

- Áp dụng các chương trình [[Machine Learning]] (ML) vào training data đã chuẩn bị
- ML programs phân tích dữ liệu và học cách nhận dạng patterns
- **Patterns ví dụ**: Kết hợp nhiệt độ cao + áp suất thấp + độ ẩm cao = khả năng mưa cao

**Bước 5: Đánh giá model**

- Sử dụng validation set để đánh giá khả năng dự báo mưa chính xác và đáng tin cậy
- Phân tích hiệu suất có thể phát hiện các vấn đề tiềm ẩn:
    - Dữ liệu huấn luyện không đủ (insufficient training data)
    - Dữ liệu huấn luyện thiên lệch (biased training data)
- Nếu có vấn đề: quay lại bước trước đó để thử cách tiếp cận khác
- Khi model hoạt động tốt với validation set: tiếp tục bước tiếp theo

**Bước 6: Triển khai model**

- Khi AI designers và engineers hài lòng với hiệu suất model
- Triển khai model trong một AI tool
- Kết quả: Giúp người dân trong thành phố tránh ướt trên đường đi làm!


### Tính chất Lặp đi Lặp lại (Iterative Nature)

#### Đặc điểm chính:

- AI designers và engineers có thể lặp lại mỗi bước nhiều lần cần thiết
- Thực hiện điều chỉnh cho đến khi tạo ra model tốt nhất có thể
- Quá trình không dừng lại ở việc triển khai


#### Giám sát Liên tục (Continuous Monitoring):

- Sau khi users tương tác với model trong tình huống thực tế
- Model có thể gặp phải những thách thức mới
- **Yêu cầu:**
    - Giám sát liên tục
    - Thu thập phản hồi về models
    - Đảm bảo models tiếp tục hoạt động đáng tin cậy
    - Xác định các khu vực cần cải thiện


### Tầm quan trọng của Hiểu biết về AI Models

#### Lợi ích khi hiểu cách phát triển AI Models:

- Đưa ra **quyết định có căn cứ** về khi nào và cách nào sử dụng AI tool
- Thảo luận về AI tools một cách chính xác và tự tin hơn
- Hiểu được quá trình tinh chỉnh liên tục (continual refinement) tạo nên:
    - AI models chính xác (precise)
    - AI models đa năng (versatile)
    - AI tools hiệu quả và đáng tin cậy


### Ghi chú thêm

Quy trình [[Training Process]] này thể hiện sự phức tạp và tính khoa học trong việc phát triển [[AI Models]]. Hiểu được quy trình này giúp người dùng đánh giá được chất lượng và độ tin cậy của các [[AI Tools]] mà họ sử dụng trong công việc hàng ngày.

**Liên kết:** [[AI Tools]], [[AI Models]], [[Training Process]], [[Machine Learning]], [[Iterative Process]], [[Validation Set]], [[Training Set]], [[Patterns]], [[Multimodal Tools]]

