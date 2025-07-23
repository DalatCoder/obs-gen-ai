# Thông tin bài báo

- **Tên bài báo**: A Review of Open Access WiFi Fingerprinting Datasets for Indoor Positioning (Tổng quan về các bộ dữ liệu WiFi Fingerprinting truy cập mở cho định vị trong nhà) 1
    
- **Tác giả**: Xu Feng, Khuong An Nguyen, and Zhiyu Luo 2
    
- **Tổ chức**: Khoa Khoa học Máy tính, Royal Holloway University of London, U.K. 3
    
- **Xuất bản tại**: IEEE Access 4
    
- **Năm xuất bản**: 2024 (Ngày nhận 1/10/2024, ngày xuất bản 12/11/2024) 5
    
- **DOI**: 10.1109/ACCESS.2024.3496561 6
    
- **Từ khóa**: Định vị trong nhà (Indoor positioning), WiFi fingerprinting, bộ dữ liệu truy cập mở (open access dataset) 7
    

# Mục tiêu nghiên cứu

Bài báo thực hiện một tổng quan toàn diện và phân tích sâu hơn 50 bộ dữ liệu WiFi fingerprinting có sẵn công khai. 8 Mục tiêu chính bao gồm:

- Cung cấp một cái nhìn tổng quan về bối cảnh hiện tại của các bộ dữ liệu WiFi fingerprinting. 9
    
- Kiểm tra và xác thực khả năng truy cập mở của tất cả các bộ dữ liệu được đề cập. 10
    
- Phân tích các yếu tố quan trọng nhất của mỗi bộ dữ liệu, ngay cả khi chúng không được công bố rõ ràng. 11
    
- Đánh giá các thách thức hiện tại và đề xuất các tiêu chuẩn, hướng dẫn để tạo ra các bộ dữ liệu WiFi fingerprint mới hiệu quả hơn. 12121212
    
- Chỉ ra một phát hiện đáng ngạc nhiên: việc tăng số lượng điểm tham chiếu (RPs) và điểm truy cập (APs), sử dụng tọa độ 3D, và tần suất thu thập dữ liệu cao hơn không phải lúc nào cũng đảm bảo hiệu suất định vị tốt hơn. 13131313
    

# Bối cảnh và động lực

- **Thách thức của GPS trong nhà**: Hệ thống định vị toàn cầu (GPS) hoạt động kém hiệu quả trong nhà do tín hiệu vệ tinh không thể xuyên qua các tòa nhà hiện đại và bị ảnh hưởng bởi các hiệu ứng đa đường (multipath), phản xạ, và che khuất. 14
    
- **Sự phổ biến của WiFi**: Nhờ vào hạ tầng điểm truy cập (Access Points - APs) WiFi rộng khắp và sự phổ biến của các thiết bị thông minh, các phương pháp định vị trong nhà dựa trên WiFi trở nên hiệu quả về mặt chi phí. 15Do đó,
    
    **WiFi fingerprinting** là một trong những kỹ thuật phổ biến nhất. 16
    
- **Vấn đề với các bộ dữ liệu hiện có**:
    
    - Các bộ dữ liệu được công bố rất đa dạng về định dạng và mức độ thông tin, thiếu một tiêu chuẩn chung. 17
        
    - Chúng bị phân tán trên nhiều nền tảng khác nhau, gây khó khăn cho các nhà nghiên cứu mới trong việc tìm kiếm và truy cập. 18181818
        
    - Nhiều bộ dữ liệu có liên kết đã hết hạn hoặc bị hạn chế truy cập. 19
        
    - Thiếu các thông tin quan trọng như ảnh hưởng của con người, loại tín hiệu đầu vào, và sự thay đổi của tín hiệu WiFi theo thời gian. 20
        
- **Hệ quả**: Những vấn đề trên dẫn đến việc sử dụng các bộ dữ liệu công khai một cách thiên vị, có khả năng gây ra hiện tượng **overfitting** (quá khớp) cho các thuật toán định vị được đề xuất. 21
    

# Các khái niệm chính

