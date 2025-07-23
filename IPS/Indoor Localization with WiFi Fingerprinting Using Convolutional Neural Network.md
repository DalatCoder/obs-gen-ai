# Thông tin bài báo

- **Tên bài báo:** Indoor Localization with WiFi Fingerprinting Using Convolutional Neural Network (Định vị trong nhà bằng Vân tay WiFi sử dụng Mạng nơ-ron tích chập)
    
- **Tác giả:** Jin-Woo Jang, Song-Nam Hong
    
- **Tổ chức:** Đại học Ajou, Suwon, Hàn Quốc
    
- **Hội nghị:** The International Conference on Ubiquitous and Future Networks (ICUFN) 2018
    
- **Từ khóa:** Indoor Positioning (Định vị trong nhà), Convolutional Neural Network (Mạng nơ-ron tích chập), WiFi fingerprints (Vân tay WiFi)1.
    

---

# Mục tiêu nghiên cứu

Mục tiêu chính của bài báo là đề xuất một phương pháp định vị trong nhà dựa trên

**Mạng nơ-ron tích chập (Convolutional Neural Network - CNN)**2. Nghiên cứu này nhằm giải quyết điểm yếu của các phương pháp dựa trên Mạng nơ-ron sâu (Deep Neural Network - DNN) truyền thống, vốn rất nhạy cảm với sự biến động của tín hiệu WiFi do hiện tượng đa đường (multipath) gây ra3.

Bằng cách khai thác

**cấu trúc topo của bản đồ vô tuyến (topology of a radio map)** thay vì chỉ dựa vào cường độ tín hiệu, mục tiêu là tạo ra một mô hình mạnh mẽ (robust), ít bị ảnh hưởng bởi những thay đổi nhỏ của tín hiệu thu được4444. Cuối cùng, bài báo chứng minh rằng phương pháp CNN đề xuất có hiệu năng vượt trội so với các phương pháp DNN khác trên bộ dữ liệu công khai5.

---

# Bối cảnh và động lực

- **Vấn đề:** Các phương pháp định vị trong nhà dựa trên DNN tuy cho hiệu năng hấp dẫn nhưng lại rất nhạy cảm với sự thay đổi của tín hiệu đầu vào6. Để đạt độ chính xác cao, chúng đòi hỏi một tập dữ liệu huấn luyện cực lớn để bao quát nhiều trường hợp nhất có thể, gây ra chi phí tốn kém7.
    
- **Động lực:** Lấy cảm hứng từ sự thành công của CNN trong lĩnh vực phân loại hình ảnh, nơi CNN có khả năng học được cấu trúc tổng thể của một hình ảnh và tỏ ra mạnh mẽ trước các thay đổi nhỏ8. Các tác giả mong muốn áp dụng nguyên lý tương tự cho bài toán định vị trong nhà bằng vân tay WiFi, một phương pháp hiệu quả về chi phí vì tận dụng được hạ tầng mạng có sẵn9999.
    

---

# Các khái niệm chính

- **Mạng nơ-ron tích chập (Convolutional Neural Network - CNN):** Một loại mạng nơ-ron sâu được thiết kế đặc biệt để xử lý dữ liệu có cấu trúc dạng lưới, chẳng hạn như hình ảnh. CNN sử dụng các bộ lọc (filters) trong các lớp tích chập (convolution layers) để học các đặc trưng mang tính không gian (hay "topo") của dữ liệu10.
    
- **Bản đồ vô tuyến 2D (2-D Radio Map):** Trong bài báo này, đây là một ma trận hai chiều được tạo ra bằng cách định hình lại một vector tín hiệu RSSI 1 chiều11. "Bản đồ" này được dùng làm đầu vào cho mô hình CNN, tương tự như một bức ảnh.
    
- **Các kỹ thuật cải thiện độ chính xác:**
    
    - **Co giãn đặc trưng (Feature Scaling):** Chuẩn hóa dữ liệu đầu vào. Bài báo sử dụng
        
        **Robust Scalar**, một phương pháp dựa trên khoảng tứ phân vị (interquartile range - IQR) để giảm thiểu ảnh hưởng của các giá trị ngoại lai (outliers)121212121212.
        
    - **Dropout:** Một kỹ thuật chính quy hóa (regularization) nhằm chống lại hiện tượng quá khớp (overfitting). Nó hoạt động bằng cách ngẫu nhiên vô hiệu hóa một số nút mạng (nodes) trong quá trình huấn luyện13.
        
    - **Cân bằng dữ liệu (Data Balancing):** Quá trình xử lý tập dữ liệu để đảm bảo mỗi nhãn (label) có số lượng mẫu tương đương nhau14. Điều này giúp mô hình không bị học lệch về phía các lớp có nhiều dữ liệu hơn15.
        
    - **Tổ hợp (Ensemble):** Một phương pháp kết hợp kết quả dự đoán từ nhiều mô hình được huấn luyện độc lập để đưa ra quyết định cuối cùng1616. Do các bộ lọc của CNN được khởi tạo ngẫu nhiên, mỗi mô hình sẽ học được các đặc trưng hơi khác nhau, và việc tổ hợp chúng thường cho độ chính xác cao hơn17171717.
        

