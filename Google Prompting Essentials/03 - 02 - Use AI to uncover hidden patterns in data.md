# Sử dụng Trí tuệ nhân tạo tạo sinh (Gen AI) để Phân tích Dữ liệu và Khám phá Insights

## Nguyên tắc Cơ bản khi Phân tích Dữ liệu

## Tầm quan trọng của Việc Diễn giải Dữ liệu

Dữ liệu có thể dạy bạn rất nhiều điều, nhưng trước tiên bạn cần biết cách **diễn giải** (interpret) nó. Sử dụng **khung prompting** (prompting framework) một cách sâu sắc để tạo ra những đầu vào xuất sắc, nhằm mở khóa các **insights** (hiểu biết sâu sắc) và **patterns** (mẫu hình) từ dữ liệu bằng công cụ trí tuệ nhân tạo tạo sinh (Gen AI).

## Lưu ý về Khả năng Công cụ

**Quan trọng:** Không phải tất cả các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) đều làm việc được với dữ liệu. Hãy đảm bảo **kiểm tra khả năng** của công cụ trước khi sử dụng.

## Sử dụng Gemini Models trong Google AI Studio

## Công cụ Thực hành

Khóa học sẽ hướng dẫn cách thực hiện điều này bằng cách **prompting Gemini models** trong **Google AI Studio**.

## Nguyên tắc Sử dụng Gen AI có Trách nhiệm

**Quy tắc cơ bản:**

- **Luôn xem xét chính sách** của tổ chức trước khi đưa dữ liệu nhạy cảm hoặc bí mật vào prompt
    
- **Ví dụ trong khóa học:** Sử dụng dữ liệu công khai từ **Kaggle**
    

## Ví dụ Thực hành: Phân tích Dữ liệu Chuỗi Cửa hàng Tạp hóa

## Bối cảnh Dữ liệu

**Dataset:** Thông tin về một chuỗi cửa hàng tạp hóa (grocery chain)

**Khả năng của AI Studio:**

- Phân tích toàn bộ dữ liệu
    
- Tìm **trends** (xu hướng) và **patterns** (mẫu hình)
    
- Đưa ra thông tin giúp vận hành công ty
    

## Tổ chức Dữ liệu

**Thách thức:** Có nhiều **variables** (biến số), cần tổ chức dữ liệu để dễ làm việc hơn.

**Giải pháp:** Yêu cầu hỗ trợ từng bước (step-by-step help)

## Quy trình Upload Dữ liệu

**Từ Google Drive:**

- Upload dữ liệu trực tiếp từ Google Drive nơi **Google Sheet** được lưu trữ
    

**Từ Microsoft Excel:**

- Upload từ máy tính của bạn
    

## Ví dụ Prompt 1: Tạo Cột Tính toán

## Prompt Mẫu

text

`Attached is a Google sheet of store data. How can I create a new column in sheets that calculates the average sales per customer for each store?`

_(Đính kèm là một Google sheet về dữ liệu cửa hàng. Làm thế nào tôi có thể tạo một cột mới trong sheets để tính toán doanh số bán hàng trung bình cho mỗi khách hàng cho từng cửa hàng?)_

## Kết quả Đạt được

**Gợi ý hữu ích:**

- Tính toán doanh số bán hàng trung bình cho mỗi khách hàng cho từng cửa hàng
    
- Giải thích cách sử dụng **công thức mô tả** (descriptive formula) để đặt nhãn cho cột mới trong bảng tính
    

## Quá trình Iteration

Nếu phương pháp tổ chức không hiệu quả, có thể **lặp lại prompt** để có được đầu ra gần với yêu cầu hơn.

## Ví dụ Prompt 2: Khám phá Xu hướng

## Tầm quan trọng của Việc Khám phá Trends

**Lợi ích:**

- Khám phá xu hướng trong **dataset** (tập dữ liệu) giúp đưa ra quyết định thông minh
    
- Có thể prompt công cụ trí tuệ nhân tạo tạo sinh (Gen AI) để tìm những xu hướng này
    

## Prompt Mẫu

text

`Give me insights into the relationship between daily customer count items, available and sales based on the given data.`

_(Cho tôi hiểu biết sâu sắc về mối quan hệ giữa số lượng khách hàng hàng ngày, các mặt hàng có sẵn và doanh số dựa trên dữ liệu đã cho.)_

## Kết quả Thú vị

**Findings quan trọng:**

- Nhận được **nhiều thông tin thú vị** một cách nhanh chóng
    
- **Không có mối tương quan rõ ràng** giữa số lượng mặt hàng trong cửa hàng và tổng doanh thu
    
- **Một số cửa hàng nhỏ** thậm chí còn vượt trội hơn các cửa hàng lớn
    

**Giá trị bổ sung:**

- Đầu ra đưa ra **những lý do tiềm năng** đằng sau xu hướng này
    
- Cho phép điều tra sâu hơn và suy nghĩ về **chiến lược bán hàng** tiềm năng
    

## Lợi ích Tổng thể của Gen AI trong Phân tích Dữ liệu

## Tiết kiệm Thời gian

**Trước đây:**

- Phải dành hàng giờ để **crunching data** (xử lý dữ liệu)
    

**Hiện tại:**

- Có thể thực hiện với chỉ **vài prompts**
    
- Nhận được **meaningful insights** (hiểu biết có ý nghĩa) một cách nhanh chóng
    

## Khả năng Ứng dụng

**Câu hỏi tự vấn:** Bạn có thể nghĩ về một bảng tính mà bạn đã định phân tích không? Hãy ghi nhớ điều đó khi đi qua ví dụ này.

**Ứng dụng thực tế:** Trí tuệ nhân tạo tạo sinh (Gen AI) có thể giúp tiết kiệm thời gian và trích xuất những hiểu biết có ý nghĩa từ dữ liệu của bạn.

## Kết luận

Với sự hỗ trợ của các công cụ trí tuệ nhân tạo tạo sinh (Gen AI), chúng ta không còn phải dành hàng giờ để xử lý dữ liệu. Chỉ với vài prompts được thiết kế tốt, chúng ta có thể:

- **Tổ chức dữ liệu** hiệu quả
    
- **Khám phá xu hướng** và mẫu hình
    
- **Trích xuất insights** có giá trị
    
- **Đưa ra quyết định** dựa trên dữ liệu
    

Điều quan trọng là phải sử dụng các công cụ này một cách có trách nhiệm, luôn tuân thủ chính sách bảo mật của tổ chức và kiểm tra khả năng của công cụ trước khi sử dụng.