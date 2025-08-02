## Quy trình Lặp lại trong Prompt Engineering (Iterative Process)

### Khái niệm Quy trình Lặp lại

**Quy trình lặp lại (Iterative Process)** là phương pháp mà bạn:

- **Tạo phiên bản đầu tiên**
- **Đánh giá kết quả**
- **Cải thiện cho phiên bản tiếp theo**
- **Lặp lại các bước** cho đến khi đạt được mục tiêu mong muốn

**Ví dụ trong công việc:**

- Phát triển proposal, report hoặc document để chia sẻ với đồng nghiệp
- Tạo nhiều bản draft và cải thiện từng bản
- Tiếp tục đến khi hài lòng với kết quả

**Nguyên tắc quan trọng:** Phương pháp lặp lại thường là cách hiệu quả nhất để giải quyết vấn đề hoặc phát triển sản phẩm.

### Ứng dụng trong Prompt Engineering

**Thực tế về Prompt Engineering:**

- **Thường cần nhiều lần thử** trước khi có output tối ưu
- **Hầu hết không đạt kết quả tốt nhất ở lần đầu**
- **Không nên nản lòng** nếu thử và không hiệu quả

**Quy trình cải thiện:**

1. **Đánh giá cẩn thận output** để xác định lý do không nhận được phản hồi mong muốn
2. **Sửa đổi prompt** để cố gắng có kết quả tốt hơn
3. **Lặp lại quá trình** cho đến khi đạt mục tiêu

### Lý do không nhận được Output hữu ích

#### 1. Khác biệt giữa các Large Language Models

- **Mỗi LLM có training data và programming techniques riêng**
- **Background knowledge khác nhau** về các lĩnh vực cụ thể
- **Models khác nhau phản hồi khác nhau** với prompt tương tự
- **Có thể không cung cấp phản hồi phù hợp** cho một số prompts

**Giải pháp:** Áp dụng iterative approach với LLM bạn đang sử dụng sẽ cho kết quả tốt nhất.

#### 2. Hạn chế của LLM

**Các vấn đề có thể gặp phải:**

- **Inaccurate** (không chính xác)
- **Biased** (thiên kiến)
- **Insufficient** (không đủ thông tin)
- **Irrelevant** (không liên quan)
- **Inconsistent** (không nhất quán)


### Cách Đánh giá Output

**5 câu hỏi quan trọng cần tự hỏi:**

1. **Output có chính xác không?** (Is the output accurate?)
2. **Output có thiên kiến không?** (Is the output unbiased?)
3. **Output có đủ thông tin không?** (Does the output include sufficient information?)
4. **Output có liên quan đến project/task không?** (Is the output relevant to my project or task?)
5. **Output có nhất quán khi sử dụng cùng prompt nhiều lần không?** (Is the output consistent if I use the same prompt multiple times?)

### Strategies cải thiện Prompt

**Khi phát hiện vấn đề trong output:**

#### 1. Thêm Context thiếu

- **Kiểm tra context** có đầy đủ trong prompt không
- **Bổ sung thông tin** cần thiết nếu thiếu


#### 2. Điều chỉnh Choice of Words

- **Lựa chọn từ ngữ** có thể ảnh hưởng đáng kể đến output của LLM
- **Sử dụng từ ngữ hoặc cách diễn đạt khác** thường cho phản hồi khác nhau
- **Thử nghiệm với phrasings khác nhau** để có output hữu ích nhất


### Ví dụ Thực tế: Tìm kiếm Colleges với Animation Programs

**Bối cảnh:**

- **Vai trò:** Human Resources Coordinator cho công ty video production
- **Mục tiêu:** Phát triển internship program cho students quan tâm đến animation và motion graphics design
- **Địa điểm:** Pennsylvania, United States
- **Yêu cầu:** Partner với local colleges để cung cấp internship opportunities

**Nhiệm vụ cụ thể:** Tạo danh sách colleges ở Pennsylvania có animation programs với format có tổ chức để team dễ review.

#### Lần thử đầu tiên

```
Prompt: "Help me find colleges with animation programs in Pennsylvania."
```

**Kết quả:**

- Output liệt kê colleges ở Pennsylvania có animation programs
- Bao gồm thông tin liên quan đến programs
- **Vấn đề:** Không có cấu trúc để team có thể tham khảo nhanh khi liên hệ colleges


#### Lần cải thiện thứ nhất

```
Prompt: "Show these options as a table."
```

**Kết quả cải thiện:**

- Output hiển thị **table format**
- Cung cấp thông tin hữu ích về **location** của mỗi college
- Bao gồm **loại degree cụ thể** mà college cung cấp
- **Format có tổ chức** dễ cho team theo dõi


#### Lần cải thiện thứ hai

```
Prompt: "Can you add a column showing whether they're public or private?"
```

**Lý do cần thiết:** Company muốn offer internships cho students từ cả public và private colleges.

**Kết quả cuối cùng:**

- Table bao gồm **column mới** chỉ ra college là private hay public
- **Thông tin đầy đủ** cho team ra quyết định
- **Có thể sử dụng Export to Sheets feature** để chia sẻ với team


### Ghi chú Quan trọng

**Về Previous Prompts:**

- **Prompts trước đó trong cùng conversation** có thể ảnh hưởng đến output của prompt mới nhất
- **Nếu nhận thấy điều này xảy ra** → nên bắt đầu conversation mới

**Nguyên tắc chung:**

- **Iteration là key part** của prompt engineering
- **Iterative approach** giúp leverage LLM để cung cấp output hữu ích nhất cho nhu cầu của bạn
- **Áp dụng cùng approach** cho các tasks tiếp theo

**Liên kết:** [[Prompt Engineering]], [[Iterative Process]], [[LLM]], [[Output Evaluation]], [[Context]], [[Gemini]], [[Table Format]], [[Human Resources]], [[Animation Programs]]

