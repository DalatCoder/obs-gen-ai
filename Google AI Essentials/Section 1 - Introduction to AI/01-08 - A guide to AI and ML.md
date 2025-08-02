## Hướng dẫn về AI và Machine Learning

### Giới thiệu về AI và ML

**Trí tuệ nhân tạo (Artificial Intelligence - AI)** và **học máy (Machine Learning - ML)** đang thay đổi tương lai của công việc. Mặc dù cả hai thuật ngữ có vẻ tương tự nhau, **machine learning thực chất là một kỹ thuật cụ thể** được các nhà thiết kế AI sử dụng để đạt được các chương trình máy tính thông minh nhân tạo.

**Tầm quan trọng:**

- Hiểu cơ bản về mối quan hệ giữa AI và ML giúp bạn điều hướng các công nghệ này
- Cho phép đóng góp hiệu quả vào các dự án được thôi thúc bởi AI
- Hỗ trợ lãnh đạo các sáng kiến AI của riêng bạn


### Kỹ thuật phát triển AI

**AI** đề cập đến **các chương trình máy tính có thể hoàn thành các nhiệm vụ nhận thức thường được liên kết với trí tuệ con người**.

#### Hai kỹ thuật chính để thiết kế chương trình AI:

**1. Kỹ thuật dựa trên quy tắc (Rule-based techniques):**

- Tạo ra các chương trình AI **tuân theo nghiêm ngặt các quy tắc được định sẵn** để đưa ra quyết định
- **Ví dụ:** Bộ lọc spam sử dụng kỹ thuật dựa trên quy tắc có thể chặn email chứa từ khóa cụ thể bằng logic được định sẵn

**2. Kỹ thuật học máy (Machine Learning techniques):**

- Tạo ra các chương trình AI có thể **phân tích và học từ các mẫu trong dữ liệu** để đưa ra quyết định độc lập
- **Ví dụ:** Bộ lọc spam sử dụng kỹ thuật này có thể đánh dấu spam tiềm ẩn để người nhận xem xét, tránh việc chặn tự động
- Nếu người nhận đánh dấu email từ nguồn tin cậy là an toàn, bộ lọc spam sẽ **học và thích ứng logic** để bao gồm các email tương tự từ người gửi đó trong tương lai


#### So sánh ứng dụng:

**Kỹ thuật dựa trên quy tắc:**

- Phù hợp cho các tác vụ **yêu cầu tính cứng nhắc**
- Ví dụ: chặn tin nhắn từ người gửi không đáng tin cậy (như yêu cầu chuyển tiền ngân hàng hoặc thông tin riêng tư)

**Kỹ thuật ML:**

- Phù hợp cho các tác vụ **đòi hỏi tính linh hoạt và khả năng thích ứng**
- Ví dụ: học nhận biết rằng tin nhắn từ người gửi đáng tin cậy có lỗi chính tả không phải là spam


### Các phương pháp huấn luyện chương trình ML

**Machine Learning** là tập con của AI tập trung vào việc phát triển các chương trình máy tính có thể phân tích dữ liệu để đưa ra quyết định hoặc dự đoán.

#### Ba phương pháp phổ biến:

**1. Học có giám sát (Supervised Learning):**

- Nhà thiết kế AI cung cấp cho chương trình ML **bộ dữ liệu huấn luyện có nhãn** (labeled training set)
- **Bộ dữ liệu có nhãn** bao gồm dữ liệu được gắn nhãn hoặc thẻ, cung cấp ngữ cảnh và ý nghĩa cho dữ liệu
- **Ví dụ:** Bộ lọc email spam được huấn luyện với supervised learning sẽ sử dụng bộ dữ liệu email được gắn nhãn "spam" hoặc "không spam"
- **Ứng dụng:** Thường được sử dụng khi có kết quả đầu ra cụ thể trong tâm trí

**2. Học không giám sát (Unsupervised Learning):**

- Nhà thiết kế AI cung cấp cho chương trình ML **bộ dữ liệu huấn luyện không có nhãn** (unlabeled training set)
- **Bộ dữ liệu không nhãn** bao gồm dữ liệu không có nhãn hoặc thẻ
- **Ví dụ:** ML có thể được sử dụng để phân tích bộ dữ liệu tin nhắn email chưa được phân loại và tìm ra các mẫu trong chủ đề, từ khóa hoặc liên hệ
- **Ứng dụng:** Sử dụng để **nhận diện các mẫu trong dữ liệu** mà không có kết quả đầu ra cụ thể trong tâm trí

