# Thông tin bài báo

- **Tên bài báo**: Research on Indoor 3D Positioning Algorithm Based on WiFi Fingerprint (Nghiên cứu thuật toán định vị 3D trong nhà dựa trên WiFi Fingerprint)
    
- **Tác giả**: Lixing Wang, Shuang Shang, Zhenning Wu
    
- **Tổ chức**: Northeastern University, Shenyang, China 1111
    
- **Xuất bản tại**: Sensors (MDPI)
    
- **Năm xuất bản**: 2022 (Ngày nhận 15/11/2022, ngày xuất bản 23/12/2022) 2
    
- **DOI**: 10.3390/s23010153 3
    
- **Từ khóa**: WiFi fingerprinting; định vị trong nhà (indoor positioning); DNN; TCN 4
    

# Mục tiêu nghiên cứu

Nghiên cứu này tập trung vào việc phát triển một thuật toán định vị 3D trong nhà (indoor 3D positioning) sử dụng các điểm truy cập không dây (AP) có sẵn mà không cần thêm phần cứng mới. 5Mục tiêu chính là đề xuất một mô hình định vị động 3D mới có tên

**TCN_DNNLoc**, dựa trên các vân tay thời gian (temporal fingerprints) để cải thiện độ chính xác và độ tin cậy (robustness) so với các phương pháp truyền thống. 6666

# Bối cảnh và động lực

- **Hạn chế của công nghệ hiện có**: Các hệ thống định vị vệ tinh như GNSS hoạt động rất kém trong nhà do tín hiệu bị suy giảm hoặc chặn hoàn toàn. 7Trong khi đó, con người dành phần lớn thời gian (87-90%) ở trong nhà, tạo ra nhu cầu lớn cho các dịch vụ dựa trên vị trí (Location-Based Services - LBS) trong nhà. 8
    
- **Ưu điểm của WiFi**: Trong số các công nghệ định vị trong nhà (siêu âm, RFID, UWB, Bluetooth,...), WiFi có lợi thế vượt trội vì không yêu cầu triển khai phần cứng bổ sung, tận dụng được hạ tầng mạng không dây đã có sẵn ở khắp nơi. 9
    
- **Lỗ hổng nghiên cứu (Động lực)**:
    
    - Hầu hết các nghiên cứu hiện tại tập trung vào định vị 2D (trên một mặt phẳng), trong khi các ứng dụng thực tế thường ở môi trường đa tầng. 10
        
    - Các thuật toán truyền thống thường chỉ xem xét một vân tay tại một thời điểm, bỏ qua mối tương quan theo thời gian giữa các chuỗi vân tay. 11Vị trí hiện tại của mục tiêu có liên quan đến các vị trí lịch sử của nó. 12
        
    - Vì vậy, có một nhu cầu cấp thiết để phát triển một mô hình định vị 3D trong nhà có khả năng khai thác dữ liệu không gian-thời gian (spatiotemporal data). 13
        

# Các khái niệm chính

- **Vân tay thời gian (Temporal Fingerprint)**: Thay vì một vector RSSI đơn lẻ, vân tay thời gian là một chuỗi các vector vân tay được thu thập liên tục theo một quỹ đạo tại các thời điểm khác nhau. 14Việc này giúp cung cấp thông tin phong phú hơn, có thể dùng để phân biệt các vị trí có vector vân tay tương tự nhau và cải thiện độ chính xác. 15
    
- **Lát cắt vân tay (Fingerprint Slice)**: Là một ma trận dữ liệu được tạo ra bằng cách sử dụng một **cửa sổ trượt (sliding window)** có kích thước cố định `W` trên chuỗi vân tay thời gian. 16161616Mỗi "lát cắt" này chứa
    
    `W` vector vân tay liên tiếp và được dùng làm đầu vào cho mô hình. 17
    
- **Mạng tích chập thời gian (Temporal Convolutional Network - TCN)**: Là một kiến trúc mạng nơ-ron chuyên dụng cho việc xử lý dữ liệu chuỗi thời gian. 18 Các cơ chế chính của TCN bao gồm:
    
    - **Tích chập nhân quả (Causal convolution)**: Đảm bảo rằng dự đoán tại thời điểm `t` chỉ phụ thuộc vào các quan sát tại thời điểm `t` và trước đó. 1919
        
    - **Tích chập giãn (Dilated convolution)**: Cho phép mạng có một "trường tiếp nhận" (receptive field) lớn hơn để nắm bắt các phụ thuộc dài hạn mà không cần tăng số lượng tham số quá nhiều. 2020
        
    - **Kết nối phần dư (Residual connection)**: Giúp giải quyết các vấn đề về suy giảm gradient (gradient vanishing) và bùng nổ gradient (gradient explosion) trong các mạng sâu. 21212121
        
