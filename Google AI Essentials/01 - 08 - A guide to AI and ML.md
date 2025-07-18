## Hướng Dẫn Về Trí Tuệ Nhân Tạo (AI) Và Học Máy (ML)

## Giới Thiệu

Trí tuệ nhân tạo (AI) và học máy (ML) đang thay đổi tương lai công việc. Mặc dù hai thuật ngữ này có vẻ tương đồng, học máy (ML) thực chất là một kỹ thuật cụ thể mà các nhà thiết kế trí tuệ nhân tạo (AI designers) sử dụng để tạo ra các chương trình máy tính thông minh nhân tạo. Việc nắm vững cơ bản về mối quan hệ giữa trí tuệ nhân tạo (AI) và học máy (ML) giúp bạn điều hướng các công nghệ này khi chúng biến đổi môi trường làm việc, cho phép bạn đóng góp hiệu quả vào các dự án dựa trên trí tuệ nhân tạo (AI) hoặc dẫn dắt sáng kiến riêng.

Nội dung này khám phá một số kỹ thuật học máy (ML techniques) mà các nhà thiết kế trí tuệ nhân tạo (AI designers) sử dụng để xây dựng chương trình trí tuệ nhân tạo (AI programs), giúp bạn hiểu sâu hơn cách học máy (ML) khai thác dữ liệu để đưa ra quyết định và thực hiện nhiệm vụ. Bạn cũng sẽ khám phá cách các kỹ thuật học máy (ML techniques) mở đường cho trí tuệ nhân tạo tạo sinh (generative AI).

## Kỹ Thuật Phát Triển Trí Tuệ Nhân Tạo (AI Development Techniques)

Trí tuệ nhân tạo (artificial intelligence) đề cập đến các chương trình máy tính có thể hoàn thành nhiệm vụ nhận thức thường liên quan đến trí tuệ con người. Có hai kỹ thuật chính để thiết kế chương trình trí tuệ nhân tạo (AI programs):

- **Kỹ thuật dựa trên quy tắc (rule-based techniques)**: Tạo chương trình trí tuệ nhân tạo (AI programs) tuân thủ nghiêm ngặt các quy tắc định trước để đưa ra quyết định. Ví dụ, bộ lọc thư rác sử dụng kỹ thuật này có thể chặn email chứa từ khóa cụ thể dựa trên logic định trước.
- **Kỹ thuật học máy (machine learning techniques)**: Tạo chương trình trí tuệ nhân tạo (AI programs) có thể phân tích và học từ mẫu trong dữ liệu để đưa ra quyết định độc lập. Ví dụ, bộ lọc thư rác sử dụng kỹ thuật này có thể đánh dấu thư rác tiềm năng để người nhận xem xét, tránh chặn tự động. Nếu người nhận đánh dấu email từ nguồn đáng tin cậy là an toàn, bộ lọc sẽ học và điều chỉnh logic để bao gồm email tương tự từ người gửi đó trong tương lai.

Công cụ trí tuệ nhân tạo (AI tools) có thể sử dụng kỹ thuật dựa trên quy tắc (rule-based techniques), kỹ thuật học máy (ML techniques), hoặc kết hợp cả hai. Nói chung, kỹ thuật dựa trên quy tắc (rule-based techniques) thường dùng cho nhiệm vụ yêu cầu tính cứng nhắc, như chặn tin nhắn từ người gửi không đáng tin rõ ràng là thư rác, chẳng hạn yêu cầu chuyển khoản ngân hàng hoặc thông tin cá nhân. Ngược lại, kỹ thuật học máy (ML techniques) phù hợp hơn cho nhiệm vụ đòi hỏi tính linh hoạt và thích ứng, như học nhận diện rằng tin nhắn từ người gửi đáng tin chứa lỗi chính tả không phải thư rác.

## Các Phương Pháp Huấn Luyện Chương Trình Học Máy (Approaches to Training ML Programs)

