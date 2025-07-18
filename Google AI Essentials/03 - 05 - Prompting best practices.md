# Ghi Chú Học Tập: Các Thực Hành Tốt Nhất Về Prompting

## Giới Thiệu

Prompting là kỹ năng thiết yếu để tận dụng tối đa trí tuệ nhân tạo tạo sinh (generative AI). Để đạt kết quả tốt nhất từ công cụ AI, bạn cần xây dựng một prompt tốt. Một prompt tốt tuân theo khung đơn giản: Task (Nhiệm vụ), Context (Ngữ cảnh), References (Tham chiếu), Evaluate (Đánh giá), và Iterate (Lặp lại). Khung này giúp nâng cao kỹ năng prompting và khai thác nhiều lợi ích hơn từ AI.

## Xác Định Nhiệm Vụ (Specify the Task)

Xác định nhiệm vụ là nền tảng của mọi prompt. Mô tả chi tiết những gì bạn muốn công cụ AI thực hiện, rõ ràng và tránh mơ hồ. Nhiệm vụ mơ hồ có thể dẫn đến đầu ra không liên quan hoặc sai lệch. Nhiệm vụ có thể bao gồm persona và định dạng ưu tiên để cụ thể hơn:

- **Nhiệm vụ (Task):** Hành động bạn muốn công cụ hỗ trợ, ví dụ viết email hoặc tạo hình ảnh.
    
- **Persona:** Chuyên môn mà công cụ AI cần sử dụng, và đối tượng mục tiêu. Ví dụ, thực hiện nhiệm vụ với chuyên môn của chuyên gia CNTT, hoặc tạo đầu ra hướng đến quản lý hoặc đội ngũ.
    
- **Định dạng (Format):** Cách định dạng đầu ra, ví dụ danh sách đánh dấu hoặc bảng so sánh.
    

**Prompt mẫu (giữ nguyên tiếng Anh):**  
You're a concert promoter specializing in raising ticket sales in the alternative rock music industry. Create a social media post about an upcoming music festival that speaks to the local music community while attracting out-of-state festival-goers. Limit the post to 125-characters. Include 5 relevant hashtags.

(Dịch: Bạn là một nhà quảng bá buổi hòa nhạc chuyên nâng cao doanh số vé trong ngành nhạc alternative rock. Tạo bài đăng mạng xã hội về lễ hội âm nhạc sắp tới, nói chuyện với cộng đồng âm nhạc địa phương đồng thời thu hút du khách từ ngoài tiểu bang. Giới hạn bài đăng ở 125 ký tự. Bao gồm 5 hashtag liên quan.)

## Cung Cấp Ngữ Cảnh Cần Thiết (Provide Necessary Context)

Bao gồm ngữ cảnh chi tiết trong prompt giúp thu hẹp trọng tâm của công cụ AI, tạo đầu ra phù hợp và hiệu quả hơn. Thông tin ngữ cảnh có thể bao gồm:

- Lý do và mục tiêu thực hiện nhiệm vụ.
    
- Quy tắc hoặc hướng dẫn mà đầu ra phải tuân theo.
    
- Thông tin nền tảng liên quan mà công cụ cần xem xét.
    

Những chi tiết này giúp công cụ AI hiểu rõ nhu cầu của bạn.

**Prompt mẫu (giữ nguyên tiếng Anh):**  
You're a concert promoter specializing in raising ticket sales in the alternative rock music industry. Create a social media post about an upcoming music festival that speaks to the local music community while attracting out-of-state festival-goers. Limit the post to 125-characters. Include 5 relevant hashtags. The local audience is primarily college students and young professionals (age 21-35) who follow indie rock. The festival features 12 bands over 2 days, with camping options and local food vendors.

(Dịch: Bạn là một nhà quảng bá buổi hòa nhạc chuyên nâng cao doanh số vé trong ngành nhạc alternative rock. Tạo bài đăng mạng xã hội về lễ hội âm nhạc sắp tới, nói chuyện với cộng đồng âm nhạc địa phương đồng thời thu hút du khách từ ngoài tiểu bang. Giới hạn bài đăng ở 125 ký tự. Bao gồm 5 hashtag liên quan. Đối tượng địa phương chủ yếu là sinh viên đại học và chuyên gia trẻ (tuổi 21-35) theo dõi indie rock. Lễ hội có 12 ban nhạc trong 2 ngày, với lựa chọn cắm trại và quầy thức ăn địa phương.)

Prompt này có khả năng tạo đầu ra hấp dẫn và hiệu quả hơn, phù hợp với đối tượng cụ thể mà không cần lặp lại thêm.

## Bao Gồm Tham Chiếu Như Ví Dụ (Include References as Examples)

Tham chiếu cung cấp ví dụ hoặc tài nguyên minh họa những gì bạn muốn công cụ AI tạo ra, chỉ định chi tiết về phong cách, giọng điệu và định dạng. Tùy công cụ AI, bạn có thể bao gồm văn bản, hình ảnh, âm thanh hoặc video làm tham chiếu.

Gợi ý khi bao gồm tham chiếu:

- Giải thích ngắn gọn cách tham chiếu liên quan đến nhiệm vụ.
    
- Sử dụng 2-5 ví dụ chất lượng cao phù hợp chặt chẽ với nhu cầu.
    