---

# Phương pháp và kỹ thuật

Mô hình đề xuất sử dụng CNN để phân loại vị trí (tòa nhà và tầng) dựa trên vân tay WiFi18.

### 1. Tiền xử lý dữ liệu: Tạo bản đồ vô tuyến 2D

- **Đầu vào gốc:** Dữ liệu là một vector 1 chiều chứa 520 giá trị RSSI từ 520 điểm truy cập (APs)19191919.
    
- **Chuyển đổi:** Để phù hợp với CNN, vector 1D này được chuyển thành một "ảnh" 2D20.
    
    - 9 giá trị 0 (dummy values) được thêm vào cuối vector 520 chiều để tạo thành một vector 529 chiều21.
        
    - Vector 529 chiều này được định hình lại (reshape) thành một ma trận
        
        **23x23**22. Đây chính là "bản đồ vô tuyến" 2D dùng làm đầu vào cho CNN.
        
- **Chuẩn hóa giá trị:** Các giá trị 100dBm (biểu thị không đo được tín hiệu) trong bộ dữ liệu gốc được đổi thành -110dBm, được xem như tín hiệu cực yếu thay vì dữ liệu bị thiếu23.
    

### 2. Kiến trúc CNN

Kiến trúc CNN cho hiệu năng tốt nhất được xác định qua thử nghiệm và có cấu trúc như sau24242424:

- **Lớp Tích chập & Gộp (Convolution & Pooling):**
    
    - **Khối 1:** 2 lớp Tích chập (64 bộ lọc, kích thước 3x3) -> 1 lớp Gộp cực đại (Max Pooling) với sải bước (stride) là 2. Kích thước bản đồ đặc trưng (feature map) giảm từ 23x23 xuống 12x1225252525.
        
    - **Khối 2:** 2 lớp Tích chập (128 bộ lọc, kích thước 3x3) -> 1 lớp Gộp cực đại (Max Pooling) với sải bước là 2. Kích thước bản đồ đặc trưng giảm từ 12x12 xuống 6x626262626.
        
- **Lớp kết nối đầy đủ (Fully Connected):**
    
    - Bản đồ đặc trưng cuối cùng (kích thước 6x6x128) được duỗi thẳng (flatten) thành một vector 4608 chiều27.
        
    - Vector này đi qua 2 lớp kết nối đầy đủ, mỗi lớp có 512 nút ẩn2828.
        
- **Lớp đầu ra (Output):** Một lớp **Softmax** được sử dụng để phân loại đầu vào vào một trong 13 nhãn (kết hợp Tòa nhà & Tầng)29292929.
    
- **Tối ưu hóa:** Mô hình sử dụng hàm kích hoạt **ReLU** và trình tối ưu hóa **Adam Optimizer**30303030.
    

### 3. Áp dụng các kỹ thuật cải thiện

Mô hình cuối cùng được huấn luyện với đầy đủ các kỹ thuật:

**Robust Scalar** để chuẩn hóa, **Dropout** sau mỗi lớp kết nối đầy đủ, **Data Balancing** (lấy 900 mẫu cho mỗi nhãn) và **Ensemble** (kết hợp 3 mô hình)31313131313131313131313131313131.

---

# Kết quả và số liệu

Các thử nghiệm được thực hiện trên bộ dữ liệu

**UJIIndoorLoc** với 19.937 mẫu huấn luyện và 1.111 mẫu kiểm định (dùng làm tập kiểm tra)32323232.

### So sánh với các mô hình học sâu khác

Độ chính xác trong việc xác định đúng cả **Tòa nhà và Tầng (B&F Accuracy)**:

|Mô hình|SAE + Classifier|Scalable DNN|**Mô hình CNN đề xuất**|
|---|---|---|---|
|**Độ chính xác B&F**|91.1% 33|92.89% 34||**95.41%** 35|

- Kết quả cho thấy mô hình CNN đề xuất có độ chính xác cao hơn các mô hình DNN hiện có từ
    
    **2.52% đến 4.31%**36.
    

### Tác động của các kỹ thuật cải thiện

