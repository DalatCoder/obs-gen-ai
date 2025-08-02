## Kỹ thuật Prompting nâng cao - Từ Chuyên gia Google

### Giới thiệu từ Rachna - Google Software Engineer

**Rachna** là Software Engineer tại Google, làm việc trong team **Central Knowledge Management** (Quản lý Kiến thức Tập trung).

**Nhiệm vụ của team:**

- **Đảm bảo developers** có quyền truy cập vào tất cả thông tin cần thiết
- **Hỗ trợ knowledge sharing** trong tổ chức


### Tầm quan trọng của Prompting

**Định nghĩa Prompting:**

- **Figuring out what text to input** (Tìm ra text input nào) để nhận được response mong muốn
- **Một trong những điều quan trọng nhất** cần học về AI

**Nguyên tắc cơ bản:**

- **Prompting = quá trình thử nghiệm** để tìm ra cách giao tiếp hiệu quả với AI
- **Kỹ năng then chốt** để tận dụng tối đa khả năng của LLM


### Rapid Iteration - Lặp lại Nhanh

**Phương pháp tìm effective prompts:**

- **Iterate rapidly** (Lặp lại nhanh chóng) trên các prompts
- **Try a wide variety** (Thử nhiều loại khác nhau) của different prompts

**Ví dụ điều chỉnh dựa trên kết quả:**

- **Nếu không đủ funny** → Lần sau prompt LLM "make it more funny"
- **Nếu quá vague** → Sử dụng prompt specifically yêu cầu AI "not to be vague"

**Nguyên tắc:** **Trying out a lot of different things** thường sẽ give you good results.

### Điều chỉnh Context cho Creativity vs Specificity

**Relationship giữa Context và Output:**

- **Amount of context** quyết định mức độ creative hoặc specific của LLM


#### Creative Response Strategy

- **Muốn creative response** → Sử dụng **very short prompt**
- **Ít context** = Nhiều freedom cho AI sáng tạo


#### Specific Response Strategy

- **Muốn very specific output** → **Put in a lot of examples**
- **LLM sẽ conform more** to your examples
- **Nhiều context** = Output sát với yêu cầu cụ thể

**Key insight:** **Context amount = Control level** over AI creativity.

### Chain-of-thought Prompting nâng cao

**Định nghĩa:** Yêu cầu model **reason out its own response** (lý luận ra phản hồi của chính nó).

**Ứng dụng thực tế - Mathematical equations:**

```
1. Ask model to break it down into steps
2. Do the first step  
3. Then the second step
4. And so on...
```

**Lợi ích:**

- **Getting LLM to do multiple steps** có thể make it **much more accurate**
- **Improved reasoning** thông qua structured approach

**Nguyên tắc:** **Step-by-step reasoning** = **Higher accuracy**.

### Self-Evaluation Technique - Kỹ thuật Tự đánh giá

**Innovative approach:** Asking the model to **react to its own responses**.

**Quy trình thực tế:**

1. **Ask model for a response**
2. **Follow-up question:** "Is this response vague?"
3. **If it answers yes** → **Throw that response out**
4. **Let AI do some of my work for me**

**Ví dụ conversation flow:**

```
Prompt 1: [Initial request]
AI Response: [First response]
Prompt 2: "Is this response vague?"
AI: "Yes"
Action: Discard response, try again
```

**Lợi ích:**

- **AI tự quality-check** output của mình
- **Reduce manual evaluation** effort
- **Leverage AI's self-awareness** capabilities


### Philosophy về Experimentation

**Mindset quan trọng:**

- **The more you experiment** = **The better results**
- **The more creative you are** = **More effective prompting**

**Approach:**

- **Không ngại thử nghiệm** với different approaches
- **Creativity in prompting** dẫn đến breakthrough results
- **Experimentation = Key to mastery**


### Keeping up với AI Development

**Thách thức thực tế:**

- **Keeping up với AI** giống như "**running on a treadmill**"
- **Always getting faster and faster** (Luôn tăng tốc)
- **So many new things changing** (Rất nhiều thứ mới thay đổi)

**Positive perspective:**

- **That's also what makes it really fun** (Đó cũng là điều làm cho nó thú vị)
- **Continuous learning** = **Exciting journey**

**Ghi chú quan trọng:**

- **Rapid evolution** of AI field requires **continuous adaptation**
- **Challenge = Opportunity** to grow and learn


### Ghi chú thêm

**Key takeaways từ Google expert:**

- **Rapid iteration** là foundation của effective prompting
- **Context control** = **Creativity control**
- **Chain-of-thought** improves accuracy significantly
- **Self-evaluation** leverages AI's capabilities
- **Experimentation mindset** essential cho success

**Practical advice:**

- **Try wide variety** of prompt approaches
- **Don't be afraid** to be creative
- **Use AI to evaluate AI** output
- **Embrace continuous learning** trong rapidly changing field

**Liên kết:** [[Prompting]], [[LLM]], [[Chain-of-thought Prompting]], [[Context]], [[Rapid Iteration]], [[Self-Evaluation]], [[Creativity]], [[Specificity]], [[Google AI]], [[Central Knowledge Management]]

