## Ghi Chú Học Tập: Thiên Kiến, Trôi Dạt Và Giới Hạn Kiến Thức

## Giới Thiệu

- Việc hiểu sâu các khái niệm trong AI có trách nhiệm (responsible AI) – chẳng hạn như thiên kiến (bias), trôi dạt (drift) và giới hạn kiến thức (knowledge cutoff) – giúp sử dụng AI đạo đức hơn và với trách nhiệm lớn hơn.
    
- Tài liệu này hướng dẫn sử dụng công cụ AI có trách nhiệm và hiểu hậu quả của đầu ra không công bằng hoặc không chính xác.
    

## Hại Và Thiên Kiến

- Sử dụng AI có trách nhiệm đòi hỏi nhận thức về thiên kiến nội tại. Thiên kiến dữ liệu (data biases) là tình huống lỗi hệ thống hoặc định kiến dẫn đến thông tin không công bằng hoặc không chính xác, tạo đầu ra thiên vị.
    
- Sử dụng AI có trách nhiệm và nhận thức về thiên kiến tiềm ẩn giúp tránh các loại hại.
    
- Đầu ra thiên vị có thể gây nhiều loại hại cho con người và xã hội, bao gồm:
    
- **Hại Phân Bổ (Allocative Harm)**: Sai phạm xảy ra khi hệ thống AI từ chối cơ hội, tài nguyên hoặc thông tin trong lĩnh vực ảnh hưởng đến phúc lợi cá nhân.
    
    - Ví dụ: Nếu quản lý bất động sản sử dụng công cụ AI kiểm tra lý lịch để sàng lọc đơn thuê căn hộ, AI có thể nhầm danh tính ứng viên và coi họ rủi ro do điểm tín dụng thấp, dẫn đến từ chối căn hộ và mất phí nộp đơn.
        
    - Cách giảm thiểu: Đánh giá tất cả nội dung do AI tạo trước khi tích hợp vào công việc hoặc chia sẻ. Tránh tình huống như ví dụ bằng cách kiểm tra chéo đầu ra AI với nguồn khác.
        
- **Hại Chất Lượng Dịch Vụ (Quality-of-Service Harm)**: Tình huống công cụ AI hoạt động kém hơn đối với một số nhóm người dựa trên đặc tính cá nhân.
    
    - Ví dụ: Khi công nghệ nhận diện giọng nói (speech-recognition technology) mới phát triển, dữ liệu huấn luyện thiếu mẫu giọng nói của người khuyết tật, dẫn đến thiết bị khó phân tích loại giọng này.
        
    - Cách giảm thiểu: Chỉ định sự đa dạng bằng cách thêm ngôn ngữ hòa nhập vào lời nhắc (prompt). Nếu công cụ AI tạo sinh (generative AI) bỏ qua nhóm hoặc đặc tính như người khuyết tật, giải quyết vấn đề khi lặp lại lời nhắc.
        
- **Hại Đại Diện (Representational Harm)**: Công cụ AI củng cố sự hạ thấp các nhóm xã hội dựa trên đặc tính của họ.
    
    - Ví dụ: Khi công nghệ dịch (translation technology) mới phát triển, một số đầu ra lệch không chính xác về nam tính hoặc nữ tính. Ví dụ, dịch từ như "nurse" và "beautiful" lệch nữ tính, trong khi "doctor" và "strong" lệch nam tính.
        
    - Cách giảm thiểu: Thách thức giả định. Nếu công cụ AI tạo phản hồi thiên vị như lệch nam/nữ, xác định và giải quyết khi lặp lại lời nhắc, yêu cầu công cụ sửa thiên kiến.
        
