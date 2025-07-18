# Ghi Chú Học Tập: Prompt Cho Các Mục Đích Khác Nhau

## Giới Thiệu

Hãy nhớ rằng mô hình ngôn ngữ lớn (large language model - LLM) là mô hình AI được huấn luyện trên lượng lớn văn bản để nhận diện mẫu giữa từ ngữ, khái niệm và cụm từ, từ đó tạo phản hồi cho prompt. Prompt tốt giúp hướng dẫn LLM tạo đầu ra hữu ích cho công việc. Trong phần này, bạn sẽ khám phá cách viết prompt rõ ràng và cụ thể cho nhiều trường hợp sử dụng tại nơi làm việc.

## Các Trường Hợp Sử Dụng

LLM có thể giúp tăng năng suất và sáng tạo tại nơi làm việc qua các nhiệm vụ như:

- Tạo nội dung (Content creation).
- Tóm tắt (Summarization).
- Phân loại (Classification).
- Trích xuất (Extraction).
- Dịch (Translation).
- Chỉnh sửa (Editing).
- Giải quyết vấn đề (Problem-solving).

Lưu ý: Các ví dụ minh họa thực hành tốt nhất về prompting; không phải mẫu chính xác để sao chép. Kết quả thay đổi tùy LLM sử dụng. Luôn đánh giá phê phán đầu ra LLM và lặp lại prompt để có kết quả tốt nhất.

## Cách Làm Prompt Hiệu Quả Hơn

- Xem xét những gì bạn muốn LLM tạo ra. Bao gồm hướng dẫn cụ thể như create (tạo), summarize (tóm tắt), classify (phân loại), extract (trích xuất), translate (dịch), edit (chỉnh sửa), hoặc solve (giải quyết).
- Cung cấp ngữ cảnh cần thiết. Bao gồm hướng dẫn chi tiết về phong cách hoặc định dạng đầu ra mong muốn.

Dưới đây là ví dụ chi tiết cho từng trường hợp sử dụng.

## Tạo Nội Dung (Content Creation)

LLM giúp tạo nội dung như bài đăng blog, báo cáo, mô tả sản phẩm hoặc khẩu hiệu. Ví dụ, cho chiến dịch quảng cáo thiết bị gia dụng:

**Prompt mẫu (giữ nguyên tiếng Anh):**  
Act like you are a creative advertising professional who can apply innovative thinking to develop original taglines that project the positive qualities of a product. Create a concise tagline for a washing machine that gets clothes extra clean, has 25 settings, and fits in a small space.

(Dịch: Hãy hành động như một chuyên gia quảng cáo sáng tạo có thể áp dụng tư duy đổi mới để phát triển khẩu hiệu gốc nhấn mạnh phẩm chất tích cực của sản phẩm. Tạo khẩu hiệu ngắn gọn cho máy giặt làm sạch quần áo cực kỳ, có 25 chế độ, và phù hợp không gian nhỏ.)

Prompt nêu rõ nhiệm vụ là tạo khẩu hiệu gốc và ngắn gọn, cung cấp ngữ cảnh về giọng điệu, phong cách và định dạng.

**Mẹo chuyên nghiệp:** Giao vai trò, công việc hoặc chức năng cho LLM để củng cố mục đích prompt và hướng dẫn tạo đầu ra hữu ích.

## Tóm Tắt (Summarization)

LLM giúp tóm tắt báo cáo, khảo sát khách hàng, ghi chép họp, email, v.v. Ví dụ, tóm tắt email dài từ nhà cung cấp phần mềm:

**Prompt mẫu (giữ nguyên tiếng Anh):**  
The following text is an email from a software vendor. Summarize its main points in a bulleted list:

"""

I hope this finds you well. It was a pleasure to chat with you at the conference last week.

Following up with more detail on our pricing plans. Our bronze level subscription gets you access to three of our most popular software products as well as training videos for these products. If you have additional software needs, you can subscribe at the silver level. This level allows you to choose two additional software products, with training videos on those products, as well as gets you 24-hour support on any difficulties you encounter while using the products. Finally, our gold level membership gets you access to all ten of our software products. You get training for all ten products as well as 24-hour support, and you are also the first to enjoy any beta additions to our products.

Please contact me for the pricing of the level that interests you. We offer monthly subscriptions and a reduced rate for a yearly subscription.

"""

(Dịch: Văn bản sau là email từ nhà cung cấp phần mềm. Tóm tắt các điểm chính dưới dạng danh sách đánh dấu:

"""

Hy vọng email này tìm thấy bạn khỏe mạnh. Rất vui được trò chuyện với bạn tại hội nghị tuần trước.

Tiếp theo chi tiết về các gói giá của chúng tôi. Gói đồng cho phép truy cập ba sản phẩm phần mềm phổ biến nhất cùng video đào tạo. Nếu cần thêm, gói bạc cho phép chọn hai sản phẩm nữa, với video đào tạo và hỗ trợ 24 giờ. Cuối cùng, gói vàng cho phép truy cập tất cả mười sản phẩm, đào tạo đầy đủ, hỗ trợ 24 giờ và ưu tiên thử nghiệm beta.

Vui lòng liên hệ tôi để biết giá của gói bạn quan tâm. Chúng tôi cung cấp đăng ký hàng tháng và giảm giá cho đăng ký hàng năm.

""")