- **Mạng nơ-ron sâu (Deep Neural Network - DNN)**: Trong mô hình này, một mạng DNN được sử dụng như một bộ hồi quy (regressor) để học mối quan hệ phi tuyến phức tạp giữa các đặc trưng không gian-thời gian (do TCN trích xuất) và tọa độ 3D thực tế. 22222222
    

# Phương pháp và kỹ thuật

Bài báo đề xuất thuật toán

**TCN_DNNLoc**, một mô hình lai kết hợp TCN và DNN. 23Quá trình hoạt động được chia thành 2 giai đoạn: offline và online. 24

1. **Tiền xử lý dữ liệu (Preprocessing)**:
    
    - Dữ liệu RSSI thô được chuẩn hóa để cải thiện khả năng học của mô hình. 25
        
    - Tác giả đã thử nghiệm 3 phương pháp chuẩn hóa và kết luận rằng
        
        **biểu diễn lũy thừa (power representation)** cho kết quả tốt nhất trên bộ dữ liệu được sử dụng. 26262626Sai số trung bình khi dùng phương pháp này là khoảng
        
        **1.23 m**, tốt hơn đáng kể so với không tiền xử lý (khoảng 1.55 m). 272727272727272727
        
2. **Xây dựng lát cắt vân tay**:
    
    - Sử dụng một cửa sổ trượt có kích thước
        
        `W` để quét qua dữ liệu vân tay thời gian. 28
        
    - Mỗi "lát cắt" (một ma trận
        
        `W x N`, với N là số AP) được tạo ra sẽ trở thành một mẫu đầu vào. 29
        
    - Nhãn vị trí (tọa độ 3D) của mỗi lát cắt được lấy từ mẫu vân tay cuối cùng trong cửa sổ đó. 30
        
3. **Kiến trúc mô hình TCN_DNNLoc**:
    
    - **Đầu vào (Input Module)**: Nhận một lát cắt vân tay `W x N`. 31
        
    - **Bộ trích xuất đặc trưng TCN (TCN Feature Extractor)**: Gồm 3 khối phần dư (residual blocks). 32323232Mỗi khối chứa 2 lớp tích chập nhân quả và giãn, theo sau là lớp chuẩn hóa trọng số và lớp kích hoạt ReLU. 33Hệ số giãn
        
        `d` tăng theo cấp số nhân (1, 2, 4) qua các khối để mở rộng trường tiếp nhận. 34
        
    - **Bộ hồi quy DNN (DNN Regressor)**: Các đặc trưng được trích xuất từ TCN được đưa vào một mạng DNN có 2 lớp ẩn. 35Lớp Dropout được thêm vào sau mỗi lớp ẩn để tránh overfitting. 36
        
    - **Đầu ra (Output Module)**: Lớp cuối cùng có 3 nơ-ron, tương ứng với 3 tọa độ (x, y, z) dự đoán. 37
        
4. **Hàm mất mát và Tối ưu hóa**:
    
    - Sử dụng hàm mất mát là
        
        **Sai số bình phương trung bình (Mean Square Error - MSE)**. 38
        
    - Sử dụng thuật toán tối ưu hóa
        
        **Adam**. 39
        

# Kết quả và số liệu

Các thí nghiệm được thực hiện trên bộ dữ liệu công khai

**IMUWIFINE** 40, được thu thập tại một tòa nhà 3 tầng với diện tích hơn 9000

m2 và 220 AP. 41414141

- **Tinh chỉnh siêu tham số**:
    
    - **Số lượng nhân tích chập (TCN)**: Hiệu suất tốt nhất đạt được với **128** nhân. 42
        
    - **Cấu trúc DNN**: Cấu trúc có 2 lớp ẩn, mỗi lớp **128 nơ-ron** (128-128), cho kết quả tối ưu. 43
        
    - **Kích thước cửa sổ trượt (`W`)**: `W=8` cho sai số trung bình thấp nhất. 44Với
        
        `W=8`, 49% kết quả có sai số dưới 1m và **82% có sai số dưới 2m**. 45
        