- **WiFi Fingerprinting**: Là một phương pháp định vị ước tính vị trí của người dùng bằng cách so khớp các phép đo tín hiệu WiFi thời gian thực (gọi là "vân tay" - fingerprints) với một bộ dữ liệu vân tay đã được xây dựng trước đó. 22 Quá trình này gồm 2 giai đoạn:
    
    1. **Giai đoạn Offline (Offline Phase)**: Xây dựng một "bản đồ vô tuyến" (radio map) chi tiết, chứa các vân tay WiFi đặc trưng và tọa độ thực (ground truth) tương ứng tại nhiều vị trí trong môi trường. Dữ liệu này sau đó được làm sạch và tiền xử lý. 23
        
    2. **Giai đoạn Online (Online Phase)**: Khi người dùng yêu cầu định vị, hệ thống thu thập một mẫu WiFi thời gian thực, so sánh nó với bản đồ vô tuyến để ước tính vị trí hiện tại. 24242424
        
- **Các loại tín hiệu WiFi đầu vào (Signal Inputs)**:
    
    - **RSS (Received Signal Strength)**: Còn gọi là RSSI, là chỉ số đo cường độ tín hiệu nhận được từ các AP. Đây là phép đo được sử dụng rộng rãi nhất do dễ dàng truy cập. 25
        
    - **RTT (Round Trip Time)**: Đo thời gian tín hiệu di chuyển từ thiết bị phát đến thiết bị thu và quay trở lại. RTT có thể được dùng để tính toán trực tiếp khoảng cách. 26Nó nhạy cảm hơn với các thay đổi trong môi trường so với RSS, đặc biệt trong các kịch bản không có tầm nhìn thẳng (NLOS). 27
        
    - **CSI (Channel State Information)**: Mô tả các thuộc tính của kênh truyền tín hiệu, chẳng hạn như sự tán xạ, phai màu, và đa đường. CSI cung cấp thông tin chi tiết hơn nhiều so với RSS, giúp mô tả hành vi tín hiệu trong môi trường phức tạp và mang lại giải pháp mạnh mẽ hơn. 28282828
        

# Phương pháp và kỹ thuật

Đây là một bài báo tổng quan, vì vậy phương pháp của nó là phương pháp rà soát và phân tích tài liệu một cách có hệ thống.

- **Phạm vi rà soát**: Tập trung vào các bộ dữ liệu WiFi fingerprinting được thiết kế cho mục đích định vị trong nhà và phải có quyền truy cập công khai hợp lệ. 29292929
    
- **Phương pháp tìm kiếm**:
    
    - Sử dụng các từ khóa tìm kiếm như: "WiFi", "indoor", "localization", "positioning", "fingerprint*", "dataset", "database". 30
        
    - Tìm kiếm trên các nền tảng xuất bản dữ liệu công khai nổi tiếng như Zenodo, Github, UCI Machine Learning Repository, IEEE Dataport, Kaggle, v.v. 31Kết quả cho thấy
        
        **Zenodo (30 bộ) và Github (10 bộ)** là hai nền tảng phổ biến nhất. 32323232
        
- **Tiêu chí lựa chọn**:
    
    - Các bộ dữ liệu phải có quyền truy cập mở, hợp lệ và đã được xác minh thủ công. 33
        
    - Phải có mô tả về các đặc điểm của bộ dữ liệu hoặc có bài báo khoa học tương ứng để tham chiếu. 34
        
    - Các bộ dữ liệu không có nhãn tọa độ thực (ground truth) hoặc mô tả không đầy đủ đều bị loại trừ. 35
        

# Kết quả và số liệu

Bài báo đã phân tích 52 bộ dữ liệu công khai và đưa ra các thống kê chi tiết:

- **Loại môi trường thử nghiệm (Testbed)**:
    
    - Phổ biến nhất là
        
        **toàn bộ tòa nhà (Building)** với 24/52 bộ dữ liệu, trong đó 17 là các tòa nhà đại học. 36
        
    - Các môi trường khác bao gồm tầng nhà (Floor, 15 bộ), phòng (Room, 8 bộ), và các không gian nhỏ hơn như hành lang. 37
        
- **Loại định vị (2D/3D)**:
    
    - **29/52** bộ dữ liệu hỗ trợ định vị 3D. 3838
        
    - Trong đó, 26 bộ cung cấp thông tin về tầng (floor identifier) thay vì tọa độ Z chi tiết, do việc ghi nhận sự thay đổi chiều cao của thiết bị là phức tạp. 39393939
        
- **Loại tín hiệu đầu vào**:
    
    - **RSS** chiếm ưu thế tuyệt đối với **49/52** bộ dữ liệu. 40
        
    - Chỉ có
        
        **4 bộ dữ liệu chứa RTT** và **3 bộ dữ liệu chứa CSI**, cho thấy sự thiếu hụt nghiêm trọng của các loại tín hiệu mới này. 41414141
        
