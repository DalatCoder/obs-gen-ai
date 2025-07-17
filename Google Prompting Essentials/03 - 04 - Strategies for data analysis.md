# Chiến Lược Phân Tích Dữ Liệu Với [[Glossary - Thuật ngữ Gen AI#Gen AI|Trí Tuệ Nhân Tạo Tạo Sinh]]

> 🧭 **Navigation**: [[03 - 03 - AI IRL - Accelerate analytical tasks with AI by your side|← Trước]] | [[MOC - Google Prompting Essentials|📚 Mục lục]] | [[03 - 05 - Decipher spreadsheets|Tiếp theo →]]

---

## Giới Thiệu

Bạn có bộ dữ liệu (dataset) luôn muốn khám phá? Có nhiều con số cần hiểu rõ? Trong vài giây, trí tuệ nhân tạo tạo sinh (Gen AI) có thể giúp bạn:

- **Phát hiện các mẫu** (spot patterns)
- **Nhận biết kết nối** giữa các điểm dữ liệu
- **Xác định xu hướng** (identify trends)
- **Đưa ra quyết định dựa trên dữ liệu** với sự tự tin

Tất cả chỉ cần **prompt đúng cách**. Viết prompt để phân tích dataset có thể có những **đặc thù riêng** (quirks), nhưng hãy nhớ rằng **khung prompting đáng tin cậy** sẽ hướng dẫn bạn - tức là bạn sẽ **Thoughtfully Create Really Excellent Inputs** (Tạo ra những đầu vào xuất sắc một cách chu đáo), chỉ cần điều chỉnh chiến lược để phù hợp với dataset.

> **Lưu ý quan trọng:** Luôn xem xét chính sách của công ty trước khi đưa dữ liệu nhạy cảm hoặc bí mật vào prompt.

## Điều Chỉnh Prompt Theo Khả Năng Của Mô Hình

## Hiểu Rõ Điểm Mạnh và Hạn Chế

Khi sử dụng công cụ Gen AI để phân tích dữ liệu, prompt cần **tính đến điểm mạnh và hạn chế** của công nghệ bạn đang sử dụng. Hiểu rõ loại phân tích dữ liệu mà công cụ Gen AI giỏi sẽ giúp bạn **tùy chỉnh prompt** và tận dụng tối đa kết quả.

## Các Ví Dụ Ứng Dụng

## 1. Phân Tích Văn Bản (Text Analysis)

- **Khả năng:** Dễ dàng phát hiện chủ đề, xác định giọng điệu, phân loại các chủ đề chính trong dữ liệu văn bản
- **Ví dụ:** Có hàng nghìn phản hồi mở từ khảo sát cộng đồng? Gen AI có thể giúp bạn nhanh chóng hiểu điều gì quan trọng nhất với mọi người, cảm nhận của họ về kế hoạch đề xuất của thị trấn, và nơi sáng kiến cuối cùng nên tạo ra tác động.

## 2. Tăng Cường Dữ Liệu (Data Augmentation)

- **Khả năng:** Mở rộng bộ dữ liệu giới hạn với dữ liệu mô phỏng (simulated data) để làm cho nó mạnh mẽ hơn
- **Ví dụ:** Bạn làm việc trong ngăn chặn gian lận (fraud prevention). Bạn muốn phân tích dữ liệu về giao dịch mua hàng gian lận nhưng chỉ có một vài điểm dữ liệu. Bạn có thể prompt công cụ Gen AI tạo ra dữ liệu mới từ dataset hiện tại để có cái nhìn toàn diện hơn về cách gian lận có thể xảy ra.

> **Lưu ý:** Chìa khóa với data augmentation là phải **minh bạch** về dữ liệu nào thật, dữ liệu nào được tăng cường, và việc tăng cường phải **thực tế nhất có thể**. Augmentation không thể cung cấp **sự thật cứng** (hard facts), chỉ đề xuất xu hướng.

## 3. Hỏi Đáp (Question and Answering)

- **Khả năng:** Nhận câu trả lời về dữ liệu bằng ngôn ngữ tự nhiên
- **Ví dụ:** Doanh số quý trước tăng hay giảm? Giống như kiểm tra với đồng nghiệp đã tổng hợp thông tin - chỉ với ít email hơn.

## 4. Phân Tích Tình Huống (Scenario Analysis)

- **Khả năng:** Bằng cách nhận biết các mẫu trong dữ liệu quá khứ, công cụ Gen AI có thể đưa ra **dự đoán có căn cứ** về điều có thể xảy ra trong tương lai
- **Ví dụ:** Bạn có thể mô phỏng các tình huống khác nhau để kiểm tra tác động, như prompt hỏi thay đổi trong mẫu giao thông sẽ ảnh hưởng đến thời gian đi lại của bạn như thế nào.

