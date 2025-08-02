## Sử dụng Ví dụ trong Prompting - Kỹ thuật Shot

### Tầm quan trọng của Ví dụ trong Prompting

**Nguyên lý cơ bản:**

- **Xây dựng dựa trên examples trước đó** là cách hiệu quả để tạo ra something mới
- **Ví dụ:** Sử dụng report được đón nhận tốt làm reference khi viết report tương tự, hoặc dùng website hấp dẫn làm model khi thiết kế website riêng

**Ứng dụng cho LLM:**

- **Bao gồm examples trong prompt** giúp LLM phản hồi tốt hơn cho request
- **Chiến lược đặc biệt hiệu quả** để đạt được desired output mong muốn


### Thuật ngữ "Shot" trong Prompt Engineering

**Định nghĩa:**

- Từ "**shot**" thường được sử dụng như **synonym** (từ đồng nghĩa) với từ "**example**"
- **Các kỹ thuật prompting** được đặt tên dựa trên số lượng examples được cung cấp cho LLM


### Các Loại Prompting Techniques

#### 1. Zero-shot Prompting

**Đặc điểm:**

- **Không cung cấp examples** trong prompt
- **Model dựa vào training data** và task description trong prompt để thực hiện
- **Hiệu quả nhất** cho các phản hồi **simple và direct**
- **Có thể không hiệu quả** cho tasks yêu cầu LLM phản hồi theo cách **specific, nuanced**


#### 2. One-shot Prompting

**Đặc điểm:**

- **Cung cấp một example** trong prompt


#### 3. Few-shot Prompting

**Đặc điểm:**

- **Cung cấp hai hoặc nhiều examples** trong prompt
- **Cải thiện hiệu suất** của LLM bằng cách cung cấp **additional context và examples**
- **Examples giúp làm rõ:**
    - **Desired format** (định dạng mong muốn)
    - **Phrasing** (cách diễn đạt)
    - **General pattern** (mẫu chung)


### Ví dụ Thực tế: Viết Product Description

**Bối cảnh:**

- **Công việc:** Làm việc cho online retailer
- **Nhiệm vụ:** Viết product description cho skateboard mới
- **Yêu cầu:** Follow style và format tương tự như descriptions hiện có (bicycle và roller blades)


#### Cấu trúc Prompt Few-shot

**Hướng dẫn chung:**

```
Write a one-sentence description of a product. It should contain two adjectives that describe the product.
```

**Examples được cung cấp:**

- **Bicycle:** "Whether you're exploring city streets or forest paths, our sleek and durable bicycle has it all."
- **Rollerblades:** "Roll into summer in style with our smooth and stylish rollerblades."

**Target output:**

- **Skateboard:** [Để trống cho LLM hoàn thành]


#### Phân tích Examples

**Pattern trong examples:**

- **Bicycle:** 2 tính từ - "**sleek**" và "**durable**"
- **Rollerblades:** 2 tính từ - "**smooth**" và "**stylish**"
- **Format:** Mỗi description dài **một câu** và chứa **hai adjectives**


#### Kết quả

**Output từ LLM:**

- Cung cấp product description cho skateboard **đáp ứng criteria** yêu cầu
- **Cùng writing style và format** như examples trong prompt
- **Thành công** với chỉ hai examples


### Số lượng Examples Tối ưu

**Thực tế về số lượng examples:**

- **Không có quy tắc chắc chắn** cho optimal number của examples trong prompt
- **Một số LLMs** có thể reproduce patterns chỉ với **few examples**
- **LLMs khác** cần **nhiều examples hơn**

**Cảnh báo về quá nhiều examples:**

- **Responses có thể trở nên less flexible và creative**
- **LLM có thể reproduce examples quá closely** (sát với nguyên bản)

**Gợi ý:**

- **Experiment** với số lượng examples để có **best results** cho specific task của bạn


### Lợi ích của Few-shot Prompting

**Ứng dụng đa dạng:**

- **Generate content** theo particular style
- **Cải thiện chất lượng output** thông qua additional context
- **Hướng dẫn LLM** tạo ra **more useful responses**

**Hiệu quả đặc biệt:**

- **Tasks yêu cầu format cụ thể**
- **Content creation** với style nhất quán
- **Pattern recognition** và reproduction


### Kết luận

**Few-shot prompting** là **effective strategy** giúp:

- **Guide LLM** tạo ra more useful responses
- **Cải thiện quality output** thông qua examples
- **Đạt được desired format** và style

**Nguyên tắc áp dụng:**

- **Experiment** với số lượng examples
- **Chọn examples** representative cho desired output
- **Cân bằng** giữa guidance và creativity

**Liên kết:** [[Prompt Engineering]], [[Few-shot Prompting]], [[Zero-shot Prompting]], [[One-shot Prompting]], [[Examples]], [[LLM]], [[Content Creation]], [[Product Description]], [[Gemini]]