- Bao gồm tác phẩm của bạn hoặc ví dụ nguồn mở nếu liên quan.
    

**Prompt mẫu (giữ nguyên tiếng Anh):**  
You're a concert promoter specializing in raising ticket sales in the alternative rock music industry. Create a social media post about an upcoming music festival that speaks to the local music community while attracting out-of-state festival-goers. Limit the post to 125-characters. Include 5 relevant hashtags. The local audience is primarily college students and young professionals (age 21-35) who follow indie rock. The festival features 12 bands over 2 days, with camping options and local food vendors. Here are examples of successful posts from similar events:

- Example 1: Where mountains meet music: Indie Rocks Festival returns! Your favorite local bands + national acts. Good eats & Sleep under the stars! #Indie Rocks #SupportLocalMusic
    
- Example 2: Join Indie Fest under the desert skies! 2 nights of raw sound 2 move you + camping vibes #RoadTrip #CampLife #RockOn
    

(Dịch: Bạn là một nhà quảng bá buổi hòa nhạc chuyên nâng cao doanh số vé trong ngành nhạc alternative rock. Tạo bài đăng mạng xã hội về lễ hội âm nhạc sắp tới, nói chuyện với cộng đồng âm nhạc địa phương đồng thời thu hút du khách từ ngoài tiểu bang. Giới hạn bài đăng ở 125 ký tự. Bao gồm 5 hashtag liên quan. Đối tượng địa phương chủ yếu là sinh viên đại học và chuyên gia trẻ (tuổi 21-35) theo dõi indie rock. Lễ hội có 12 ban nhạc trong 2 ngày, với lựa chọn cắm trại và quầy thức ăn địa phương. Dưới đây là ví dụ về các bài đăng thành công từ sự kiện tương tự:

- Ví dụ 1: Nơi núi non gặp gỡ âm nhạc: Lễ hội Indie Rocks trở lại! Các ban nhạc địa phương yêu thích + nghệ sĩ quốc gia. Thức ăn ngon & Ngủ dưới sao! #IndieRocks #SupportLocalMusic
    
- Ví dụ 2: Tham gia Indie Fest dưới bầu trời sa mạc! 2 đêm âm thanh thô sơ lay động bạn + không khí cắm trại #RoadTrip #CampLife #RockOn)
    

Lưu ý: Sau trong khóa học, bạn sẽ học thêm về kỹ thuật prompting sử dụng tham chiếu.

## Đánh Giá Đầu Ra (Evaluate Your Output)

Công cụ AI khác nhau về đào tạo và khả năng, mỗi công cụ có điểm mạnh và hạn chế ảnh hưởng đến chất lượng đầu ra. Sau khi nhận phản hồi, cần đánh giá kỹ chất lượng và hiệu quả của nội dung do AI tạo trước khi sử dụng hoặc chia sẻ.

Tập trung vào các yếu tố khi đánh giá:

- Độ chính xác (Accuracy).
    
- Thiên kiến (Bias).
    
- Tính liên quan (Relevancy).
    
- Tính nhất quán (Consistency).
    

Nội dung do AI tạo nên là điểm khởi đầu, không phải sản phẩm cuối cùng. Nếu đầu ra không chấp nhận được hoặc không hữu ích, tiếp tục bước tiếp theo trong khung prompting.

## Lặp Lại Để Có Kết Quả Tốt Hơn (Iterate for Better Results)

Ngay cả prompt được xây dựng tốt cũng có thể không tạo kết quả lý tưởng ngay lần đầu. Lặp lại là quá trình tinh chỉnh prompt dựa trên đầu ra của AI, giống như cuộc trò chuyện qua lại với công cụ AI. Quy trình thường diễn ra như sau:

- Bạn cung cấp prompt ban đầu.
    
- Công cụ AI phản hồi với đầu ra.
    
- Bạn đánh giá hiệu quả của phản hồi do AI tạo.
    
- Bạn tinh chỉnh yêu cầu dựa trên những gì hiệu quả và không hiệu quả.
    
- Lặp lại chu kỳ đến khi đạt kết quả mong muốn.
    

Prompting hiệu quả không phải về kết quả hoàn hảo ngay lần đầu, mà là sẵn sàng tinh chỉnh và cải thiện cách tiếp cận. Hãy kiên nhẫn, cung cấp phản hồi rõ ràng và tiếp tục prompting đến khi đạt kết quả.

**Mẹo chuyên nghiệp:** Khi có prompt hiệu quả cho nhiệm vụ cụ thể, hãy lưu lại! Sử dụng chúng như mẫu cho các trường hợp sử dụng khác, giúp tái tạo đầu ra AI thành công mà không cần bắt đầu từ đầu.

## Tiếp Tục Học Tập (Continue Your Learning)

Sau khi hoàn thành Google AI Essentials, nâng cao kỹ năng prompting với khóa học Google Prompting Essentials. Do chuyên gia AI tại Google giảng dạy, khóa tự học này hoàn thành dưới 10 giờ, không yêu cầu kinh nghiệm trước, áp dụng cho nhiều ngành. Khám phá cách AI giúp tạo nội dung, phân tích dữ liệu và tóm tắt thông tin. Trong khóa học, bạn sẽ học cách prompting hiệu quả để AI làm việc cho bạn.