## 5. Phân Tích Hình Ảnh và Hình Ảnh (Image and Visual Analysis)

- **Khả năng:** Giúp bạn nhanh chóng xác định mẫu và đưa ra kết luận về dữ liệu hình ảnh
- **Ví dụ:** Bạn có thể dán biểu đồ hiển thị số liệu bán hàng của team trong 2 năm qua vào prompt và đặt câu hỏi về nó để phân tích tập trung hơn.

## 6. Nghiên Cứu Khách Hàng và Thị Trường (Customer and Market Research)

- **Khả năng:** Phân tích khảo sát, mạng xã hội, và dữ liệu chuyên ngành khác như biểu đồ và đồ thị
- **Mục đích:** Khám phá điều khách hàng muốn và cách thị trường đang thay đổi

## Khi Công Cụ Gen AI Không Phù Hợp

Nếu bạn cần hoàn thành **tác vụ phân tích dữ liệu mà chúng không thực sự được xây dựng cho** - như phân tích thống kê nghiêm ngặt (rigorous statistical analysis) hoặc bất cứ điều gì với dữ liệu có cấu trúc cao - đừng lo lắng. Bạn chỉ cần **thích ứng cách prompt** để phù hợp nhất với khả năng của nó.

**Ví dụ:** Thay vì để công cụ Gen AI thực hiện phân tích thống kê cho bạn, hãy yêu cầu nó **đề xuất các phương pháp hiệu quả nhất** dựa trên dữ liệu của bạn với hướng dẫn từng bước.

> **Lưu ý về Hallucinations:** Khi theo dõi khung prompting, bạn sẽ đánh giá đầu ra trong quá trình. Nhưng hãy nhớ rằng **spot checking không thực sự hiệu quả cho datasets** - trong 100 điểm dữ liệu được tạo ra, chỉ 10 có thể là hallucinations. Vì vậy hãy **theo dõi chặt chẽ** đầu ra của bạn và chỉ tạo ra thông tin có thể dễ dàng **tham chiếu chéo** (cross-referenced).

## Chuẩn Bị Dataset

## Nguyên Tắc Cơ Bản

**Đầu ra chỉ tốt bằng dữ liệu mà nó dựa trên.** Điều này có nghĩa là bạn cần **xác thực dữ liệu** và liên tục kiểm tra thông tin bạn đang phân tích với Gen AI.

## Checklist Để Nhập Dữ Liệu Vào Công Cụ Gen AI

Dữ liệu cần đảm bảo:

- **Cập nhật** (up to date)
- **Chính xác** (accurate)
- **Đầy đủ** (complete)
- **Nhất quán** (consistent)
- **Liên quan** (relevant)
- **Không thiên vị** (bias-free)

## Sử Dụng Gen AI Để Chuẩn Bị Dataset

Gen AI có thể giúp bạn chuẩn bị dataset:

- **Xác định lỗi** (identify errors)
- **Phát hiện điểm dữ liệu lạ** (spot strange-looking data points)
- **Chuẩn hóa định dạng** (standardize formatting)

## Ví Dụ Prompt Kiểm Tra Độ Chính Xác

text

`Here's a sample of my data. Identify any potential issues or inconsistencies in the data, and suggest ways that I can address them.`

_(Đây là mẫu dữ liệu của tôi. Xác định bất kỳ vấn đề tiềm ẩn hoặc không nhất quán nào trong dữ liệu, và đề xuất cách tôi có thể giải quyết chúng.)_

## Sử Dụng Nhiều Công Cụ Khác Nhau

**Làm sạch dữ liệu** trước khi tiến hành phân tích là ví dụ tốt về việc sử dụng nhiều công cụ khác nhau để điều tra một dataset duy nhất. Ví dụ:

- Sử dụng một công cụ Gen AI để **chuyển đổi định dạng** dataset
- Sau đó sử dụng công cụ khác để **đặt câu hỏi** về thông tin vừa được tổ chức

## Khuyến Khích Khám Phá

## Sức Mạnh Của Gen AI Trong Khám Phá

Gen AI thực sự giỏi trong việc **khám phá những hiểu biết có thể đang ẩn** trong một dataset lớn. Bạn chỉ cần biết cách prompt công cụ đúng cách.

## Chiến Lược Đặt Câu Hỏi

Bạn muốn đặt **câu hỏi rộng, mở** (broad, open-ended questions). Bằng cách không **quy định cứng nhắc** (prescriptive), bạn đang tạo cơ hội cho công cụ Gen AI xác định các mẫu và phát hiện hiểu biết với một số **tự do**, có thể giới thiệu hoặc tiết lộ xu hướng bạn không mong đợi.