**3. Học tăng cường (Reinforcement Learning):**

- Nhà thiết kế AI cung cấp cho chương trình ML dữ liệu cho phép nó **học qua thử và sai** (trial-and-error)
- Chương trình học bằng cách **nhận phần thưởng** khi đưa ra lựa chọn tốt dẫn đến kết quả mong muốn
- **Ứng dụng:** Thường được sử dụng bởi các công cụ AI hội thoại
- Khi các công cụ này nhận phản hồi từ người dùng và nhà thiết kế AI, chúng học cách tạo ra phản hồi hiệu quả


### AI Tạo sinh (Generative AI)

**Định nghĩa:** AI có thể **tạo ra nội dung mới** như văn bản, hình ảnh hoặc phương tiện truyền thông khác.

#### Cách hoạt động:

- Khi người dùng cung cấp đầu vào dưới dạng **prompt** (văn bản đầu vào cung cấp hướng dẫn cho mô hình AI về cách tạo kết quả đầu ra)
- Công cụ AI xử lý đầu vào này để **tạo ra nội dung mới**


#### Vai trò của ba phương pháp ML trong AI hội thoại:

**Supervised Learning:**

- Trang bị cho công cụ AI hội thoại **dữ liệu đối thoại cơ bản**
- Cho phép chúng phản hồi phù hợp với các tín hiệu hội thoại thông thường

**Unsupervised Learning:**

- Cho phép chúng **diễn giải các sắc thái trong ngôn ngữ** như cách nói thông tục xảy ra tự nhiên trong cuộc trò chuyện

**Reinforcement Learning:**

- **Tăng cường các công cụ này** bằng cách cho phép chúng cải thiện phản hồi theo thời gian thực dựa trên phản hồi của người dùng
- Cho phép chúng thích ứng với bối cảnh hội thoại và tham gia vào cuộc trò chuyện tự nhiên


### Lợi ích của AI Tạo sinh

**Khả năng tạo ra và đổi mới** của AI tạo sinh mang lại nhiều lợi ích cho tất cả các loại nơi làm việc và nghề nghiệp:

#### Các ngành được hỗ trợ:

- Marketing
- Phát triển sản phẩm
- Kỹ thuật
- Giáo dục
- Sản xuất
- Nghiên cứu và phát triển


#### Lợi ích cụ thể:

**1. Hiệu quả cao hơn (Greater efficiency):**

- AI tạo sinh có thể **tự động hóa hoặc tăng cường các tác vụ thường ngày**
- Cho phép nhân viên tập trung vào các ưu tiên công việc khác

**2. Trải nghiệm cá nhân hóa (Personalized experiences):**

- AI tạo sinh có thể **điều chỉnh tương tác** theo sở thích và nhu cầu cá nhân

**3. Quyết định tốt hơn (Better decisions):**

- AI tạo sinh có thể **nhanh chóng phân tích lượng lớn dữ liệu** để khám phá những thông tin hữu ích


### Tài nguyên bổ sung

**PAIR Explorables:**

- Tài nguyên tùy chọn cho những ai muốn tìm hiểu thêm về AI
- Là tập hợp các bài viết tương tác được thiết kế để **làm cho các khái niệm AI chính trở nên dễ tiếp cận và hiểu hơn**

**Các chủ đề được đề cập:**

- Cơ bản về machine learning
- Công bằng và thiên vị trong các chương trình AI
- Cân nhắc về dữ liệu và quyền riêng tư trong AI
- Rủi ro và lợi ích tiềm ẩn của AI

**Đặc điểm:**

- Mỗi bài viết có **hình ảnh trực quan và điều khiển tương tác**
- Giúp bạn khám phá các khái niệm AI khác nhau và trải nghiệm cách chúng hoạt động


### Ghi chú thêm

Bài đọc này cung cấp cái nhìn tổng quan toàn diện về mối quan hệ giữa AI và ML, từ các kỹ thuật cơ bản đến ứng dụng tiên tiến như AI tạo sinh. Hiểu rõ những khái niệm này là nền tảng quan trọng để tham gia hiệu quả vào thế giới công nghệ AI đang phát triển nhanh chóng.

**Liên kết:** [[Artificial Intelligence]], [[Machine Learning]], [[Supervised Learning]], [[Unsupervised Learning]], [[Reinforcement Learning]], [[Generative AI]], [[Rule-based Techniques]], [[Training Set]], [[Prompt]], [[PAIR Explorables]]

