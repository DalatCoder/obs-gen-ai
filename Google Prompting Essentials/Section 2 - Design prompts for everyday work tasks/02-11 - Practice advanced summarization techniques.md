## Kỹ thuật Chain of Density Prompting - Phương pháp tóm tắt nâng cao

### Khái niệm Chain of Density Prompting

**Chain of Density Prompting** là kỹ thuật giúp tạo ra các bản tóm tắt ngày càng súc tích hơn và cuối cùng tạo thành một chuỗi các đầu ra được tinh chỉnh liên tục.

**Vấn đề thường gặp:**

- Khi yêu cầu công cụ AI tạo sinh tóm tắt, đôi khi kết quả đầu ra quá rộng
- Cần thêm chi tiết để làm cho bản tóm tắt thực sự hữu ích


### Ví dụ minh họa: Elevator Pitch

**So sánh với quy trình tạo elevator pitch hoàn hảo:**

- **Bản thảo đầu tiên:** Quá dài và bao gồm quá nhiều chi tiết
- **Qua các lần tinh chỉnh:** Ngắn gọn và trực tiếp hơn, không mất đi những điểm quan trọng
- **Kết quả cuối cùng:** Elevator pitch hoàn hảo - nhanh, trực tiếp và hiệu quả


### Quy trình thực hiện

#### Bước 1: Tóm tắt ngắn hơn với focus cụ thể

**Prompt mẫu:**

```
Cung cấp bản tóm tắt ngắn hơn, tập trung vào 2-3 xu hướng hàng đầu của báo cáo.
```


#### Bước 2: Rút gọn thành một câu duy nhất

**Prompt tiếp theo:**

```
Cô đọng bản tóm tắt thành một câu duy nhất, làm nổi bật xu hướng chủ đạo nhất.
```

**Nguyên tắc quan trọng:**

- Tiếp tục yêu cầu tinh chỉnh thêm
- Trực tiếp và cụ thể về đầu ra mong muốn
- Lặp lại quy trình cho đến khi tạo ra kết quả hữu ích và hữu ích nhất


#### Bước 3: Tối ưu hóa bằng prompt đa tầng

**Kỹ thuật nâng cao:** Có thể vượt qua các bước lặp lại bổ sung bằng cách yêu cầu công cụ AI cung cấp nhiều lần lặp ngày càng ngắn trong prompt ban đầu.

### Lý do sử dụng phương pháp lặp lại

#### Kiểm soát Hallucination (Ảo giác)

**Tại sao không đi thẳng đến kết quả ngắn nhất:**

- Lặp lại giúp kiểm tra **hallucination (ảo giác)** khi đi từ kết quả siêu chi tiết đến đầu ra trực tiếp hơn
- Giúp theo dõi thông tin nào đang bị loại bỏ khi đầu ra ngắn hơn
- Đảm bảo không mất thông tin quan trọng trong quá trình rút gọn


#### Kiểm soát độ chi tiết

**Lợi ích của việc theo dõi từng bước:**

- Biết được thông tin gì đang được lược bỏ
- Có thể điều chỉnh nếu thấy mất thông tin quan trọng
- Kiểm soát chất lượng tốt hơn


### Ứng dụng ngược chiều

**Chain of Density Prompting cũng hoạt động theo hướng ngược lại:**

- Nếu đầu ra quá ngắn, có thể yêu cầu tăng độ dài và thêm chi tiết
- Linh hoạt điều chỉnh theo cả hai hướng: ngắn hơn hoặc chi tiết hơn


### Ví dụ prompt thực tế

#### Prompt ban đầu:

```
Tóm tắt báo cáo này dưới dạng outline, chỉ tập trung vào những điểm thiết yếu nhất.
```


#### Prompt tinh chỉnh lần 1:

```
Cung cấp bản tóm tắt ngắn hơn, tập trung vào 2-3 xu hướng hàng đầu của báo cáo.
```


#### Prompt tinh chỉnh lần 2:

```
Cô đọng bản tóm tắt thành một câu duy nhất, làm nổi bật xu hướng chủ đạo nhất.
```


### Ghi chú thêm

**Khuyến nghị thực hành:**

- Thử nghiệm với những báo cáo chưa có thời gian đọc
- Khám phá tốc độ tạo ra bản tóm tắt hữu ích
- Kết hợp với kỹ thuật Long Context Window đã học trước đó

**Ưu điểm chính:**

- Kiểm soát được mức độ chi tiết
- Giảm thiểu rủi ro mất thông tin quan trọng
- Tạo ra nhiều phiên bản tóm tắt cho các mục đích khác nhau
- Có thể sử dụng cho nhiều loại nội dung khác nhau

**Liên kết:** [[Chain of Density Prompting]], [[Summarization]], [[Hallucination]], [[Iteration]], [[Prompt Refinement]], [[Long Context Window]], [[Elevator Pitch]], [[Generative AI]], [[Advanced Prompting]]

