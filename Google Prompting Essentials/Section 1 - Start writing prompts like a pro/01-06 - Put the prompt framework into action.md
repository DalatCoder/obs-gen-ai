## Áp dụng Framework Prompting trong thực tế

### Demo với Gemini: Brainstorming dòng giày thể thao

**Mục tiêu:** Sử dụng Gemini để **brainstorm ý tưởng** cho dòng giày thể thao hiệu suất cao mới

**Framework áp dụng:** **T.C.R.E.I** - Thoughtfully Create Really Excellent Inputs

### Bước 1: Task (Nhiệm vụ) đầu tiên

**Prompt ban đầu:**

```
Generate five ideas for a new high-performance sneaker line.
```

**Vấn đề:**

- Chỉ có **task**, thiếu các thành phần khác trong framework
- Kết quả **quá broad** (rộng) và không hữu ích lắm
- Gemini tạo ra 5 ý tưởng với tên và mô tả độc đáo nhưng chưa tối ưu

**Kết quả:** Đây là khởi đầu không tệ, nhưng có thể làm tốt hơn

### Bước 2: Thêm Format và chi tiết Task

**Prompt cải tiến:**

```
List the concepts and materials for each sneaker in an outline.
```

**Cải thiện:**

- Thêm **format preference** (định dạng outline)
- Task cụ thể hơn (yêu cầu concepts và materials)

**Kết quả:**

- Nhận được **ý tưởng độc đáo** cho dòng giày
- Bao gồm **materials** (vật liệu) cho từng đôi giày
- Xuất hiện theo **định dạng ưa thích**


### Bước 3: Thêm Context (Bối cảnh)

**Context bổ sung:**

```
The sneakers should be made for athletes doing cross-training activities.
```

**Kết quả với context:**

- Gemini tạo ra **5 ý tưởng giày mới** phù hợp với mục tiêu cụ thể
- Thiết kế dành cho **cross-training activities** (hoạt động tập luyện đa năng)

**Nguyên tắc quan trọng:**

- **Tailored outputs** (đầu ra được tùy chỉnh) cần **chi tiết và context** nhiều hơn
- **Success is all about the details** (Thành công là về chi tiết)


### Bước 4: References (Tham chiếu) - Few-shot Prompting

#### Khái niệm Few-shot Prompting

**Few-shot prompting:** Cung cấp **multiple references** (nhiều tham chiếu/ví dụ)

**Các loại Shot Prompting:**

- **Zero-shot:** Không cung cấp references nào
- **Single-shot:** Cung cấp 1 reference
- **Few-shot:** Cung cấp nhiều references (2-5 là sweet spot)

**Lưu ý:**

- **Quá ít references:** Không đủ context
- **Quá nhiều references:** Có thể **skew results** (làm lệch kết quả) và hạn chế creativity


#### Áp dụng References cho dự án sneaker

**References được thêm:**

- Mô tả giày từ **budget line** (dòng giá rẻ)
- Giày có **adaptive sole** (đế thích ứng) mới

**Prompt với references:**

```
Keep the five ideas generated, but refine them using these two examples as references.
```

**Kết quả:**

- Nhiều lựa chọn chất lượng cho task
- Có ý tưởng **innovative** như giày điều chỉnh nhiệt độ (temperature regulation)


### Bước 5: Evaluate và Iterate

#### Quá trình liên tục

**Thực tế:** Chúng ta đã **evaluating và iterating** suốt quá trình demo:

1. **Lần 1:** Đánh giá prompt đầu tiên → Iterate bằng cách thêm context
2. **Lần 2:** Đánh giá output → Iterate bằng cách thêm references
3. **Tiếp tục:** Có thể thêm chi tiết hoặc điều chỉnh phong cách để thay đổi outputs

#### Nguyên tắc "A.B.I"

**Always Be Iterating** - Luôn luôn lặp lại/cải tiến

### Mẹo thực hành Framework

#### Chiến lược tiệp cận

- **Bắt đầu đơn giản** → Từ từ thêm complexity
- **Iterate as you go** (lặp lại khi tiến hành)
- Nếu outputs **mất chất lượng** → quay lại làm prompts **đơn giản hơn**


#### Khi gặp khó khăn

**Nhớ nguyên tắc:** "Thoughtfully Create Really Excellent Inputs"

- Tập trung vào chất lượng input
- Học **what works và what doesn't** là part of the journey


### Bài học từ Demo

#### Sự cải thiện qua từng bước

1. **Task only:** Kết quả broad, generic
2. **Task + Format:** Cụ thể hơn, có cấu trúc
3. **+ Context:** Tailored cho mục đích cụ thể
4. **+ References:** Creative và đa dạng hơn
5. **+ Evaluation/Iteration:** Tinh chỉnh liên tục

#### Takeaway quan trọng

- **Details matter** - Chi tiết quan trọng
- **Iterative process** - Quá trình lặp lại liên tục
- **Quality inputs = Quality outputs**
- Framework là **hướng dẫn linh hoạt**, không phải quy tắc cứng nhắc


### Ghi chú thêm

Demo này minh họa tính **thực tế và hiệu quả** của framework T.C.R.E.I. Việc áp dụng từng bước một cách có hệ thống giúp đạt được kết quả **ngày càng tốt hơn** từ gen AI tools.

**Liên kết:** [[Prompting Framework]], [[Gemini]], [[Few-shot Prompting]], [[Context]], [[References]], [[Task]], [[Format]], [[Brainstorming]], [[Iterate]], [[Cross-training]]