|Kỹ thuật|Điều kiện|Độ chính xác B&F|Ghi chú|
|---|---|---|---|
|**Feature Scaling**|Sử dụng **Robust Scalar**||**95.41%** 37|Tốt nhất so với Standard (90.63%), Min Max (94.77%), Quantile (85.95%)38.|
|**Dropout**|**Có sử dụng Dropout**||**95.5%** 3939|Cao hơn 1.18% so với khi không sử dụng (94.32%)40404040.|
|**Data Balancing**|Sử dụng **mẫu cân bằng**||**95.13%** 4141|Tốt hơn so với mẫu không cân bằng (94.06%)42424242.|
|**Ensemble**|Sử dụng **3 mô hình**||**95.76%** 43|Tốt nhất so với không sử dụng (94.33%) và 5 mô hình (95.67%)44.|

---

# Đánh giá, ưu – nhược điểm

### Ưu điểm

- **Độ chính xác vượt trội:** Mô hình CNN cho thấy hiệu năng cao hơn đáng kể so với các kiến trúc dựa trên DNN cho cùng bài toán45.
    
- **Tính bền vững (Robustness):** Bằng cách học "cấu trúc topo" của bản đồ vô tuyến 2D, mô hình ít bị ảnh hưởng bởi nhiễu và biến động tín hiệu, điều này đặc biệt hữu ích khi tập dữ liệu bị hạn chế46464646.
    
- **Hiệu quả tính toán:** CNN có số lượng tham số ít hơn so với các mạng DNN kết nối đầy đủ, dẫn đến độ phức tạp thời gian thấp hơn và tốc độ thực thi nhanh hơn trong giai đoạn định vị thực tế47.
    

### Nhược điểm

- **Chỉ phân loại vị trí:** Nghiên cứu chỉ tập trung vào việc xác định vị trí tương đối (tòa nhà, tầng) mà không ước tính tọa độ chính xác (x, y).
    
- **Tính "topo" nhân tạo:** Cấu trúc "topo" mà CNN học được là do việc định hình lại vector 1D một cách nhân tạo, chứ không phản ánh vị trí vật lý thực tế của các điểm truy cập WiFi.
    

---

# Thách thức và hướng cải tiến

- **Thách thức:** Thách thức lớn nhất trong các phương pháp học sâu là sự phụ thuộc vào lượng dữ liệu huấn luyện48. Tuy nhiên, việc thu thập dữ liệu vân tay WiFi rất tốn kém và mất thời gian49. Do đó, việc đạt được độ chính xác cao với một lượng dữ liệu hạn chế là mục tiêu quan trọng.
    
- **Hướng cải tiến:** Bài báo chứng minh rằng phương pháp CNN có thể cải thiện độ chính xác mà không cần thu thập thêm dữ liệu50. Các hướng phát triển tiếp theo có thể bao gồm việc áp dụng kiến trúc này cho bài toán hồi quy (ước tính tọa độ) hoặc khám phá các cách biến đổi dữ liệu 1D thành 2D có ý nghĩa hơn về mặt vật lý.
    

---

# Ứng dụng thực tiễn

Với độ chính xác cao và tốc độ xử lý nhanh trong thời gian thực 51, mô hình CNN đề xuất có thể được ứng dụng rộng rãi trong nhiều lĩnh vực52:

- 📢 Hệ thống quảng cáo theo ngữ cảnh trong các trung tâm thương mại phức hợp.
    
- 🚗 Định vị vị trí xe trong các bãi đỗ xe lớn.
    
- 🆘 Dịch vụ cứu hộ khẩn cấp, xác định vị trí người bị nạn.
    

---

# Nhận xét tổng quan

Bài báo này trình bày một cách tiếp cận sáng tạo và hiệu quả khi áp dụng thành công Mạng nơ-ron tích chập (CNN) cho bài toán định vị trong nhà bằng vân tay WiFi.

Điểm đột phá chính là việc **biến đổi vector tín hiệu RSSI 1D thành một "ảnh" 2D**, cho phép CNN học các đặc trưng về "cấu trúc topo" nhân tạo. Mặc dù cấu trúc này là nhân tạo, kết quả thực nghiệm đã chứng minh nó giúp mô hình trở nên mạnh mẽ hơn đáng kể so với các mô hình DNN truyền thống chỉ xem xét cường độ tín hiệu đơn lẻ.

Nghiên cứu cũng cho thấy một quy trình tối ưu hóa mô hình rất bài bản, từ việc lựa chọn kiến trúc đến việc áp dụng và đánh giá một loạt các kỹ thuật tăng cường hiệu năng. Kết quả không chỉ vượt trội so với các công trình trước đó mà còn chỉ ra rằng đây là một hướng đi đầy hứa hẹn để giải quyết bài toán định vị trong nhà với dữ liệu hạn chế.