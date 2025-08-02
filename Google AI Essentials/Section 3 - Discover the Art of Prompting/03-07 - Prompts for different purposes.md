## Prompt cho các Mục đích Khác nhau

### Tổng quan về LLM và Prompting

**Large Language Model (LLM)** là mô hình AI được huấn luyện trên lượng lớn văn bản để nhận diện các mẫu giữa từ, khái niệm và cụm từ, từ đó có thể tạo ra phản hồi cho các prompt.

**Nguyên tắc prompting hiệu quả:**

- **Xác định rõ output mong muốn:** LLM sẽ tạo ra kết quả hữu ích hơn khi bạn bao gồm hướng dẫn cụ thể như create, summarize, classify, extract, translate, edit, hoặc solve
- **Cung cấp context cần thiết:** LLM tạo ra output hữu ích hơn khi bạn bao gồm hướng dẫn chi tiết với guidance cụ thể về style hoặc format mong muốn


### Các Use Cases Chính

#### 1. Tạo Nội dung (Content Creation)

**Ứng dụng:** Tạo blog posts, báo cáo, mô tả sản phẩm, taglines cho nhiều ngành nghề khác nhau.

**Ví dụ thực tế - Tạo tagline cho chiến dịch quảng cáo:**

```
Act like you are a creative advertising professional who can apply innovative thinking to develop original taglines that project the positive qualities of a product. Create a concise tagline for a washing machine that gets clothes extra clean, has 25 settings, and fits in a small space.
```

**Đặc điểm prompt hiệu quả:**

- **Nhiệm vụ rõ ràng:** Tạo tagline ngắn gọn và độc đáo
- **Context cần thiết:** Xác định tone, style và format của tagline
- **Gán vai trò:** Assign LLM một role, job hoặc function để tăng hiệu quả

**💡 Pro tip:** Gán cho LLM một vai trò cụ thể để củng cố mục đích của prompt và hướng dẫn LLM tạo ra output hữu ích.

#### 2. Tóm tắt (Summarization)

**Ứng dụng:** Tóm tắt reports, customer surveys, meeting notes, emails và nhiều loại văn bản khác.

**Ví dụ thực tế - Tóm tắt email từ software vendor:**

```
The following text is an email from a software vendor. Summarize its main points in a bulleted list:

"""
I hope this finds you well. It was a pleasure to chat with you at the conference last week.
Following up with more detail on our pricing plans. Our bronze level subscription gets you access to three of our most popular software products as well as training videos for these products. If you have additional software needs, you can subscribe at the silver level. This level allows you to choose two additional software products, with training videos on those products, as well as gets you 24-hour support on any difficulties you encounter while using the products. Finally, our gold level membership gets you access to all ten of our software products. You get training for all ten products as well as 24-hour support, and you are also the first to enjoy any beta additions to our products.
Please contact me for the pricing of the level that interests you. We offer monthly subscriptions and a reduced rate for a yearly subscription.
"""
```

**Cấu trúc prompt:**

- **Context hữu ích:** Giải thích nguồn gốc email
- **Nhiệm vụ rõ ràng:** Tóm tắt các điểm chính
- **Format cụ thể:** Định dạng bulleted list

**⚠️ Lưu ý quan trọng:** LLM có thể hallucinate - tạo ra output không đúng sự thật. Luôn đánh giá độ chính xác trước khi sử dụng.

#### 3. Phân loại (Classification)

**Ứng dụng:** Phân loại customer service emails, categorize social media content, phân tích sentiment của customer feedback.

**Ví dụ thực tế - Phân tích sentiment:**

```
Read these customer reviews and tell me whether the sentiment of the reviews is positive, negative, or neutral.

- Customer Review: I don't know where to begin. We had reservations for 7:00 but they seated us at 7:45. Then, no one came to our table for at least 30 minutes. Our appetizer and main course were mediocre. I did love the dessert, but that wasn't enough to change our experience.
- Customer Review: I love this restaurant. The food is delicious and the service is excellent.
```

**Cấu trúc prompt:**

- **Nhiệm vụ rõ ràng:** Phân tích sentiment
- **Options cụ thể:** positive, negative, hoặc neutral
- **Label rõ ràng:** "Customer Review" để định dạng input


#### 4. Trích xuất Dữ liệu (Extraction)

