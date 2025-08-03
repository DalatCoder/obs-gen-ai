## Chiến lược Phân tích Dữ liệu với AI Tạo sinh

### Tổng quan về khả năng AI trong phân tích dữ liệu

- **AI tạo sinh có thể giúp bạn** trong vài giây:
    - Phát hiện các patterns (mô hình)
    - Nhận ra mối liên kết giữa các data points (điểm dữ liệu)
    - Xác định trends (xu hướng)
- **Mục tiêu**: Đưa ra quyết định dựa trên dữ liệu với sự tự tin
- **Công cụ chính**: Prompt phù hợp sử dụng [[Prompting Framework]] - **T**houghtfully **C**reate **R**eally **E**xcellent **I**nputs


### Nguyên tắc cơ bản khi tạo prompt cho phân tích dữ liệu

- **Luôn xem xét chính sách công ty** trước khi đưa dữ liệu nhạy cảm vào prompt
- Điều chỉnh chiến lược prompt để phù hợp với dataset (bộ dữ liệu)
- Hiểu rõ **strengths (điểm mạnh)** và **limitations (hạn chế)** của công cụ AI đang sử dụng


### Các chiến lược prompting theo khả năng của mô hình

#### 1. Text Analysis (Phân tích văn bản)

- **Khả năng**: Tìm ra themes (chủ đề), xác định tone (giọng điệu), phân loại topics (chủ đề chính)
- **Ví dụ ứng dụng**: Phân tích hàng nghìn phản hồi mở từ khảo sát cộng đồng
- **Kết quả**: Hiểu điều gì quan trọng nhất với người dân, cảm xúc về kế hoạch đề xuất


#### 2. Data Augmentation (Mở rộng dữ liệu)

- **Mục đích**: Mở rộng dataset hạn chế bằng simulated data (dữ liệu mô phỏng)
- **Ví dụ**: Phân tích dữ liệu gian lận mua sắm khi chỉ có vài data points
- **Lưu ý quan trọng**:
    - Minh bạch về dữ liệu thật và dữ liệu mở rộng
    - Augmentation chỉ gợi ý trends, không đưa ra hard facts (sự thật tuyệt đối)
    - Kiểm tra chính sách tổ chức


#### 3. Question and Answering (Hỏi đáp)

- **Khả năng**: Trả lời về dữ liệu bằng ngôn ngữ đơn giản
- **Ví dụ**: "Doanh số quý trước tăng hay giảm?"
- **Ưu điểm**: Như hỏi đồng nghiệp đã biên soạn thông tin, ít email hơn


#### 4. Scenario Analysis (Phân tích kịch bản)

- **Cách hoạt động**: Phát hiện patterns trong dữ liệu quá khứ để dự đoán tương lai
- **Ứng dụng**:
    - Tác động của thay đổi traffic patterns (mô hình giao thông) đến thời gian đi lại
    - Dự đoán ngày nào văn phòng có nhiều khách nhất


#### 5. Image and Visual Analysis (Phân tích hình ảnh và trực quan)

- **Khả năng**: Xác định patterns nhanh chóng từ visual data (dữ liệu trực quan)
- **Ví dụ**: Paste biểu đồ sales figures (số liệu bán hàng) 2 năm và đặt câu hỏi phân tích


#### 6. Customer and Market Research (Nghiên cứu khách hàng và thị trường)

- **Dữ liệu phân tích**: Khảo sát, social media, biểu đồ ngành
- **Mục tiêu**: Khám phá customer wants (nhu cầu khách hàng) và market changes (thay đổi thị trường)


### Xử lý các tác vụ ngoài khả năng AI

#### Với Statistical Analysis (Phân tích thống kê) hoặc Highly Structured Data (dữ liệu có cấu trúc cao):

- **Không yêu cầu AI thực hiện trực tiếp**
- **Thay vào đó**: Yêu cầu AI đề xuất methods (phương pháp) hiệu quả nhất
- **Lợi ích**: Học các phương pháp phân tích nhanh hơn tự học
- Thiết kế prompt phù hợp với limitations không hạn chế công việc


