## Kỹ thuật Prompt Chaining (Nối Chuỗi Prompt)

### Khái niệm Cơ bản

**Prompt Chaining** là kỹ thuật hướng dẫn công cụ AI sinh tạo thông qua một chuỗi các prompt có liên kết với nhau, mỗi bước đều bổ sung thêm ngữ cảnh hoặc nhiệm vụ mới.

**Ví dụ minh họa**: Giống như ghép hình jigsaw puzzle

- Không đổ tất cả mảnh ghép ra rồi hy vọng may mắn
- Có kế hoạch cụ thể: tìm các mảnh góc → xây dựng viền → làm phần giữa
- Hoặc hoàn thành các phần nhỏ trước khi nối thành bức tranh lớn
- **Quá trình có chủ đích và xây dựng theo thời gian**


### Cách Thức Hoạt động

- Mỗi prompt và phản hồi được xây dựng dựa trên prompt trước đó
- Tạo ra một chuỗi prompt liên kết trong một chuỗi duy nhất
- Giúp giải quyết các vấn đề phức tạp từng bước một
- **Khác với iteration**: Thay vì chỉ điều chỉnh prompt để cải thiện kết quả, prompt chaining sử dụng output làm khối xây dựng cho các yêu cầu phức tạp hơn


### Ví dụ Thực tế: Catch-up Sau Kỳ Nghỉ

**Tình huống**: Cần cập nhật công việc sau khi nghỉ

1. **Prompt đầu tiên**: Tóm tắt email và tài liệu nhận được khi vắng mặt
2. **Prompt thứ hai**: Tập trung vào các yêu cầu cấp thiết sau khi xem output
3. **Prompt thứ ba**: Đưa ra giải pháp xử lý các vấn đề khẩn cấp được phát hiện
4. **Tiếp tục chuỗi**: Mỗi bước xây dựng dựa trên bước trước

### Thực hành với Google AI Studio

**Công cụ sử dụng**: [[Google AI Studio]] với [[Gemini Models]] có cửa sổ ngữ cảnh dài (long context window)

#### Dự án Mẫu: Marketing Sách

**Bối cảnh**: Vừa hoàn thành viết tiểu thuyết, cần tạo kế hoạch marketing

**Bước 1: Tạo Tagline**

```
Prompt: Generate three options for a one sentence summary of this novel manuscript. The summary should be similar in voice and tone to the manuscript, but more catchy and engaging.
```

**Bước 2: Tinh chỉnh Tagline**

```
Prompt: Create a tagline that is a combination of the previous three options with a special focus on the exciting plot twists and mystery of the book. Find the catchiest and most impactful combination. The tagline should be concise and leave the reader hooked and wanting to read more.
```

**Bước 3: Tạo Blurb cho Bìa Sau**

```
Prompt: Create a five sentence summary of the entire manuscript below that expands on the one sentence summary.
```

**Bước 4: Lập Kế hoạch Book Tour**

```
Prompt: Generate a six week promotional plan for a book tour, including what locations I should visit and what channels I should utilize to promote each stop on the tour.
```


### Lợi Ích Của Prompt Chaining

- **Tận dụng ngữ cảnh**: Model đã phân tích manuscript và nhớ cuộc hội thoại nhờ long context window
- **Xây dựng tích lũy**: Mỗi output trở thành nền tảng cho yêu cầu phức tạp hơn
- **Hiệu quả cao**: Chỉ cần một chuỗi prompt để tạo ra tagline, tóm tắt và kế hoạch book tour
- **Linh hoạt**: Vẫn có thể iteration trên bất kỳ prompt nào nếu không hài lòng với kết quả


### Ghi chú Quan trọng

- Prompt chaining **không chỉ là việc thêm ngữ cảnh** vào prompt
- Mà là **mở rộng dựa trên những gì AI đã tạo ra trước đó**
- Khác biệt với [[Iteration]] trong [[Prompt Framework]]: iteration tập trung điều chỉnh prompt để cải thiện kết quả, còn chaining sử dụng output làm building block

**Liên kết**: [[Prompt Chaining]], [[Google AI Studio]], [[Gemini Models]], [[Long Context Window]], [[Prompt Framework]], [[Iteration]], [[Generative AI]]