**Quan trọng nhất:** Hãy **giữ tính tò mò** (stay curious). Bạn có thể tìm thấy điều gì đó bất ngờ chỉ bằng cách giữ quan điểm mở.

## Ví Dụ Thực Tế

Bạn là nhà báo (journalist) đang nghiên cứu cho một bài viết về thị trường bất động sản. Bạn được cung cấp một dataset lớn hiển thị các tài sản dân cư trống theo quận trong một số thành phố, nhưng bạn không chắc có thể rút ra kết luận gì từ nó.

text

`You're a journalist investigating housing trends. How would you use this vacant property data to tell a compelling story about the real estate market?`

_(Bạn là một nhà báo đang điều tra xu hướng nhà ở. Bạn sẽ sử dụng dữ liệu tài sản trống này như thế nào để kể một câu chuyện hấp dẫn về thị trường bất động sản?)_

> **Lưu ý:** Luôn theo dõi khung prompting để **đánh giá đầu ra** về **độ tin cậy và tính chính xác** (credibility and accuracy).

## Tận Dụng Các Công Cụ AI Tích Hợp

## Lợi Ích Của AI Tích Hợp

Nhiều nền tảng phân tích dữ liệu hiện có **nhúng AI ngay trong giao diện người dùng**, khiến việc phân tích thông tin trở nên thuận tiện hơn. Các tích hợp này tạo ra quy trình phân tích dữ liệu **liền mạch** (seamless) bằng cách kết nối sức mạnh của AI và hệ thống phân tích dữ liệu chuyên dụng.

## Các Nền Tảng Chính

## 1. Gemini trong Google Sheets

- **Khả năng:** Tạo bảng, thiết lập công thức, tóm tắt file Drive hoặc tin nhắn Gmail
- **Mục đích:** Tổ chức và phân tích dữ liệu trực tiếp trong bảng tính

## 2. Tableau Pulse

- **Khả năng:** Nhận **hiểu biết cá nhân hóa, tự động** về dữ liệu
- **Hình thức:** Ảnh chụp nhanh (snapshots) trên nền tảng Tableau Cloud hoặc tóm tắt thường xuyên qua Slack hoặc email

## 3. Looker Studio

- **Khả năng:**
  - Truy cập thư viện mạnh mẽ các **mẫu báo cáo** (report templates)
  - Khám phá dữ liệu cơ bản dễ dàng qua **trình kết nối dữ liệu có sẵn** (prebuilt data connectors)
  - Nhúng báo cáo cuối cùng vào bất kỳ trang web hoặc intranet nào

## 4. BigQuery Data Insights

- **Khả năng:** Khám phá mẫu, đánh giá chất lượng dữ liệu, thực hiện phân tích thống kê
- **Phương pháp:** Tạo ra các truy vấn tự động (automated queries) dựa trên metadata thông tin

## Ví Dụ Prompt Trong Google Sheets

Giả sử bạn đã lưu dataset về tài sản trống trong Google Sheets. Bạn có thể mở **bảng bên** (side panel) và gõ:

text

`Create a table that includes the median rate of vacancy for each city in the dataset.`

_(Tạo một bảng bao gồm tỷ lệ trống trung bình cho mỗi thành phố trong dataset.)_

## Kết Luận

Lần tới khi bạn làm việc với dataset, hãy nhớ rằng bạn có một **trợ lý mạnh mẽ** trong các công cụ [[Glossary - Thuật ngữ Gen AI#Gen AI|Gen AI]]. Bằng cách:

- **Tạo ra prompt phù hợp** cho công cụ phù hợp
- **Giữ dữ liệu gọn gàng** (keeping data tidy)
- **Đặt câu hỏi rộng** về thông tin

---

> 📚 **Thuật ngữ liên quan**: [[Glossary - Thuật ngữ Gen AI#Text Analysis|Text Analysis]] | [[Glossary - Thuật ngữ Gen AI#Data Augmentation|Data Augmentation]] | [[Glossary - Thuật ngữ Gen AI#Question Answering|Question Answering]]
>
> 🔗 **Xem thêm**: [[03 - 02 - Use AI to uncover hidden patterns in data|Khám phá patterns]] | [[03 - 05 - Decipher spreadsheets|Giải mã bảng tính]]
>
> 🎯 **Thực hành**: [[01 - 05 - Use the 5-step prompt framework|Framework prompting]] | [[03 - 06 - Decipher almost anything with the help of AI|Giải mã với AI]]

- **Tận dụng tất cả các loại công cụ**

Bạn sẽ tìm thấy các **câu chuyện (stories) và hiểu biết (insights)** có thể đã bị chôn vùi. Ai biết bạn sẽ khám phá ra điều gì tiếp theo?