- **Thiết bị thu thập**:
    
    - **Điện thoại thông minh (Smartphone)** và máy tính bảng là phổ biến nhất, được sử dụng trong **30/52** bộ dữ liệu. 42
        
    - Các thiết bị khác bao gồm Raspberry Pi (7 bộ), WiFi adaptor (4 bộ), và ESP32. 43
        
- **Phương pháp thu thập tọa độ thực (Ground Truth Acquisition)**:
    
    - **23/52** bộ dữ liệu sử dụng phương pháp thủ công (đo đạc bằng tay, dùng mốc có sẵn). 44
        
    - **4 bộ** sử dụng robot được trang bị cảm biến (LIDAR, IMU, camera RGB-D). 45
        
    - Các phương pháp khác bao gồm hệ thống mobile mapping, ORB-SLAM3, và máy toàn đạc (total station). 46
        
- **Các mô hình Machine Learning được dùng để đánh giá hiệu suất**:
    
    - **k-Nearest Neighbors (KNN)**: Là mô hình phổ biến nhất, xuất hiện trong 26/52 bộ dữ liệu. 47
        
        - Đạt sai số định vị
            
            **0.781 m** trong một tầng nhà đại học, **0.394 m** trong phòng làm việc, và **0.562 m** trong một căn hộ. 48
            
        - Một biến thể là SRL-KNN đạt sai số
            
            **0.66 m**. 49
            
    - **INN (1-Nearest Neighbor)**: Một phiên bản đơn giản hơn của KNN, cũng được sử dụng rộng rãi để thiết lập hiệu suất cơ bản. Ví dụ, trên bộ dữ liệu UjiIndoorLoc, INN đạt sai số
        
        **7.9 m**. 50505050
        
    - **Mạng nơ-ron (Neural Networks)**:
        
        - **ANN (Artificial Neural Network)**: Đạt sai số ước tính khoảng cách **4 m** (với độ tin cậy 98%) trên một bộ dữ liệu WiFi RTT. 51
            
        - **CNN (Convolutional Neural Network)**: Phương pháp CNNLoc sử dụng 1D-CNN đạt sai số **7.60 m** trên bộ dữ liệu UTSIndoorLoc. 52 Một mô hình 1D-CNN khác đạt sai số
            
            **1.38 m** trên bộ dữ liệu CSUIndoorLoc.
            
        - **LSTM (Long Short-Term Memory)**: Đạt sai số **0.62 m** trên bộ dữ liệu XJTLUIndoorLoc. 53Biến thể
            
            **BILSTM** đạt sai số **0.82 m** và **0.70 m** trên các bộ dữ liệu khác. 54
            

# Đánh giá, ưu – nhược điểm

- **Hạn chế của các bộ dữ liệu hiện có (Nhược điểm)**:
    
    - **Thiếu hụt nghiêm trọng** các bộ dữ liệu RTT và CSI. 55
        
    - Mô tả không đầy đủ, thông tin quan trọng thường chỉ có trong các bài báo liên quan, nhưng các liên kết này lại không được cung cấp rõ ràng. 56
        
    - Nhiều liên kết truy cập bị hết hạn sau vài năm, thiếu sự bảo trì. 57575757
        
    - Sự không nhất quán và sai lệch giữa trang mô tả, bài báo và trích dẫn gây khó khăn cho việc trích xuất thông tin. 58
        
- **Phân tích ảnh hưởng của các đặc tính lên hiệu suất (Phân tích sâu)**:
    
    - **Không phải "càng nhiều càng tốt"**: Phân tích cho thấy việc có **số lượng AP nhiều hơn không nhất thiết cải thiện hiệu suất**. 59Tương tự,
        
        **số lượng RP nhiều hơn** hoặc **khoảng cách giữa các RP lớn hơn** cũng không cho thấy mối tương quan rõ ràng với việc cải thiện độ chính xác. 60
        
    - **Tần suất thu thập**: Tần suất thu thập WiFi cao hơn (ví dụ 100 Hz) có ảnh hưởng tối thiểu đến hiệu suất cuối cùng, vì nó chỉ tạo ra nhiều mẫu vân tay tương tự nhau trong một khoảng thời gian ngắn. 61
        
    - **Định vị 2D vs. 3D**: Các bộ dữ liệu được thiết kế cho định vị 3D có xu hướng cho hiệu suất **kém ổn định hơn** vì tín hiệu WiFi không thay đổi nhiều theo chiều dọc. 62
        
    - **Yếu tố tích cực**: Các yếu tố có xu hướng cải thiện hiệu suất bao gồm: môi trường thử nghiệm nhỏ hơn, số lượng mẫu dữ liệu lớn hơn, và loại tín hiệu chứa nhiều thông tin hơn (như RTT, CSI). 63
        