#### Lưu ý về Hallucinations (ảo giác AI)

- **Vấn đề**: Trong 100 data points được tạo, có thể có 10 điểm là hallucination
- **Giải pháp**:
    - Giám sát chặt chẽ outputs (kết quả đầu ra)
    - Chỉ tạo thông tin có thể cross-referenced (tham chiếu chéo) dễ dàng


### Chuẩn bị Dataset

#### Nguyên tắc: "Output chỉ tốt bằng data nó dựa trên"

- **Validate data** (xác thực dữ liệu) liên tục
- Kiểm tra thông tin đang phân tích với AI


#### Sử dụng AI để chuẩn bị dataset:

- Identify errors (xác định lỗi)
- Phát hiện strange-looking data points (điểm dữ liệu bất thường)
- Standardize formatting (chuẩn hóa định dạng)


#### Prompt mẫu để kiểm tra dataset:

```
Here's a sample of my data. Identify any potential issues or inconsistencies in the data, and suggest ways that I can address them.
```


#### Quy trình đa công cụ:

- Công cụ AI thứ nhất: Convert dataset format (chuyển đổi định dạng)
- Công cụ AI thứ hai: Đặt câu hỏi về thông tin đã tổ chức


### Khuyến khích khám phá (Exploration)

#### Chiến lược đặt câu hỏi:

- **Sử dụng broad, open-ended questions** (câu hỏi rộng, mở)
- **Không prescriptive** (không quy định cứng nhắc)
- **Cho AI tự do** identify patterns và detect insights
- **Giữ thái độ curious** (tò mò)


#### Prompt mẫu cho journalist (nhà báo):

```
You're a journalist investigating housing trends. How would you use this vacant property data to tell a compelling story about the real estate market?
```

- Luôn theo [[Prompting Framework]] để đánh giá **credibility** (độ tin cậy) và **accuracy** (độ chính xác)


### Tận dụng Embedded AI Tools (Công cụ AI tích hợp)

#### Các nền tảng chính:

**[[Gemini in Google Sheets]]**:

- Tạo tables (bảng), thiết lập formulas (công thức)
- Tóm tắt Drive files hoặc Gmail messages
- Tổ chức và phân tích dữ liệu trực tiếp trong spreadsheet

**[[Tableau Pulse]]**:

- Nhận personalized, automated insights (thông tin chi tiết cá nhân hóa, tự động)
- Snapshots trên Tableau Cloud platform
- Regular digests qua Slack hoặc email

**[[Looker Studio]]**:

- Thư viện phong phú các report templates (mẫu báo cáo)
- Khám phá underlying data (dữ liệu cơ bản) qua prebuilt data connectors
- Embed final reports vào web page hoặc intranet

**[[BigQuery Data Insights]]**:

- Khám phá patterns, đánh giá data quality (chất lượng dữ liệu)
- Statistical analysis bằng automated queries dựa trên metadata


#### Prompt mẫu cho Google Sheets:

```
Create a table that includes the median rate of vacancy for each city in the dataset.
```


### Ghi chú thêm

- **AI là powerful assistant** (trợ lý mạnh mẽ) trong việc làm việc với dataset
- **Kết hợp**: Prompt phù hợp + công cụ phù hợp + dữ liệu sạch + câu hỏi rộng
- **Kết quả**: Tìm ra stories và insights có thể bị chôn vùi
- Luôn duy trì thái độ khám phá để phát hiện điều bất ngờ

**Liên kết:** [[Generative AI]], [[Prompting Framework]], [[Data Analysis]], [[Text Analysis]], [[Data Augmentation]], [[Statistical Analysis]], [[Gemini in Google Sheets]], [[Tableau Pulse]], [[Looker Studio]], [[BigQuery Data Insights]], [[Customer Research]], [[Market Research]]

