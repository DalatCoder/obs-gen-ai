# Sử dụng Gen AI để Trực quan hóa Dữ liệu

## Tổng quan về Trình bày Dữ liệu

Khi thuyết trình với khách hàng tiềm năng, đồng nghiệp hay ban lãnh đạo, nguyên tắc quan trọng là **"thể hiện thay vì kể"** dữ liệu. Trí tuệ nhân tạo tạo sinh (Gen AI) rất hiệu quả trong việc giúp xác định các cách thức tốt nhất để trực quan hóa dữ liệu.

## Khung Prompting (Prompting Framework) cho Trực quan hóa

Áp dụng khung prompting cơ bản:

- **Nhiệm vụ (Task)**: Yêu cầu cụ thể về loại biểu đồ
    
- **Bối cảnh (Context)**: Mô tả tập dữ liệu
    
- **Tham chiếu (References)**: Nếu cần thiết
    
- **Đánh giá và lặp lại (Evaluate & Iterate)**: Tinh chỉnh kết quả
    

## Ví dụ Thực tế: Cửa hàng Sách

## Bối cảnh

Hai đồng sở hữu cửa hàng sách cần phân tích danh sách sách bán chạy nhất để quyết định nhập kho. Dữ liệu bao gồm:

- **Cột dữ liệu**: Title, Published, Genre, First published, Approximate sales in millions
    

**Lưu ý quan trọng**: Không phải tất cả công cụ Gen AI đều có thể phân tích dữ liệu. Cần kiểm tra khả năng của công cụ trước khi sử dụng. Trong trường hợp này, chúng ta sử dụng công cụ Google AI Studio.

## Phương pháp 1: Yêu cầu Gợi ý Loại Biểu đồ

**Prompt mẫu:**

text

`Describe the data set here. This is our context: My data set is a spreadsheet that uses the following columns: Title, Published, Genre, First published, and Approximate sales in millions. Give me options for a chart that shows the correlation between genre and sales. Explain how genre and sales are correlated according to the information.`

_(Mô tả tập dữ liệu ở đây. Đây là bối cảnh của chúng tôi: Tập dữ liệu của tôi là một bảng tính sử dụng các cột sau: Tiêu đề, Xuất bản, Thể loại, Lần xuất bản đầu tiên, và Doanh số bán hàng xấp xỉ tính bằng triệu. Cho tôi các tùy chọn cho một biểu đồ cho thấy mối tương quan giữa thể loại và doanh số bán hàng. Giải thích cách thể loại và doanh số bán hàng có mối tương quan theo thông tin.)_

**Kết quả**: Nhận được 3 ý tưởng tuyệt vời về biểu đồ với giải thích chi tiết, giúp lựa chọn cách trực quan hóa phù hợp nhất.

## Phương pháp 2: Sử dụng Biểu đồ Tham chiếu

Khi không biết loại biểu đồ nào phù hợp, có thể sử dụng biểu đồ tương tự làm tham chiếu.

## Bước 1: Phân tích Biểu đồ Tham chiếu

**Prompt mẫu:**

text

`Describe this chart, what kind of data relationships are highlighted in the chart.`

_(Mô tả biểu đồ này, loại mối quan hệ dữ liệu nào được làm nổi bật trong biểu đồ.)_

**Kết quả**: Mô hình xác định đây là biểu đồ cột xếp chồng (stacked bar chart) thể hiện sự phân bổ nhân sự theo các phòng ban, phân tích chi tiết về tỷ lệ nhân viên toàn thời gian và bán thời gian.

## Bước 2: Áp dụng cho Dữ liệu Riêng

**Prompt mẫu:**

text

`My data set is a spreadsheet that uses the following columns: Title, Published, Genre, First published and Approximate Sales in millions. I am interested in showing the relationship between genre and sales. Suggest modifications to make this chart work better with my specific data using Google Sheets.`

_(Tập dữ liệu của tôi là một bảng tính sử dụng các cột sau: Tiêu đề, Xuất bản, Thể loại, Lần xuất bản đầu tiên và Doanh số bán hàng xấp xỉ tính bằng triệu. Tôi muốn thể hiện mối quan hệ giữa thể loại và doanh số bán hàng. Đề xuất các chỉnh sửa để làm cho biểu đồ này hoạt động tốt hơn với dữ liệu cụ thể của tôi bằng Google Sheets.)_

**Kết quả**: Nhận được hướng dẫn chi tiết về cách tạo biểu đồ mới với dữ liệu sẵn có, bao gồm cả cách chỉnh sửa để thể hiện mối quan hệ giữa thể loại và doanh số rõ ràng hơn.

## Nguyên tắc Quan trọng

## Độ Cụ thể trong Prompt

- Càng rõ ràng về loại biểu đồ mong muốn
    
- Càng chi tiết về các thông số (parameters)
    
- Kết quả càng hữu ích
    

## Quy trình Lặp lại

- Bắt đầu đơn giản, sau đó tăng dần độ phức tạp
    
- Nếu kết quả không như mong muốn, có thể điều chỉnh prompt và lặp lại
    
- Luôn đánh giá và tinh chỉnh kết quả
    

## Sử dụng Tham chiếu Hiệu quả

- Tải lên biểu đồ mẫu tương tự
    
- Yêu cầu mô tả trước khi tái tạo
    
- Áp dụng cấu trúc tương tự cho dữ liệu riêng
    

Phương pháp này giúp tận dụng sức mạnh của Gen AI trong việc tạo ra các biểu đồ trực quan hóa dữ liệu hiệu quả, hỗ trợ quá trình ra quyết định kinh doanh.