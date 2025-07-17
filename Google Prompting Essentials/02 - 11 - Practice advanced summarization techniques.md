# Kỹ thuật [[Glossary - Thuật ngữ Gen AI#Prompting|Prompting]] Nâng cao: Chain of Density Prompting

> 🧭 **Navigation**: [[02 - 10 - AI IRL - Reclaim your time with the help of AI|← Trước]] | [[MOC - Google Prompting Essentials|📚 Mục lục]] | [[02 - 12 - Summarization best practices|Tiếp theo →]]

---

## Vấn đề với Tóm tắt Quá Rộng

Khi yêu cầu công cụ trí tuệ nhân tạo tạo sinh (Gen AI) cung cấp tóm tắt, đôi khi **đầu ra ban đầu quá rộng**. Bạn cần thêm chi tiết để làm cho nó thực sự hữu ích.

## Giới thiệu Chain of Density Prompting

## Định nghĩa và Khái niệm

**Chain of density prompting** là kỹ thuật giúp bạn có được các bản tóm tắt ngày càng súc tích hơn và kết thúc với một chuỗi các đầu ra được tinh chỉnh.

## Ví dụ Minh họa: Elevator Pitch

Hãy tưởng tượng bạn đang làm việc trên **elevator pitch** hoàn hảo cho công ty của mình:

1. **Bản thảo đầu tiên:** Quá dài và bao gồm quá nhiều chi tiết
2. **Quy trình tinh chỉnh:** Khi bạn tinh chỉnh, nó trở nên ngắn hơn và trực tiếp hơn
3. **Giữ nguyên điểm quan trọng:** Không mất đi những điểm quan trọng cần truyền đạt
4. **Kết quả cuối cùng:** Elevator pitch hoàn hảo - **nhanh, trực tiếp và hiệu quả**

## Quy trình Thực hiện Chain of Density Prompting

## Bước 1: Tóm tắt Ngắn hơn với Xu hướng Chính

Dựa trên prompt tóm tắt report 44 trang ở bài trước đó.

**Prompt:**

text

`Provide a shorter summary, focusing on the report's top two to three trends`

_(Cung cấp tóm tắt ngắn hơn, tập trung vào hai đến ba xu hướng hàng đầu của báo cáo)_

**Kết quả:** Nhiệm vụ hoàn thành, nhưng có thể bạn muốn nó ngắn hơn nữa.

## Bước 2: Cụ thể hóa và Rút gọn hơn

**Prompt cải tiến:**

text

`Condense the summary into a single sentence, highlighting the most dominant trend`

_(Cô đọng tóm tắt thành một câu duy nhất, làm nổi bật xu hướng chiếm ưu thế nhất)_

**Đặc điểm của prompt này:**

- **Cụ thể hơn** với đầu ra mong muốn
- **Không chỉ tóm tắt đơn giản** mà còn **nhắm mục tiêu** vào nhu cầu cụ thể
- **Yêu cầu một câu duy nhất** với ngữ cảnh cụ thể

## Bước 3: Lặp lại Quy trình

**Nguyên tắc:**

- Tiếp tục yêu cầu tinh chỉnh thêm
- **Trực tiếp và cụ thể** về đầu ra mong muốn
- Lặp lại quá trình này cho đến khi tạo ra **đầu ra hữu ích và hỗ trợ nhất** cho nhiệm vụ

## Phương pháp Tối ưu hóa

## Prompt Tổng hợp

Bạn có thể **vượt qua các bước lặp lại bổ sung** bằng cách yêu cầu công cụ trí tuệ nhân tạo tạo sinh (Gen AI) cung cấp **nhiều lần lặp ngắn dần** trong prompt ban đầu.

## Lý do Không Đi Thẳng đến Kết quả Ngắn Nhất

## 1. Kiểm tra Hallucinations (Ảo giác)

**Lợi ích của iteration:**

- Giúp kiểm tra **hallucinations** (hiện tượng AI tạo ra thông tin sai lệch)
- Từ thông tin **cực kỳ chi tiết** đến đầu ra **trực tiếp và đúng trọng tâm**

## 2. Giữ Kiểm soát Thông tin

**Tầm quan trọng:**

- Giúp chúng ta **được thông báo** về thông tin nào đang bị loại bỏ
- Theo dõi quá trình **đầu ra ngắn dần**

## Ứng dụng Ngược lại

## Từ Ngắn sang Dài

**Chain of density prompting** cũng hoạt động theo **hướng ngược lại**:

- Nếu đầu ra **quá ngắn**
- Chúng ta có thể prompt để **tăng độ dài** và thêm chi tiết

## Khuyến khích Thực hành

## Áp dụng Kỹ thuật

**Gợi ý thực hành:**

- Nghĩ về báo cáo mà bạn chưa có thời gian để đọc
- Thử các kỹ thuật prompting này
- Khám phá mức độ **nhanh chóng** bạn có thể tạo ra **tóm tắt hữu ích**

## Lợi ích Tổng thể

## Ưu điểm của Chain of Density Prompting

- **Kiểm soát độ chi tiết:** Từ tổng quan đến cụ thể
- **Tránh thông tin sai lệch:** Qua quá trình iteration
- **Tùy chỉnh linh hoạt:** Có thể điều chỉnh theo cả hai hướng
- **Kết quả tối ưu:** Đầu ra phù hợp với nhu cầu cụ thể

## Ứng dụng Thực tế

- **Báo cáo doanh nghiệp:** Tóm tắt từ chi tiết đến executive summary
- **Tài liệu nghiên cứu:** Từ phân tích sâu đến key findings
- **Thuyết trình:** Từ nội dung đầy đủ đến elevator pitch

---

> 📚 **Thuật ngữ liên quan**: [[Glossary - Thuật ngữ Gen AI#Chain of Density|Chain of Density]] | [[Glossary - Thuật ngữ Gen AI#Elevator Pitch|Elevator Pitch]] | [[Glossary - Thuật ngữ Gen AI#Iterative Summarization|Iterative Summarization]]
>
> 🔗 **Xem thêm**: [[02 - 09 - Summarize lengthly documents|Tóm tắt tài liệu dài]] | [[02 - 12 - Summarization best practices|Best practices tóm tắt]]
>
> 🎯 **Thực hành**: [[01 - 09 - Practice 4 iteration methods|Phương pháp iteration]] | [[01 - 10 - Generate better outputs through iteration|Cải thiện output]]

## Kết luận

Chain of density prompting là một kỹ thuật mạnh mẽ giúp bạn kiểm soát mức độ chi tiết của tóm tắt từ trí tuệ nhân tạo tạo sinh (Gen AI). Thay vì chấp nhận kết quả đầu tiên, bạn có thể sử dụng quy trình lặp lại có kiểm soát để đạt được độ súc tích và tập trung mong muốn, đồng thời đảm bảo chất lượng và độ chính xác của thông tin.
