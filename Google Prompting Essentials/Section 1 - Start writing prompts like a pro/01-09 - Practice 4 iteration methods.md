## Bốn phương pháp lặp lại để tối ưu prompt

### Nguyên lý ABI (Always Be Iterating)

Thay vì bỏ toàn bộ công việc khi prompt không cho kết quả mong muốn, hãy áp dụng nguyên lý **Always Be Iterating (ABI)** - Luôn Lặp Lại để điều chỉnh đầu ra thành thứ hữu ích hơn.

### 1. Quay lại khung prompting và tăng tính cụ thể

Kiểm tra lại xem bạn đã cung cấp đủ thông tin cụ thể trong **task** (nhiệm vụ), **context** (bối cảnh) và **references** (tài liệu tham khảo) chưa.

**Ví dụ so sánh:**

❌ **Prompt mơ hồ:**

```
Cho tôi 5 ý tưởng bài blog
```

✅ **Prompt cụ thể:**

```
Bạn là chuyên gia về dinh dưỡng thể thao. Cung cấp 5 tiêu đề bài blog tóm tắt những xu hướng lớn nhất đang diễn ra trong ngành cho đối tượng là các nhà vật lý trị liệu làm việc với cầu thủ bóng rổ chuyên nghiệp.
```


### 2. Chia nhỏ prompt thành câu ngắn hơn

Thay vì đưa ra một prompt dài phức tạp, hãy chia thành các nhiệm vụ nhỏ và thực hiện từng bước.

**Ví dụ prompt dài:**

```
Tóm tắt các điểm dữ liệu và thông tin chính trong báo cáo này. Sau đó tạo biểu đồ trực quan từ dữ liệu và rút gọn thông tin chính thành dạng gạch đầu dòng.
```

**Chia thành các bước nhỏ:**

1. **Bước 1:** Tóm tắt các điểm dữ liệu và thông tin chính trong báo cáo này
2. **Bước 2:** Tạo biểu đồ trực quan với dữ liệu bạn đã tóm tắt
3. **Bước 3:** Rút gọn thông tin chính bạn đã tóm tắt thành dạng gạch đầu dòng

**Lợi ích:** Câu ngắn giúp công cụ AI xử lý từng nhiệm vụ nhỏ thay vì phải nhận diện mối quan hệ giữa tất cả nhiệm vụ cùng lúc.

### 3. Thay đổi cách diễn đạt hoặc dùng nhiệm vụ tương tự

Sử dụng **analogous task** (nhiệm vụ tương tự) - nhiệm vụ rất giống với điều bạn muốn hoàn thành nhưng khác biệt đủ để kích hoạt phản hồi mới.

**Ví dụ chuyển đổi:**

❌ **Prompt gốc:**

```
Viết kế hoạch marketing cho sản phẩm này
```

✅ **Prompt tương tự:**

```
Viết một câu chuyện về cách sản phẩm này phù hợp với cuộc sống của nhóm khách hàng mục tiêu
```

**Hiệu quả:** Chuyển từ "viết kế hoạch marketing" sang "viết câu chuyện" khiến AI tiếp cận nhiệm vụ theo cách khác, có thể dẫn đến kết quả hữu ích hơn.

### 4. Thêm ràng buộc (constraints) để tập trung đầu ra

Ràng buộc giúp công cụ AI thu hẹp phạm vi đầu ra và tạo ra kết quả độc đáo hoặc hữu ích hơn.

**Ví dụ thực tiễn:**

**Tình huống:** Tạo playlist cho chuyến đi đường dài

❌ **Prompt chung chung:**

```
Tạo playlist nhạc cho chuyến đi. Tôi thích thể loại rock.
```

✅ **Prompt có ràng buộc:**

```
Tạo playlist nhạc cho chuyến đi với các ràng buộc:
- Chỉ nghệ sĩ từ khu vực Bắc Âu
- Nghệ sĩ đã phát hành nhạc trong 5 năm qua
- Thể loại rock
```

**Lợi ích ràng buộc:**

- Tránh kết quả nhàm chán, quen thuộc
- Tạo ra đầu ra bất ngờ và độc đáo
- Giúp AI tập trung vào yêu cầu cụ thể


### Nguyên tắc tổng quát

**Quy tắc vàng:** Càng đánh giá và lặp lại tốt, đầu ra càng chất lượng cao.

**Quy trình thực hiện:**

1. Kiểm tra tính cụ thể của prompt
2. Chia nhỏ nhiệm vụ phức tạp
3. Thử cách diễn đạt khác
4. Thêm ràng buộc phù hợp
5. Lặp lại cho đến khi đạt kết quả mong muốn

**Liên kết:** [[TCREI Framework]], [[Prompt Engineering]], [[Task Decomposition]], [[Constraint Design]], [[Analogous Tasks]]

