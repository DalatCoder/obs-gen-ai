# Kỹ Thuật Prompting - Tổng Hợp

## 📝 Giới thiệu

File này tổng hợp các kỹ thuật prompting quan trọng được đề cập trong khóa học Google AI Essentials, giúp bạn nhanh chóng tham khảo và áp dụng.

## 🎯 Kỹ Thuật Cơ Bản

### 1. CLEAR Framework

**Chi tiết:** [[03 - 05 - Prompting best practices]]

- **C**oncise (Ngắn gọn): Viết prompt rõ ràng, tránh dài dòng
- **L**ogical (Logic): Sắp xếp thông tin theo trật tự hợp lý
- **E**xplicit (Rõ ràng): Nêu rõ yêu cầu, không để mơ hồ
- **A**daptive (Linh hoạt): Sẵn sàng điều chỉnh dựa trên kết quả
- **R**eflective (Phản hồi): Đánh giá và cải thiện prompt

### 2. Task-Context-References-Evaluate-Iterate

**Chi tiết:** [[03 - 05 - Prompting best practices]]

- **Task**: Xác định nhiệm vụ cụ thể
- **Context**: Cung cấp ngữ cảnh cần thiết
- **References**: Đưa ra ví dụ hoặc tham chiếu
- **Evaluate**: Đánh giá kết quả đầu ra
- **Iterate**: Lặp lại và cải thiện

---

## 🚀 Kỹ Thuật Nâng Cao

### 1. Few-Shot Prompting

**Chi tiết:** [[03 - 09 - Discover few-shot prompting]]

Cung cấp một vài ví dụ để hướng dẫn AI hiểu pattern mong muốn.

**Ví dụ:**

```
Classify the sentiment of these reviews:

Review: "Amazing product, love it!" → Positive
Review: "Terrible quality, broke immediately" → Negative
Review: "It's okay, nothing special" → Neutral
Review: "Outstanding service and fast delivery" → ?
```

### 2. Chain-of-Thought Prompting

**Chi tiết:** [[03 - 10 - Explore chain-of-thought prompting]]

Yêu cầu AI giải thích từng bước suy nghĩ.

**Ví dụ:**

```
Solve this step by step:
A store has 50 apples. They sell 30 apples in the morning
and 15 apples in the afternoon. How many apples are left?

Let me think through this step by step:
1. Starting apples: 50
2. Sold in morning: 30
3. Sold in afternoon: 15
4. Total sold: 30 + 15 = 45
5. Apples left: 50 - 45 = 5
```

### 3. Iterative Improvement

**Chi tiết:** [[03 - 08 - Improve AI output through iteration]]

Cải thiện prompt qua nhiều lần thử nghiệm:

1. Prompt ban đầu
2. Đánh giá kết quả
3. Xác định vấn đề
4. Điều chỉnh prompt
5. Lặp lại cho đến khi đạt kết quả mong muốn

---

## 💡 Best Practices

### Viết Prompt Rõ Ràng

**Chi tiết:** [[03 - 04 - Write clear and specific prompts]]

- ✅ Sử dụng ngôn ngữ cụ thể, tránh mơ hồ
- ✅ Đưa ra context đầy đủ
- ✅ Specify format đầu ra mong muốn
- ❌ Tránh prompt quá chung chung
- ❌ Không giả định AI hiểu ngữ cảnh implicit

### Prompt Engineering Framework

**Chi tiết:** [[03 - 01 - Module 3 introduction - Discover the art of prompting]]

```
1. Define Goal (Xác định mục tiêu)
2. Provide Context (Cung cấp ngữ cảnh)
3. Set Constraints (Đặt giới hạn)
4. Give Examples (Đưa ví dụ)
5. Specify Format (Chỉ định định dạng)
6. Iterate & Improve (Lặp lại & cải thiện)
```

---

## ⚖️ Sử Dụng Có Trách Nhiệm

### Nhận Biết Bias

**Chi tiết:** [[04 - 02 - Understand bias in AI]]

- Kiểm tra bias trong prompt
- Đánh giá bias trong output
- Sử dụng diverse perspectives
- Test với nhiều scenarios khác nhau

### Human-in-the-Loop

**Chi tiết:** [[02 - 10 - Leverage the human-in-the-loop approach to AI]]

- Luôn review AI output
- Fact-check thông tin quan trọng
- Không hoàn toàn dựa vào AI
- Kết hợp judgment của con người

---

## 🛠️ Ứng Dụng Thực Tế

### Với Gemini

**Chi tiết:** [[02 - 07 - Work with Gemini]]

- Viết cover letter
- Chuẩn bị phỏng vấn
- Brainstorm ý tưởng
- Tạo training activities

### Trong Google Workspace

**Chi tiết:** [[02 - 13 - Use Gemini in Google Docs, Slides, Sheets, Meet, and Gmail]]

- Google Docs: Viết và edit content
- Google Slides: Tạo presentations
- Google Sheets: Phân tích dữ liệu
- Gmail: Compose emails
- Google Meet: Meeting summaries

---

## 📊 Evaluation Checklist

Khi đánh giá AI output, hãy kiểm tra:

- [ ] **Accuracy**: Thông tin có chính xác không?
- [ ] **Relevance**: Có liên quan đến yêu cầu không?
- [ ] **Completeness**: Có đầy đủ thông tin không?
- [ ] **Bias**: Có bias hoặc thiên kiến không?
- [ ] **Safety**: Có an toàn và phù hợp không?
- [ ] **Format**: Định dạng có đúng yêu cầu không?

---

## 🔗 Liên Kết Quan Trọng

### Cơ Bản

- [[03 - 02 - Understand large language models]] - Hiểu về LLM
- [[03 - 04 - Write clear and specific prompts]] - Viết prompt cơ bản

### Nâng Cao

- [[03 - 09 - Discover few-shot prompting]] - Few-shot technique
- [[03 - 10 - Explore chain-of-thought prompting]] - Chain-of-thought

### Thực Hành

- [[02 - 07 - Work with Gemini]] - Thực hành với Gemini
- [[03 - 11 - Improve prompts through exploration]] - Cải thiện prompt

### Responsible AI

- [[04 - 02 - Understand bias in AI]] - Hiểu về bias
- [[02 - 10 - Leverage the human-in-the-loop approach to AI]] - Human-in-the-loop

---

**🏠 Quay về:** [[01 - 01 - Introduction to Google AI Essentials]]  
**📋 Mục lục:** [[00 - Index - Mục Lục Tổng Hợp]]