Prompt bắt đầu bằng ngữ cảnh về email, nêu rõ nhiệm vụ tóm tắt điểm chính, và chỉ định định dạng danh sách đánh dấu.

Lưu ý: LLM đôi khi hallucinate (tạo đầu ra không đúng sự thật), như thêm chi tiết không có trong nguồn. Luôn đánh giá độ chính xác.

## Phân Loại (Classification)

LLM giúp phân loại email dịch vụ khách hàng, nội dung mạng xã hội, hoặc phân tích cảm xúc phản hồi. Ví dụ, phân tích cảm xúc đánh giá khách hàng:

**Prompt mẫu (giữ nguyên tiếng Anh):**  
Read these customer reviews and tell me whether the sentiment of the reviews is positive, negative, or neutral.

- Customer Review: I don't know where to begin. We had reservations for 7:00 but they seated us at 7:45. Then, no one came to our table for at least 30 minutes. Our appetizer and main course were mediocre. I did love the dessert, but that wasn't enough to change our experience.
- Customer Review: I love this restaurant. The food is delicious and the service is excellent.

(Dịch: Đọc các đánh giá khách hàng này và cho tôi biết cảm xúc của chúng là tích cực, tiêu cực hay trung lập.

- Đánh giá Khách hàng: Tôi không biết bắt đầu từ đâu. Chúng tôi đặt chỗ lúc 7:00 nhưng được ngồi lúc 7:45. Sau đó, không ai đến bàn ít nhất 30 phút. Món khai vị và chính kém. Tôi thích món tráng miệng, nhưng không đủ thay đổi trải nghiệm.
- Đánh giá Khách hàng: Tôi yêu nhà hàng này. Thức ăn ngon và dịch vụ tuyệt vời.)

Prompt nêu rõ nhiệm vụ phân tích cảm xúc với lựa chọn: positive, negative, hoặc neutral, rồi cung cấp đánh giá.

## Trích Xuất (Extraction)

LLM giúp trích xuất dữ liệu từ văn bản và chuyển thành định dạng có cấu trúc. Ví dụ, trích xuất sản phẩm quần áo từ bài đăng blog:

**Prompt mẫu (giữ nguyên tiếng Anh):**  
Read the blog post below and extract all of the references to items of clothing I can buy and how much each item costs. Create a bulleted list of just these items.

- Blog post: Hey everybody, I want to share what I’m wearing on campus this fall. If I’m going out for the evening, I prefer the raw selvedge denim jeans ($150) paired with the cashmere crew neck sweater ($250). For a more casual look, I like the fleece hoodie ($99) and fleece sweatpants ($129). I also love every color of the striped socks ($15). They pair well with both the jeans and the sweats.

(Dịch: Đọc bài đăng blog dưới đây và trích xuất tất cả tham chiếu đến các món đồ quần áo có thể mua và giá của từng món. Tạo danh sách đánh dấu chỉ các món này.

- Bài đăng blog: Này mọi người, tôi muốn chia sẻ những gì tôi mặc trên khuôn viên trường mùa thu này. Nếu đi chơi tối, tôi thích quần jeans denim selvedge thô ($150) kết hợp áo len cashmere cổ tròn ($250). Để vẻ ngoài casual hơn, tôi thích áo hoodie fleece ($99) và quần sweatpants fleece ($129). Tôi cũng yêu mọi màu của tất sọc ($15). Chúng kết hợp tốt với cả jeans và sweatpants.)

Prompt nêu rõ nhiệm vụ trích xuất món đồ và giá, chỉ định định dạng danh sách đánh dấu, rồi cung cấp blog.

## Dịch (Translation)

LLM dịch văn bản nhanh giữa các ngôn ngữ. Ví dụ, dịch mô tả sản phẩm từ tiếng Anh sang tiếng Tây Ban Nha:

**Prompt mẫu (giữ nguyên tiếng Anh):**  
Translate our product descriptions from English to Spanish. Maintain the same structure and casual tone that is used in the English version in the Spanish translation.

- Bicycle: Whether you’re exploring city streets or forest paths, our sleek and durable bicycle has it all.
- Rollerblades: Roll into summer in style with our smooth and stylish rollerblades.

(Dịch: Dịch mô tả sản phẩm của chúng tôi từ tiếng Anh sang tiếng Tây Ban Nha. Giữ nguyên cấu trúc và giọng điệu casual như phiên bản tiếng Anh.

- Bicycle: Dù bạn đang khám phá đường phố thành phố hay lối rừng, chiếc xe đạp mượt mà và bền bỉ của chúng tôi có tất cả.
- Rollerblades: Lăn vào mùa hè phong cách với đôi giày trượt patin mượt mà và stylish của chúng tôi.)