- **So sánh hiệu suất**:
    
    - Mô hình TCN_DNNLoc được so sánh với các mô hình khác: FNN, SRL_KNN (không tuần tự) và LSTM (tuần tự). 46
        
    - TCN_DNNLoc đạt sai số trung bình 3D thấp nhất là
        
        **1.22 m** trên tập kiểm tra. 4747
        
    - Hiệu suất này
        
        **cải thiện 7.5%** so với LSTM (sai số 1.33 m). 48
        
    - Kết quả vượt trội đáng kể so với FNN (1.71 m) và SRL_KNN (1.66 m). 49
        
    - Đường cong phân phối lỗi tích lũy (CEDF) của TCN_DNNLoc tăng nhanh nhất, cho thấy hiệu suất tổng thể tốt nhất. 50
        

# Đánh giá, ưu – nhược điểm

- **Ưu điểm**:
    
    - Thuật toán TCN_DNNLoc đã chứng minh được hiệu quả của việc sử dụng thông tin thời gian, cho độ chính xác cao hơn hẳn các mô hình chỉ dựa trên một vân tay đơn lẻ. 51
        
    - Việc sử dụng TCN để trích xuất đặc trưng tỏ ra hiệu quả hơn so với LSTM trong bài toán này, mang lại độ chính xác cao hơn 7.5%. 52
        
    - Mô hình có thiết kế end-to-end, trực tiếp ánh xạ chuỗi vân tay đầu vào sang tọa độ 3D đầu ra, đơn giản hóa quy trình định vị. 53
        
- **Nhược điểm**:
    
    - Hiệu suất của mô hình rất nhạy cảm với việc lựa chọn kích thước cửa sổ trượt
        
        `W`. 54Một chuỗi quá dài có thể tích lũy nhiều lỗi hơn. 55
        
    - Nghiên cứu chỉ được xác thực trên một bộ dữ liệu duy nhất (IMUWIFINE), do đó khả năng tổng quát hóa trên các môi trường khác chưa được kiểm chứng. 56
        
    - Bản thân tác giả cũng thừa nhận rằng việc tối ưu hóa trọng số và độ lệch của mô hình có thể được cải thiện thêm bằng các thuật toán heuristic. 57
        

# Thách thức và hướng cải tiến

Bài báo đề xuất hai hướng nghiên cứu trong tương lai: 58

1. **Tối ưu hóa tham số mô hình**: Sử dụng các thuật toán heuristic như thuật toán di truyền (GA) hoặc tối ưu hóa bầy đàn (PSO) để tối ưu hóa các trọng số kết nối và độ lệch của mạng nơ-ron, nhằm tránh rơi vào các điểm tối ưu cục bộ và tăng tốc độ hội tụ. 59
    
2. **Tích hợp đa công nghệ (Multi-technology fusion)**: Kết hợp WiFi với các công nghệ khác hoặc các cảm biến sẵn có trên điện thoại thông minh (như cảm biến áp suất không khí, gia tốc kế) để cung cấp thông tin định vị chính xác hơn, bù đắp cho những hạn chế của một công nghệ đơn lẻ. 60
    

# Ứng dụng thực tiễn

Thuật toán TCN_DNNLoc có thể được ứng dụng rộng rãi trong các tòa nhà đa tầng phức tạp như:

- **Dẫn đường trong nhà**: Hỗ trợ người dùng di chuyển trong các trung tâm mua sắm, thư viện, sân bay. 61616161
    
- **Quản lý đám đông và hàng hóa**: Giám sát thời gian thực trạng thái của nhân viên và hàng hóa. 62
    
- **Cứu hộ khẩn cấp**: Giúp lực lượng cứu hộ nhanh chóng xác định vị trí người gặp nạn. 63
    
- **Dịch vụ thông minh**: Cung cấp hướng dẫn ảo trong bảo tàng hoặc đẩy thông tin quảng cáo tại cửa hàng. 64
    

# Nhận xét tổng quan

Đây là một bài báo nghiên cứu chất lượng, đề xuất một kiến trúc deep learning mới và hiệu quả cho bài toán định vị 3D trong nhà. Đóng góp cốt lõi là việc sử dụng các "lát cắt vân tay thời gian" làm đầu vào và dùng mạng TCN để xử lý, một cách tiếp cận đã được chứng minh là vượt trội hơn so với cả các mô hình tuần tự phổ biến như LSTM và các mô hình không tuần tự. Các phân tích và so sánh được trình bày rõ ràng, chi tiết, cho thấy sự nghiêm túc trong nghiên cứu. Với sai số trung bình 3D chỉ **1.22 m**, mô hình TCN_DNNLoc cho thấy tiềm năng ứng dụng thực tế rất lớn.