Học máy (machine learning) là một phần con của trí tuệ nhân tạo (AI), tập trung vào phát triển chương trình máy tính có thể phân tích dữ liệu để đưa ra quyết định hoặc dự đoán. Các nhà thiết kế trí tuệ nhân tạo (AI designers) thường sử dụng học máy (ML) trong chương trình trí tuệ nhân tạo (AI programs) vì nó không có hạn chế của kỹ thuật dựa trên quy tắc (rule-based techniques).

Có ba phương pháp phổ biến để huấn luyện chương trình học máy (ML programs):

- Học có giám sát (supervised learning)
- Học không giám sát (unsupervised learning)
- Học tăng cường (reinforcement learning)

**Học có giám sát (Supervised Learning)**  
Với phương pháp này, các nhà thiết kế trí tuệ nhân tạo (AI designers) cung cấp cho chương trình học máy (ML program) một tập huấn luyện có nhãn (labeled training set), và chương trình học từ dữ liệu đó. Tập huấn luyện có nhãn (labeled training set) bao gồm dữ liệu được gắn nhãn hoặc thẻ, cung cấp ngữ cảnh và ý nghĩa. Ví dụ, bộ lọc thư rác được huấn luyện bằng học có giám sát (supervised learning) sử dụng tập huấn luyện gồm email được gắn nhãn "thư rác" hoặc "không phải thư rác". Phương pháp này thường dùng khi có đầu ra cụ thể trong đầu.

**Học không giám sát (Unsupervised Learning)**  
Với phương pháp này, các nhà thiết kế trí tuệ nhân tạo (AI designers) cung cấp cho chương trình học máy (ML program) một tập huấn luyện không nhãn (unlabeled training set), và chương trình học từ dữ liệu đó. Tập huấn luyện không nhãn (unlabeled training set) bao gồm dữ liệu không có nhãn hoặc thẻ. Ví dụ, học máy (ML) có thể phân tích tập dữ liệu email chưa sắp xếp để tìm mẫu trong chủ đề, từ khóa hoặc liên hệ. Nói cách khác, học không giám sát (unsupervised learning) dùng để xác định mẫu trong dữ liệu mà không có đầu ra cụ thể.

**Học tăng cường (Reinforcement Learning)**  
Với phương pháp này, các nhà thiết kế trí tuệ nhân tạo (AI designers) cung cấp cho chương trình học máy (ML program) dữ liệu cho phép học qua thử và sai (trial-and-error). Chương trình học bằng cách nhận phần thưởng cho lựa chọn tốt dẫn đến kết quả mong muốn. Học tăng cường (reinforcement learning) thường dùng cho công cụ trí tuệ nhân tạo hội thoại (conversational AI tools). Khi các công cụ này nhận phản hồi từ người dùng và nhà thiết kế, chúng học cách tạo phản hồi hiệu quả.

Mỗi kỹ thuật học máy (ML technique) có điểm mạnh và yếu riêng. Tùy thuộc vào loại dữ liệu có sẵn và nhu cầu giải quyết vấn đề cụ thể, các nhà thiết kế trí tuệ nhân tạo (AI designers) có thể sử dụng một, hai hoặc cả ba kỹ thuật để tạo giải pháp dựa trên trí tuệ nhân tạo (AI-powered solution).

## Trí Tuệ Nhân Tạo Tạo Sinh (Generative AI)

Tiến bộ trong học có giám sát (supervised learning), học không giám sát (unsupervised learning) và học tăng cường (reinforcement learning) đã mở đường cho trí tuệ nhân tạo tạo sinh (generative AI) – trí tuệ nhân tạo (AI) có thể tạo nội dung mới, như văn bản, hình ảnh hoặc phương tiện khác. Khi người dùng cung cấp đầu vào dưới dạng lệnh (prompt) – đầu vào văn bản cung cấp hướng dẫn cho mô hình trí tuệ nhân tạo (AI model) về cách tạo đầu ra – công cụ trí tuệ nhân tạo (AI tool) xử lý đầu vào này để tạo nội dung mới.