Prompt nêu rõ nhiệm vụ dịch, chỉ định giữ cấu trúc và giọng điệu, rồi cung cấp mô tả với nhãn sản phẩm.

Lưu ý: Kiểm tra độ chính xác bằng công cụ dịch khác.

## Chỉnh Sửa (Editing)

LLM giúp chỉnh sửa văn bản, thay đổi giọng điệu hoặc kiểm tra ngữ pháp. Ví dụ, chỉnh báo cáo kỹ thuật dễ hiểu hơn:

**Prompt mẫu (giữ nguyên tiếng Anh):**  
Edit the language of the following paragraph so that it's easy for a general audience to understand it. Use simpler vocabulary and grammatical structures but maintain the same ideas.

Site selection for expansion is a complex and multifaceted process. The west side site offers several advantages, including zoning for industrial use and direct access to both a major highway and railroad. However, the site is also located in a jurisdiction with a complex and time-consuming permitting process, and its distance from residential zones may necessitate higher wages to attract workers.

(Dịch: Chỉnh sửa ngôn ngữ của đoạn văn sau để dễ hiểu với đối tượng chung. Sử dụng từ vựng và cấu trúc ngữ pháp đơn giản hơn nhưng giữ nguyên ý tưởng.

Việc chọn địa điểm mở rộng là quá trình phức tạp và đa diện. Địa điểm phía tây có nhiều lợi thế, bao gồm quy hoạch cho sử dụng công nghiệp và tiếp cận trực tiếp với xa lộ lớn và đường sắt. Tuy nhiên, địa điểm nằm ở khu vực có quy trình cấp phép phức tạp và tốn thời gian, và khoảng cách từ khu dân cư có thể đòi hỏi lương cao hơn để thu hút công nhân.)

Prompt nêu rõ nhiệm vụ chỉnh sửa để dễ hiểu, chỉ định đơn giản hóa từ vựng và ngữ pháp nhưng giữ ý, rồi cung cấp đoạn văn.

## Giải Quyết Vấn Đề (Problem-Solving)

LLM tạo giải pháp cho thách thức như phân tích dữ liệu bán hàng hoặc lập kế hoạch sự kiện. Ví dụ, tổ chức chương trình dạy trẻ em làm vườn:

**Prompt mẫu (giữ nguyên tiếng Anh):**  
We are running a community program to teach children gardening skills. The program runs from June 1 to August 15. We want the children to be able to grow plants that will be ready for harvest by the time the program ends. First, identify a list of 10 plants that can be planted and grown in that time period. Include sources that support the time to harvest for each plant.

We want the children to grow three plants. These plants should be as different from each other as possible. So next, choose three plants from the list that will provide the children with this variety.

(Dịch: Chúng tôi đang chạy chương trình cộng đồng dạy trẻ em kỹ năng làm vườn. Chương trình từ 1/6 đến 15/8. Chúng tôi muốn trẻ em trồng cây có thể thu hoạch khi chương trình kết thúc. Đầu tiên, xác định danh sách 10 cây có thể trồng và phát triển trong khoảng thời gian đó. Bao gồm nguồn hỗ trợ thời gian thu hoạch cho từng cây.

Chúng tôi muốn trẻ em trồng ba cây. Những cây này nên khác nhau nhất có thể. Vậy tiếp theo, chọn ba cây từ danh sách để cung cấp sự đa dạng này.)

Prompt bắt đầu bằng ngữ cảnh chương trình, chia vấn đề thành hai bước: xác định 10 cây với nguồn, rồi chọn ba cây đa dạng. Yêu cầu trích dẫn nguồn giúp xác minh độ chính xác.

---

## Navigation

⬅️ [[03 - 06 - Leverage an LLM's capabilities at work|Khai thác khả năng của LLM tại nơi làm việc]] | [[03 - 08 - Improve AI output through iteration|Cải thiện đầu ra AI qua lặp lại]] ➡️

🏠 [[README|Trang chủ khóa học]]

---

## Chủ Đề Liên Quan

- [[01 - 07 - Foundations of generative AI|Nền tảng của AI sinh tạo]]
- [[02 - 09 - Generative AI tools for workplace tasks|Công cụ AI sinh tạo cho công việc]]
- [[03 - 04 - Write clear and specific prompts|Viết prompt rõ ràng và cụ thể]]
- [[03 - 05 - Prompting best practices|Thực hành tốt nhất cho prompting]]
- [[03 - 08 - Improve AI output through iteration|Cải thiện đầu ra AI qua lặp lại]]
- [[03 - 09 - Discover few-shot prompting|Khám phá few-shot prompting]]

---

## Tóm Tắt Module 3

Việc nắm vững các loại prompt khác nhau giúp tối ưu hóa việc sử dụng LLM cho nhiều mục đích công việc khác nhau.
