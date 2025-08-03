## Sử dụng AI để Tạo Data Visualization và Biểu đồ

### Khái niệm cơ bản

- **Mục tiêu trình bày**: "Show rather than tell" (cho thấy hơn là kể) khi present data (trình bày dữ liệu)
- **Ứng dụng**: Pitch potential clients (thuyết trình khách hàng tiềm năng), relay information (chuyển tải thông tin) cho colleagues hoặc leadership
- **AI có thể giúp**: Xác định **best ways to visualize data** (cách tốt nhất để trực quan hóa dữ liệu)
- **Điều kiện**: Cần biết **what to ask for** (hỏi gì) từ [[AI Tools]]


### Nguyên tắc sử dụng AI cho Data Visualization

#### Áp dụng Prompting Framework

- **Add task, context, references** nếu cần
- **Evaluate output** và **iterate** (lặp lại)
- **Càng rõ ràng** về loại chart muốn tạo và parameters (tham số), output càng hữu ích


#### Lưu ý quan trọng

- **Không phải tất cả [[AI Tools]] có thể analyze data**
- Cần check khả năng của tool trước khi sử dụng
- Ví dụ minh họa sử dụng: [[Google AI Studio]]


### Quy trình thực hành với ví dụ Bookstore

#### Bối cảnh dữ liệu

**Scenario**: Co-owners của bookstore với dữ liệu best-selling books
**Dataset columns**:

- Title (Tiêu đề)
- Published (Năm xuất bản)
- Genre (Thể loại)
- First published (Lần đầu xuất bản)
- Approximate sales in millions (Doanh số xấp xỉ tính bằng triệu)


#### Bước 1: Mô tả dataset và yêu cầu gợi ý

**Context prompt**:

```
My data set is a spreadsheet that uses the following columns: Title, Published, Genre, First published, and Approximate sales in millions.
```

**Task prompt**:

```
Give me options for a chart that shows the correlation between genre and sales.
```


#### Bước 2: Làm rõ loại correlation

**Specific request**:

```
Explain how genre and sales are correlated according to the information.
```

**Kết quả**:

- Nhận được **3 ý tưởng tuyệt vời** để tạo charts visualize data clearly
- **Detailed explanations** (giải thích chi tiết) về mỗi chart
- **Option to choose** (tùy chọn lựa chọn) visualization phù hợp nhất với dataset


### Sử dụng Reference Chart (Biểu đồ tham chiếu)

#### Khi nào sử dụng

- **Không biết loại chart muốn dùng**
- Muốn tạo chart **similar to existing ones** (tương tự những chart có sẵn)
- Có chart mẫu hữu ích muốn emulate (bắt chước)


#### Quy trình với Reference Chart

**Bước 1: Upload sample chart**

```
Describe this chart, what kind of data relationships are highlighted in the chart.
```

**Lý do**: **Start simple** (bắt đầu đơn giản) rồi **gradually add complexity** (dần dần tăng độ phức tạp)

**Bước 2: Phân tích chart mẫu**

- AI xác định: **Stacked bar chart** (biểu đồ thanh xếp chồng)
- **Represents**: Staffing breakdown (phân tích nhân sự) across different departments
- **Analyzed data**: Finance department có high proportion (tỷ lệ cao) full-time staff, Product department có more even mix (hỗn hợp đều hơn)

**Bước 3: Apply vào data riêng**

**Context**:

```
My data set is a spreadsheet that uses the following columns: Title, Published, Genre, First published and Approximate Sales in millions. I am interested in showing the relationship between genre and sales.
```

**Task**:

```
Suggest modifications to make this chart work better with my specific data using Google Sheets.
```

**Kết quả**:

- Nhận được **instructions** về cách tạo new chart với data riêng
- Output giải thích cách **modify bar** để illustrate relationship giữa genre và sales **more clearly** (rõ ràng hơn)


### Nguyên tắc Iteration và Optimization

- **Nếu output không match** với yêu cầu: **tweak prompt** (điều chỉnh prompt) và **iterate** (lặp lại)
- **Flexibility**: AI cho phép thử nghiệm nhiều approaches (cách tiếp cận) khác nhau
- **Continuous improvement**: Có thể refine (tinh chỉnh) cho đến khi đạt kết quả mong muốn


### Lợi ích của việc sử dụng AI cho Data Visualization

- **Time-saving**: Không cần tự nghiên cứu loại chart phù hợp
- **Professional guidance**: Nhận được expert advice (lời khuyên chuyên gia) về chart selection
- **Customization**: Adapt existing charts cho specific data (dữ liệu cụ thể)
- **Learning opportunity**: Hiểu được **data relationships** (mối quan hệ dữ liệu) qua chart analysis


### Ghi chú thêm

- **Plain language**: Có thể mô tả dataset bằng ngôn ngữ tự nhiên
- **Step-by-step approach**: Tốt nhất là từng bước một thay vì làm tất cả cùng lúc
- **Multiple options**: AI thường đưa ra nhiều lựa chọn để consider (xem xét)
- **Detailed explanations**: AI không chỉ suggest mà còn explain why (giải thích tại sao)

**Liên kết:** [[Generative AI]], [[Data Visualization]], [[Google AI Studio]], [[AI Tools]], [[Data Analysis]], [[Prompting Framework]], [[Charts]], [[Stacked Bar Chart]], [[Google Sheets]]