# Thách thức và hướng cải tiến

- **Thách thức chính**:
    
    1. Sự thiếu hụt các bộ dữ liệu công khai chất lượng cao cho các tín hiệu mới như RTT và CSI.
        
    2. Thiếu một tiêu chuẩn chung cho việc thu thập, định dạng, mô tả và xuất bản dữ liệu.
        
    3. Vấn đề về tính bền vững và khả năng truy cập lâu dài của các bộ dữ liệu.
        
- **Hướng dẫn để xuất bản bộ dữ liệu WiFi Fingerprint (Hướng cải tiến)**:
    
    1. **Khảo sát môi trường**: Thực hiện khảo sát kỹ lưỡng khu vực thử nghiệm, cung cấp bản đồ chi tiết và diện tích. 64646464
        
    2. **Thu thập Ground Truth**: Cần chú ý cẩn thận đến việc phân chia các điểm tham chiếu (RPs) và thu thập tọa độ thực một cách chính xác. 65
        
    3. **Xác định phương pháp luận rõ ràng**: Ghi lại chi tiết về thiết bị sử dụng, cách cầm thiết bị, loại tín hiệu, tần suất và thời gian thu thập. 66666666Sử dụng các giá trị nhân tạo (ví dụ -200 dBm) để biểu thị các AP không nghe thấy. 67676767
        
    4. **Xuất bản trên nền tảng đáng tin cậy**: Đăng tải bộ dữ liệu kèm mô tả chi tiết lên một nền tảng truy cập mở, ổn định. Bài báo đặc biệt
        
        **khuyến nghị Zenodo** do các tính năng như cấp DOI, tích hợp Github và thống kê sử dụng, đảm bảo tính citable và truy xuất được. 68686868
        

# Ứng dụng thực tiễn

Bài báo này là một nguồn tài nguyên quý giá cho cộng đồng nghiên cứu định vị trong nhà. Các ứng dụng thực tiễn chính là:

- **Hỗ trợ lựa chọn dữ liệu**: Cung cấp một danh sách được rà soát và xác thực gồm hơn 50 bộ dữ liệu, giúp các nhà nghiên cứu nhanh chóng tìm thấy bộ dữ liệu phù hợp nhất cho thuật toán của họ. 69
    
- **Thiết lập đường cơ sở (Baseline)**: Các kết quả hiệu suất được báo cáo trên các mô hình phổ biến (KNN, INN,...) có thể được sử dụng làm đường cơ sở để so sánh với các hệ thống định vị mới. 70
    
- **Hướng dẫn xây dựng dữ liệu mới**: Các tiêu chuẩn và hướng dẫn được đề xuất giúp các nhóm nghiên cứu tránh được những sai lầm phổ biến và tạo ra các bộ dữ liệu chất lượng cao, dễ sử dụng và có giá trị lâu dài cho cộng đồng. 71
    

# Nhận xét tổng quan

Đây là một bài báo tổng quan (survey paper) cực kỳ chi tiết, công phu và có giá trị. Nó không chỉ tổng hợp một danh sách lớn các bộ dữ liệu mà còn thực hiện một công việc quan trọng là **xác thực thủ công** các liên kết truy cập, điều mà nhiều bài báo tổng quan khác không làm. 72

Phát hiện quan trọng nhất và có phần phản trực giác là việc tăng cường các yếu tố như số lượng AP, RP hay tần suất lấy mẫu không phải lúc nào cũng dẫn đến kết quả tốt hơn. 73 Điều này thách thức những giả định phổ biến và gợi ý rằng chất lượng, sự đa dạng và loại tín hiệu có thể quan trọng hơn số lượng đơn thuần.

Các hướng dẫn được đề xuất cho việc xuất bản dữ liệu là rất thực tế và cần thiết, nếu được áp dụng rộng rãi sẽ góp phần giải quyết tình trạng "hỗn loạn" của các bộ dữ liệu hiện nay, thúc đẩy một môi trường nghiên cứu cởi mở và hiệu quả hơn.