Ví dụ, cả ba phương pháp đóng vai trò riêng biệt trong công cụ trí tuệ nhân tạo hội thoại (conversational AI tools). Học có giám sát (supervised learning) trang bị dữ liệu đối thoại cơ bản, cho phép phản hồi phù hợp với tín hiệu hội thoại thông thường. Học không giám sát (unsupervised learning) cho phép diễn giải sắc thái ngôn ngữ, như cách nói thông tục trong cuộc trò chuyện tự nhiên. Học tăng cường (reinforcement learning) củng cố thêm bằng cách cho phép cải thiện phản hồi thời gian thực dựa trên phản hồi người dùng, giúp thích ứng với ngữ cảnh hội thoại và tham gia cuộc trò chuyện tự nhiên.

Khả năng tạo và đổi mới của trí tuệ nhân tạo tạo sinh (generative AI) mang lại nhiều lợi ích cho các nơi làm việc và nghề nghiệp, như tiếp thị, phát triển sản phẩm, kỹ thuật, giáo dục, sản xuất và nghiên cứu phát triển. Các lợi ích bao gồm:

- **Hiệu quả cao hơn**: Trí tuệ nhân tạo tạo sinh (generative AI) có thể tự động hóa hoặc hỗ trợ nhiệm vụ routine, cho phép nhân viên tập trung vào ưu tiên khác.
- **Trải nghiệm cá nhân hóa**: Trí tuệ nhân tạo tạo sinh (generative AI) có thể điều chỉnh tương tác theo sở thích và nhu cầu cá nhân.
- **Quyết định tốt hơn**: Trí tuệ nhân tạo tạo sinh (generative AI) có thể phân tích nhanh lượng dữ liệu lớn để khám phá insights hữu ích.

Đây chỉ là một số cách trí tuệ nhân tạo tạo sinh (generative AI) có thể nâng cao công việc của bạn.

## Thông Tin Thêm

PAIR Explorables là tài nguyên tùy chọn cho bất kỳ ai muốn học thêm về trí tuệ nhân tạo (AI). Đây là bộ sưu tập bài viết tương tác được thiết kế để làm cho các khái niệm trí tuệ nhân tạo (AI) dễ tiếp cận và dễ hiểu hơn. PAIR Explorables bao gồm nhiều chủ đề, bao gồm:

- Cơ bản học máy (machine learning basics)
- Công bằng và thiên kiến trong chương trình trí tuệ nhân tạo (fairness and bias in AI programs)
- Xem xét dữ liệu và quyền riêng tư trong trí tuệ nhân tạo (data and privacy considerations in AI)
- Rủi ro và lợi ích tiềm năng của trí tuệ nhân tạo (potential risks and benefits of AI)

Mỗi bài viết có hình ảnh hóa và điều khiển tương tác giúp khám phá các khái niệm trí tuệ nhân tạo (AI) và trải nghiệm cách chúng hoạt động.

---

## Chủ Đề Liên Quan

- **Machine Learning cơ bản:** [[01 - 06 - Explore how AI uses machine learning]]
- **Training models:** [[02 - 05 - AI models and the training process]]
- **GenAI foundation:** [[01 - 07 - Foundations of generative AI]]
- **Bias trong AI:** [[04 - 02 - Understand bias in AI]]
- **Privacy & Security:** [[04 - 05 - Security and privacy risks of AI]]

---

## Điều Hướng

**⬅️ Quay lại:** [[01 - 07 - Foundations of generative AI]]

**➡️ Tiếp theo:** [[01 - 09 - Understand the capabilities and limitations of AI]]

**🏠 Trang chủ:** [[01 - 01 - Introduction to Google AI Essentials]]
