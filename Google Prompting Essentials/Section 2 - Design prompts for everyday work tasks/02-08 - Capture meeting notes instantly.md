## Sử dụng Gemini trong Google Docs để cải thiện văn bản và tạo biên bản họp

### Cải thiện nội dung văn bản hiện có

**Tình huống thường gặp:**

- Khi chỉnh sửa trong Google Docs, nhận ra văn bản có thể được cải thiện nhưng không biết cách tiếp cận
- Thay vì ngồi nhìn màn hình trống rỗng, có thể sử dụng Gemini để đưa ra gợi ý cải thiện

**Yêu cầu:** Cần có tài khoản Google để đăng nhập vào Docs.

#### Ví dụ thực hành: Cải thiện chính sách hoàn trả

**Bối cảnh:**
Nhận phản hồi từ khách hàng rằng chính sách hoàn trả của công ty quá dài và khó hiểu.

**Quy trình thực hiện:**

1. Dán chính sách hoàn trả hiện tại vào tài liệu Google Docs
2. Sử dụng prompt với Gemini

**Prompt mẫu:**

```
Tóm tắt nội dung này để viết một chính sách hoàn trả sản phẩm rõ ràng và súc tích, đồng thời phác thảo năm bước cho khách hàng thực hiện theo thứ tự tuần tự.
```

**Kết quả đạt được:**

- Chính sách hoàn trả rõ ràng để tham khảo khi hỗ trợ khách hàng
- Danh sách các bước cụ thể để khách hàng bắt đầu quy trình hoàn trả


### Tạo biên bản họp từ transcript

**Vấn đề thường gặp:**

- Những ngày đầy các cuộc họp với nhiều người và nhiều hành động cần thực hiện
- Khó theo dõi ai nói gì và bạn có trách nhiệm làm gì
- Cần có transcript để ghi nhớ nội dung họp

**Giải pháp:**

- Tạo transcript trực tiếp trong Google Meet
- Sử dụng Gemini in Docs để tổ chức thông tin thành biên bản họp có cấu trúc


#### Phương pháp 1: Phân chia theo người nói

**Prompt framework (Khung viết prompt):**

**Nhiệm vụ (Task):**

```
Tạo biên bản họp cho cuộc họp này.
```

**Định dạng (Format):**

```
Phân chia biên bản họp theo người nói, và tạo danh sách gạch đầu dòng tóm tắt các điểm chính do người nói đó đưa ra. Nếu có thể, hãy làm nổi bật các hành động cần thực hiện cho mỗi người nói.
```


#### Phương pháp 2: Phân chia theo điểm chính (Cải tiến)

**Vấn đề của phương pháp 1:** Biên bản họp có thể hữu ích hơn nếu được định dạng rõ ràng hơn với vai trò và trách nhiệm được xác định cụ thể.

**Prompt cải tiến:**

**Nhiệm vụ (Task) - giữ nguyên:**

```
Tạo biên bản họp cho cuộc họp này.
```

**Định dạng mới (Format) - cụ thể hơn:**

```
Tạo các phần dựa trên các điểm chính được trích xuất từ biên bản. Gán mỗi điểm chính cho người nói, sau đó chỉ định các hành động cần thực hiện cho người nói phù hợp nhất để hoàn thành chúng.
```

**Kết quả đạt được:**

- Các hành động cần thực hiện được hiển thị rõ ràng
- Có những điểm quan trọng nhất từ mỗi người tham dự
- Dễ dàng phối hợp với đồng nghiệp về dự án
- Chia sẻ cập nhật để thông báo cho các bên liên quan
- Giúp đồng đội hoàn thành trách nhiệm của họ
- Theo dõi tiến độ của các deliverable (sản phẩm bàn giao)


### Nguyên tắc quan trọng

**Sử dụng prompt framework:**

- **Thoughtfully create really excellent inputs** - Tạo đầu vào xuất sắc một cách chu đáo
- Xác định rõ nhiệm vụ (Task) và định dạng (Format) mong muốn
- Lặp lại và cải tiến prompt để đạt kết quả tốt hơn

**Lợi ích của việc lặp lại prompt (Iterate):**

- Có thể điều chỉnh định dạng và yêu cầu cụ thể hơn
- Đạt được kết quả phù hợp hơn với nhu cầu thực tế
- Cải thiện chất lượng đầu ra liên tục

**Liên kết:** [[Gemini]], [[Google Docs]], [[Google Meet]], [[Prompt Framework]], [[Meeting Minutes]], [[Task Context]], [[Format]], [[Transcript]], [[Iteration]], [[Action Items]], [[Deliverables]]