- **Hại Hệ Thống Xã Hội (Social System Harm)**: Tác động xã hội ở mức vĩ mô, khuếch đại sự chênh lệch giai cấp, quyền lực hoặc đặc quyền hiện có, hoặc gây hại vật lý từ phát triển/sử dụng công cụ AI.
    
    - Ví dụ: Deepfake không mong muốn (deepfakes) – ảnh hoặc video giả mạo do AI tạo, cho thấy người thật nói hoặc làm điều họ không làm – là ví dụ về hại hệ thống xã hội.
        
    - Cách giảm thiểu: Kiểm tra sự thật và tham chiếu chéo đầu ra. Một số công cụ AI tạo sinh có tính năng cung cấp nguồn thông tin. Kiểm tra sự thật bằng công cụ tìm kiếm để xác nhận, hoặc hỏi chuyên gia. Chạy lời nhắc qua hai hoặc nhiều tài nguyên giúp phát hiện đầu ra không chính xác.
        
- **Hại Liên Cá Nhân (Interpersonal Harm)**: Sử dụng công nghệ để tạo bất lợi cho một số người, ảnh hưởng tiêu cực đến mối quan hệ hoặc gây mất cảm giác tự chủ và bản ngã.
    
    - Ví dụ: Nếu ai đó kiểm soát thiết bị gia đình ở căn hộ cũ để chơi khăm bạn cùng phòng cũ, hành động này có thể gây mất cảm giác tự chủ và bản ngã cho người bị ảnh hưởng.
        
    - Cách giảm thiểu: Xem xét hiệu quả sử dụng AI, luôn dùng phán đoán tốt nhất và kỹ năng tư duy phê phán. Tự hỏi AI có phù hợp với nhiệm vụ không. AI có thể hữu ích hoặc hại tùy cách sử dụng, và người dùng chịu trách nhiệm tránh gây hại.
        

## Trôi Dạt So Với Giới Hạn Kiến Thức

- Hiện tượng khác gây đầu ra không công bằng hoặc không chính xác là trôi dạt (drift) – sự suy giảm độ chính xác dự đoán của mô hình AI do thay đổi theo thời gian không phản ánh trong dữ liệu huấn luyện.
    
- Thường do giới hạn kiến thức (knowledge cutoff) – khái niệm mô hình được huấn luyện tại thời điểm cụ thể, nên không biết sự kiện hoặc thông tin sau ngày đó.
    
- Ví dụ: Nhà thiết kế thời trang muốn theo dõi xu hướng chi tiêu trước khi tạo bộ sưu tập mới. Nếu sử dụng mô hình huấn luyện cuối cùng trên xu hướng thời trang và thói quen tiêu dùng từ 2015, mô hình có thể không tạo đầu ra hữu ích vì các yếu tố này thay đổi theo thời gian. Sở thích tiêu dùng năm 2015 khác hẳn xu hướng hiện nay. Nói cách khác, dự đoán của mô hình trôi dạt từ chính xác lúc huấn luyện sang kém chính xác hiện tại, phần nào do giới hạn kiến thức.
    
- Các yếu tố khác gây trôi dạt, làm mô hình AI kém đáng tin cậy: Thiên kiến trong dữ liệu mới, thay đổi hành vi con người và sử dụng công nghệ, hoặc sự kiện lớn trên thế giới.
    
- Để duy trì mô hình AI hoạt động tốt, cần giám sát hiệu suất thường xuyên và giải quyết giới hạn kiến thức bằng cách tiếp cận con người trong vòng lặp (human-in-the-loop approach).
    

## Tài Nguyên Khám Phá Thêm

- Để khám phá thiên kiến, dữ liệu, trôi dạt và giới hạn kiến thức, thử bài tập "What Have Language Models Learned?" từ Google PAIR Explorables. Ở đó, tương tác với BERT – một trong những mô hình ngôn ngữ lớn (large language models – LLMs) đầu tiên – và khám phá cách tương quan dữ liệu dẫn đến thiên kiến vấn đề trong kết quả.
    
- Kiểm tra các PAIR AI Explorables khác để học thêm về AI có trách nhiệm.