**Định nghĩa:** Kéo dữ liệu từ text và chuyển đổi thành định dạng có cấu trúc dễ hiểu hơn.

**Ví dụ thực tế - Trích xuất thông tin sản phẩm từ blog:**

```
Read the blog post below and extract all of the references to items of clothing I can buy and how much each item costs. Create a bulleted list of just these items.

- Blog post: Hey everybody, I want to share what I'm wearing on campus this fall. If I'm going out for the evening, I prefer the raw selvedge denim jeans ($150) paired with the cashmere crew neck sweater ($250). For a more casual look, I like the fleece hoodie ($99) and fleece sweatpants ($129). I also love every color of the striped socks ($15). They pair well with both the jeans and the sweats.
```

**Cấu trúc prompt:**

- **Nhiệm vụ cụ thể:** Trích xuất items quần áo và giá
- **Format output:** Bulleted list
- **Source content:** Blog post đầy đủ


#### 5. Dịch thuật (Translation)

**Ứng dụng:** Dịch text giữa các ngôn ngữ khác nhau một cách nhanh chóng.

**Ví dụ thực tế - Dịch product descriptions:**

```
Translate our product descriptions from English to Spanish. Maintain the same structure and casual tone that is used in the English version in the Spanish translation.

- Bicycle: Whether you're exploring city streets or forest paths, our sleek and durable bicycle has it all.
- Rollerblades: Roll into summer in style with our smooth and stylish rollerblades.
```

**Yêu cầu chất lượng:**

- **Nhiệm vụ rõ ràng:** Dịch từ English sang Spanish
- **Yêu cầu style:** Giữ nguyên structure và casual tone
- **Format input:** Label cho mỗi product

**📝 Best practice:** Xác nhận độ chính xác của bản dịch bằng cách cross-check với công cụ dịch khác.

#### 6. Chỉnh sửa (Editing)

**Ứng dụng:** Chỉnh sửa và viết lại text - thay đổi tone từ formal sang casual, grammar check.

**Ví dụ thực tế - Đơn giản hóa technical report:**

```
Edit the language of the following paragraph so that it's easy for a general audience to understand it. Use simpler vocabulary and grammatical structures but maintain the same ideas.

Site selection for expansion is a complex and multifaceted process. The west side site offers several advantages, including zoning for industrial use and direct access to both a major highway and railroad. However, the site is also located in a jurisdiction with a complex and time-consuming permitting process, and its distance from residential zones may necessitate higher wages to attract workers.
```

**Yêu cầu editing:**

- **Target audience:** General audience
- **Yêu cầu cụ thể:** Vocabulary và grammar đơn giản hơn
- **Giữ nguyên:** Main content và ideas


#### 7. Giải quyết Vấn đề (Problem-solving)

**Ứng dụng:** Tạo giải pháp cho workplace challenges - từ phân tích sales data đến lập kế hoạch sự kiện.

**Ví dụ thực tế - Tổ chức chương trình nonprofit:**

```
We are running a community program to teach children gardening skills. The program runs from June 1 to August 15. We want the children to be able to grow plants that will be ready for harvest by the time the program ends. First, identify a list of 10 plants that can be planted and grown in that time period. Include sources that support the time to harvest for each plant.

We want the children to grow three plants. These plants should be as different from each other as possible. So next, choose three plants from the list that will provide the children with this variety.
```

**Cấu trúc problem-solving prompt:**

- **Context đầy đủ:** Mục đích chương trình và timeline
- **Chia nhỏ vấn đề:** Hai bước cụ thể
- **Yêu cầu sources:** Để verify độ chính xác


### Ghi chú quan trọng

**Nguyên tắc chung:**

- Các ví dụ minh họa best practices, không phải exact templates
- Kết quả có thể khác nhau tùy thuộc vào LLM cụ thể
- **Luôn đánh giá critically** tất cả LLM output
- **Iterate** prompt ban đầu để có output hữu ích nhất

**Factors ảnh hưởng kết quả:**

- Specific LLM đang sử dụng
- Cách diễn đạt prompt
- Context và examples được cung cấp
- Độ rõ ràng của instructions

**Liên kết:** [[LLM]], [[Content Creation]], [[Summarization]], [[Classification]], [[Data Extraction]], [[Translation]], [[Editing]], [[Problem-solving]], [[Prompt Engineering]], [[Hallucination]], [[Context]], [[Workplace AI]]

