# Thông tin bài báo

- **Tên bài báo:** A survey of deep learning approaches for WiFi-based indoor positioning (Một khảo sát về các phương pháp học sâu cho định vị trong nhà dựa trên WiFi) 1
- **Tác giả:** Xu Feng, Khuong An Nguyen & Zhiyuan Luo 2
- **Tạp chí:** Journal of Information and Telecommunication 3
- **Năm xuất bản:** 2022 (Nộp online: 20/09/2021) 4
- **DOI:** 10.1080/24751839.2021.1975425 5
- **Tóm tắt:** Bài báo này là một bài khảo sát (survey) toàn diện, đánh giá hơn 150 công trình nghiên cứu ứng dụng [[Deep Learning|học sâu (deep learning)]] vào bài toán [[Indoor Positioning System|định vị trong nhà]] dựa trên kỹ thuật [[WiFi Fingerprinting|vân tay WiFi (WiFi fingerprinting)]]. Mục tiêu là xác định các kiến trúc mạng nơ-ron hiệu quả nhất và so sánh độ chính xác của các loại tín hiệu WiFi khác nhau. 6666

---

# Mục tiêu nghiên cứu

Bài báo khảo sát nhằm trả lời hai câu hỏi nghiên cứu chính:

1. **Đâu là thước đo tín hiệu WiFi chính xác nhất cho hệ thống [[Indoor Positioning System|định vị trong nhà]]?** So sánh giữa [[RSSI|Cường độ tín hiệu thu được (Received Signal Strength - RSS)]], [[CSI|Thông tin trạng thái kênh (Channel State Information - CSI)]], và [[RTT|Thời gian trọn vòng (Round-Trip Time - RTT)]]. 7
2. **Đâu là các mạng nơ-ron (neural networks) hiệu quả nhất cho [[Indoor Positioning System|định vị trong nhà]] bằng WiFi?** Bài báo kiểm chứng giả thuyết liệu các mạng phức tạp (như [[CNN]] với hàng chục/trăm lớp ẩn) có luôn cho kết quả tốt hơn các mạng đơn giản hay không. 8

---

# Bối cảnh và động lực

- Định vị trong nhà bằng WiFi, đặc biệt là phương pháp [[WiFi Fingerprinting|vân tay (fingerprinting)]], từ lâu đã được xem là một bài toán [[Machine Learning|học máy (machine learning)]] truyền thống, đạt độ chính xác trung bình ở mức vài mét. 9
- Gần đây, [[Deep Learning|học sâu (deep learning)]] nổi lên như một phương pháp thay thế đầy hứa hẹn, với nhiều công bố đạt được độ chính xác dưới một mét (sub-metre). 10
- Các phương pháp [[Machine Learning|học máy]] nông (shallow learning) truyền thống gặp khó khăn trong việc xử lý dữ liệu WiFi có chiều dữ liệu cao (high-dimensional data) và khó đạt được độ chính xác dưới mét. 11111111
- Sự phát triển của [[Deep Learning|học sâu]] cho phép xử lý hiệu quả lượng dữ liệu lớn này, tìm ra các biểu diễn (representations) có giá trị của dữ liệu WiFi để cải thiện độ chính xác. 12121212
- Do đó, một bài khảo sát tổng hợp và đánh giá các phương pháp này là cần thiết và kịp thời. 13

---

# Các khái niệm chính

### 1. [[WiFi Fingerprinting|Vân tay WiFi (WiFi Fingerprinting)]]

Đây là phương pháp phổ biến nhất trong định vị WiFi, bao gồm hai giai đoạn: 14

- **[[Offline Phase|Giai đoạn Ngoại tuyến (Offline Phase)]]:** Thu thập tín hiệu WiFi tại các [[Reference Points|điểm tham chiếu (reference points)]] trong khu vực mục tiêu để xây dựng một cơ sở dữ liệu (còn gọi là [[Radio Map|bản đồ vô tuyến - radio map]]). Dữ liệu này được tiền xử lý và gán nhãn vị trí (tọa độ, tầng, tòa nhà). 15
- **[[Online Phase|Giai đoạn Trực tuyến (Online Phase)]]:** Khi người dùng ở một vị trí không xác định, thiết bị của họ sẽ đo tín hiệu WiFi hiện tại. Tín hiệu này sau đó được so khớp với cơ sở dữ liệu để ước tính vị trí của người dùng. 16161616
  Mỗi vị trí trong nhà có một "vân tay" tín hiệu WiFi đặc trưng do sự phức tạp của môi trường (tường, vật cản, người) gây ra hiện tượng đa đường (multipath), suy hao (attenuation) và phản xạ (reflection). 17171717

### 2. Các loại tín hiệu WiFi

- **[[RSSI|Cường độ tín hiệu thu được (Received Signal Strength - RSS)]]:**
  - Là loại tín hiệu phổ biến và dễ thu thập nhất từ hầu hết các thiết bị. 18181818
  - Đơn vị là dBm. 19
  - Giá trị
    `100` trong tập dữ liệu mẫu thường biểu thị không nhận được tín hiệu từ [[Access Points|Access Point (AP)]] đó. 20
- **[[CSI|Thông tin trạng thái kênh (Channel State Information - CSI)]]:**
  - Là thông tin chi tiết về đặc tính của kênh truyền (channel properties) trong một liên kết giao tiếp, thu được qua kỹ thuật OFDM (Orthogonal Frequency-Division Multiplexing). 21
  - [[CSI]] mô tả các hiệu ứng tổng hợp như đa đường, tán xạ, suy hao, ổn định hơn [[RSSI]] theo thời gian nhưng rất đặc trưng về không gian. 22
  - [[CSI]] bao gồm hai thành phần: biên độ (amplitude) và pha (phase). 23
  - Khó thu thập hơn [[RSSI]], đòi hỏi phải truy cập vào driver của card mạng WiFi, gây khó khăn khi triển khai trên smartphone. 24
- **[[RTT|Thời gian trọn vòng (Round-Trip Time - RTT)]]:**
  - Là một công nghệ mới được giới thiệu trong chuẩn IEEE 802.11-https://www.google.com/search?q=2016, sử dụng giao thức Fine Time Measurement (FTM). 25
  - Cho phép tính toán trực tiếp thời gian tín hiệu di chuyển giữa thiết bị phát và thu. 26
  - Tại thời điểm bài báo được viết, còn rất ít nghiên cứu sử dụng [[RTT]] kết hợp với [[Deep Learning|học sâu]]. 2727

### 3. Các loại Mạng Nơ-ron (Neural Networks)

- **[[ANN|Mạng Nơ-ron Nhân tạo (Artificial Neural Network - ANN)]]:**
  - Là loại cơ bản nhất, bao gồm các biến thể như Multi-layer Perceptron (MLP), Deep Neural Network (DNN), Back Propagation Neural Network (BPNN). 28282828
  - Thường được dùng để tìm ra ánh xạ trực tiếp từ dữ liệu WiFi số đến vị trí cụ thể. 29
- **[[Autoencoder|Mạng Tự mã hóa (Auto-Encoder - AE)]]:**
  - Là một mạng học không giám sát (unsupervised learning), gồm hai phần: bộ mã hóa (encoder) và bộ giải mã (decoder). 30
  - Mục tiêu là học một biểu diễn nén (compact representation) của dữ liệu đầu vào. 31
  - Thường dùng để trích xuất đặc trưng, giảm chiều dữ liệu và khử nhiễu. 32Các biến thể bao gồm Denoising AE (DAE), Stacked AE (SAE). 33
- **[[CNN|Mạng Nơ-ron Tích chập (Convolutional Neural Network - CNN)]]:**
  - Nổi tiếng trong lĩnh vực xử lý ảnh. 34
  - Sử dụng các lớp tích chập (convolutional layers) để trích xuất các đặc trưng phân cấp (hierarchical features) từ dữ liệu. 35
  - Trong định vị WiFi, dữ liệu tín hiệu thường được chuyển đổi thành dạng ảnh 2D hoặc vector 2D để làm đầu vào cho [[CNN]]. 36
  - **1D-CNN** là biến thể xử lý dữ liệu 1 chiều. 37
- **Mạng Nơ-ron Hồi quy (Recurrent Neural Network - RNN):**
  - Được thiết kế để xử lý dữ liệu dạng chuỗi (sequence data). 38
  - Rất phù hợp cho các bài toán theo dõi (tracking) chuyển động của người dùng dựa trên chuỗi tín hiệu WiFi thu thập theo thời gian. 39393939
  - **[[LSTM|Long Short-Term Memory (LSTM)]]** là một biến thể nâng cao của RNN, giải quyết vấn đề "quên" thông tin trong các chuỗi dài (vanishing gradient). 40
- **Các mạng khác:** Deep Belief Network (DBN), Generative Adversarial Network (GAN), Capsule Neural Network. 41

---

# Phương pháp và kỹ thuật

### Phân loại các hệ thống

Bài báo chia các công trình nghiên cứu thành hai nhóm chính để phân tích:

1. **[[Deep Learning|Học sâu]] làm phương pháp trích xuất đặc trưng (Feature Extraction):** Các mô hình DL ([[Autoencoder|AE]], [[CNN]],...) được dùng để học các biểu diễn dữ liệu hiệu quả hơn. Sau đó, một thuật toán khác (như [[KNN|k-NN]], SVM, hoặc các phương pháp xác suất) sẽ đưa ra dự đoán vị trí cuối cùng. 42424242
2. **[[Deep Learning|Học sâu]] làm giải pháp định vị (Positioning Solution):** Các mô hình DL được sử dụng trực tiếp để dự đoán vị trí, hoạt động như một bộ phân loại (classifier) hoặc một bộ hồi quy (regressor). 43434343

### Các chỉ số đánh giá (Evaluation Metrics)

Bài báo sử dụng một bộ chỉ số tiêu chuẩn để đánh giá và so sánh hiệu năng:

- **Tỷ lệ chính xác (Hitting Rate):** Dùng cho bài toán phân loại (dự đoán tòa nhà, tầng, hoặc vùng/lưới). 4444
  Hitting rate=tổng soˆˊ dự đoaˊnsoˆˊ dự đoaˊn đuˊng​×100%
  45
- **Lỗi khoảng cách trung bình (Mean Distance Error - MDE):** Dùng cho bài toán hồi quy (dự đoán tọa độ). Là giá trị trung bình của các lỗi khoảng cách Euclid. 46464646
  MDE=N1​i=1∑N​(x^i​−xi​)2+(y^​i​−yi​)2![](data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="400em" height="1.28em" viewBox="0 0 400000 1296" preserveAspectRatio="xMinYMin slice"><path d="M263,681c0.7,0,18,39.7,52,119%0Ac34,79.3,68.167,158.7,102.5,238c34.3,79.3,51.8,119.3,52.5,120%0Ac340,-704.7,510.7,-1060.3,512,-1067%0Al0 -0%0Ac4.7,-7.3,11,-11,19,-11%0AH40000v40H1012.3%0As-271.3,567,-271.3,567c-38.7,80.7,-84,175,-136,283c-52,108,-89.167,185.3,-111.5,232%0Ac-22.3,46.7,-33.8,70.3,-34.5,71c-4.7,4.7,-12.3,7,-23,7s-12,-1,-12,-1%0As-109,-253,-109,-253c-72.7,-168,-109.3,-252,-110,-252c-10.7,8,-22,16.7,-34,26%0Ac-22,17.3,-33.3,26,-34,26s-26,-26,-26,-26s76,-59,76,-59s76,-60,76,-60z%0AM1001 80h400000v40h-400000z"></path></svg>)​
  47
- **Sai số toàn phương trung bình gốc (Root Mean Squared Error - RMSE):** Cũng dùng cho bài toán hồi quy, là độ lệch chuẩn của các sai số. 48484848
  RMSE=N1​i=1∑N​[(x^i​−xi​)2+(y^​i​−yi​)2]![](data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="400em" height="3.3738em" viewBox="0 0 400000 3373" preserveAspectRatio="xMinYMin slice"><path d="M702 80H40000040%0AH742v3239l-4 4-4 4c-.667.7 -2 1.5-4 2.5s-4.167 1.833-6.5 2.5-5.5 1-9.5 1%0Ah-12l-28-84c-16.667-52-96.667 -294.333-240-727l-212 -643 -85 170%0Ac-4-3.333-8.333-7.667-13 -13l-13-13l77-155 77-156c66 199.333 139 419.667%0A219 661 l218 661zM702 80H400000v40H742z"></path></svg>)​
  49
- **Hàm phân phối tích lũy (Cumulative Distribution Function - CDF):** Biểu diễn xác suất mà lỗi định vị nhỏ hơn hoặc bằng một giá trị nhất định (ví dụ: 90% các dự đoán có lỗi nhỏ hơn 2 mét). 50505050
- **Độ phức tạp (Complexity):** Được đo bằng số lớp ẩn (number of hidden layers) của mạng nơ-ron. 51
- **Thời gian kiểm thử (Testing Time):** Thời gian cần thiết để hệ thống đưa ra một dự đoán cho một mẫu thử. 52

---

# Kết quả và số liệu

### Nhóm 1: Deep Learning làm phương pháp trích xuất đặc trưng

- **Phân loại (Classification):**
  - Hầu hết các hệ thống phân loại tầng đều dùng tín hiệu [[RSSI]]. 53
  - Tỷ lệ nhận dạng tầng (floor hitting rate) trung bình là
    **92.59%**. 54
  - Hệ thống của **Qi et al. [cite_start](https://www.google.com/search?q=2018&authuser=5)** đạt hiệu năng tốt nhất với tỷ lệ **98.69%**, sử dụng một tập hợp các mạng ELM (biến thể của [[ANN]]) và thuật toán bỏ phiếu đa số (majority voting). 55555555
- **Hồi quy (Regression):**
  - **So sánh tín hiệu đầu vào (MDE):**
    - Các hệ thống dựa trên
      **[[CSI]]** cho kết quả ổn định và chính xác hơn, với MDE trung bình là **1.43m**. 565656
    - Các hệ thống dựa trên
      **[[RSSI]]** có MDE trung bình là **1.96m**. 57Tuy nhiên, một số hệ thống [[RSSI]] được tinh chỉnh kỹ lưỡng hoặc kết hợp với các cảm biến khác (IMU, từ kế) có thể đạt độ chính xác dưới mét. 585858585858585858
  - **So sánh mô hình (MDE):**
    - **[[CNN]]** cho hiệu năng tốt nhất với MDE trung bình là **1.343m**. 59595959
    - **[[ANN]]** cũng rất hiệu quả với MDE trung bình là **1.607m** và chi phí tính toán thấp hơn. 60606060
  - **Kết quả nổi bật (độ chính xác dưới mét):**
    - **W. Zhang et al. [cite_start](https://www.google.com/search?q=2016&authuser=5)** sử dụng kết hợp DNN và SDAE với tín hiệu RSS đạt RMSE chỉ **0.339m**. 61616161
    - **Zhao et al. [cite_start](https://www.google.com/search?q=2019&authuser=5)** sử dụng CNN với tín hiệu CSI đạt MDE **0.46m** (trong môi trường có đường truyền thẳng - LoS). 62626262
    - **Belmonte-Hernández et al. [cite_start](https://www.google.com/search?q=2019&authuser=5)** kết hợp RSS với nhiều cảm biến khác (IMU, Bluetooth, XBee) và dùng ANN, đạt MDE **0.45m**. 63636363

### Nhóm 2: Deep Learning làm giải pháp định vị trực tiếp

- **Phân loại (Classification):**
  - **Nhận dạng tầng:** Các mạng **ANN** và **DBN** hoạt động tốt. Trong số 5 hệ thống có tỷ lệ chính xác trên 98%, có 3 hệ thống dùng ANN. 64646464
  - **Nhận dạng vùng (Zone):**
    - **Tín hiệu CSI** cho hiệu năng tốt và ổn định nhất (tỷ lệ chính xác trung bình **91.83%**). 65
    - **CNN** được xem là mô hình tốt nhất nói chung cho bài toán này (tỷ lệ chính xác trung bình sau khi lọc ngoại lệ là **93.26%**). 66666666
    - Hệ thống tốt nhất của **Adege, Yen, et al. (https://www.google.com/search?q=2018)** và **Koike-Akino et al. [cite_start](https://www.google.com/search?q=2020&authuser=5)** dùng ANN đạt tỷ lệ chính xác **100%**. 67
- **Hồi quy (Regression):**
  - **So sánh tín hiệu đầu vào (MDE):**
    - Hệ thống dùng
      **tín hiệu RSS lai (hybrid)** (kết hợp với cảm biến khác) cho kết quả tốt nhất, MDE trung bình sau khi lọc ngoại lệ là **1.25m**. 68
    - Hệ thống dùng
      **CSI** đứng thứ hai với MDE trung bình **1.47m**. 69
    - Trong các hệ thống CSI,
      **CSI biên độ (amplitude)** cho kết quả tốt hơn **CSI pha (phase)** (MDE trung bình 1.23m so với 1.71m). 70
  - **So sánh mô hình (MDE):**
    - **CNN** là mạng nơ-ron tốt nhất cho bài toán dự đoán tọa độ, với MDE trung bình là **1.871m**. 717171717171717171
  - **Kết quả nổi bật (độ chính xác dưới mét):**
    - **Koike-Akino et al. [cite_start](https://www.google.com/search?q=2020&authuser=5)** đạt kết quả ấn tượng nhất với RMSE chỉ **0.111m**, sử dụng tín hiệu **SNR** từ WiFi sóng milimet (mmWave) và một mạng DNN dựa trên ResNet. 72727272
    - **Xingli et al. [cite_start](https://www.google.com/search?q=2018&authuser=5)** kết hợp RSS, iBeacon, và dữ liệu địa từ, sử dụng DNN, đạt MDE **0.29m**. 73737373
    - **Vilović and Zovko-Cihlar (2005)**, một công trình rất sớm, đã đạt MDE **0.2m** chỉ với RSS và MLP. 74

---

# Đánh giá, ưu – nhược điểm

### Về tín hiệu WiFi

- **RSS:**
  - **Ưu điểm:** Dễ dàng truy cập, có sẵn trên mọi thiết bị, là công nghệ hữu ích. 7575757575
  - **Nhược điểm:** Độ chính xác trung bình, không ổn định. 76
  - **Cải tiến:** Hiệu năng được cải thiện đáng kể khi kết hợp với tín hiệu từ các cảm biến khác (IMU, từ kế) hoặc sử dụng các mô hình DL được tinh chỉnh kỹ lưỡng, có thể đạt độ chính xác dưới mét. 77777777
- **CSI:**
  - **Ưu điểm:** Cung cấp thông tin phong phú, ổn định và chính xác hơn RSS nhiều, là lựa chọn tốt nhất để đạt độ chính xác dưới mét. 7878787878787878
  - **Nhược điểm:** Khó thu thập trên các thiết bị thương mại (đặc biệt là smartphone) do hạn chế về phần cứng và driver. 79797979
- **RTT & SNR:**
  - **Ưu điểm:** Là các công nghệ mới và đầy hứa hẹn, có khả năng đạt độ chính xác rất cao. 80808080
  - **Nhược điểm:** Chưa có đủ nghiên cứu để đưa ra kết luận chắc chắn. 81818181

### Về các loại Mạng Nơ-ron

- **Mạng đơn giản (ANN, DBN):**
  - **Ưu điểm:** Hiệu quả về mặt tính toán, độ phức tạp thấp, cho độ chính xác ở mức chấp nhận được. 828282Phù hợp để triển khai trên các thiết bị có tài nguyên hạn chế như smartphone. 83
  - **Nhược điểm:** Khả năng trích xuất đặc trưng không mạnh bằng các mạng phức tạp hơn.
- **Mạng phức tạp (CNN):**
  - **Ưu điểm:** Khả năng trích xuất đặc trưng phân cấp rất mạnh, thường cho độ chính xác cao nhất, đặc biệt trong các bài toán hồi quy tọa độ. 848484848484848484
  - **Nhược điểm:** Yêu cầu tài nguyên tính toán lớn, khó triển khai trực tiếp trên smartphone. 85Phù hợp hơn với mô hình xử lý trên máy chủ từ xa. 86

**Kết luận:** Không có một giải pháp "tốt nhất" cho mọi trường hợp. Lựa chọn tối ưu phụ thuộc vào yêu cầu cụ thể của ứng dụng. Mạng đơn giản không phải lúc nào cũng kém hiệu quả hơn mạng phức tạp, đặc biệt khi xét đến chi phí tính toán. 87

---

# Thách thức và hướng cải tiến

- **Tích hợp phần cứng:** Việc thu thập tín hiệu CSI và RTT trên các thiết bị di động phổ thông vẫn là một thách thức lớn. 88888888
- **Thiếu dữ liệu chuẩn:** Thiếu một bộ dữ liệu công khai (public dataset) tiêu chuẩn và quy mô lớn cho tín hiệu CSI và RTT, gây khó khăn cho việc so sánh công bằng giữa các hệ thống. 898989898989898989
- **Tối ưu hóa mô hình:** Cần các phương pháp để tối ưu hóa và giảm độ phức tạp của các mô hình DL mạnh mẽ như CNN để chúng có thể chạy hiệu quả trên thiết bị di động.
- **Kết hợp đa cảm biến (Multi-sensor Fusion):** Kết hợp tín hiệu WiFi (đặc biệt là RSS) với dữ liệu từ các cảm biến khác có sẵn trên smartphone (IMU, từ kế, барометр) là một hướng đi rất tiềm năng để cải thiện độ chính xác mà không cần phần cứng chuyên dụng. 90909090
- **Khám phá công nghệ mới:** Cần thêm nhiều nghiên cứu về tiềm năng của RTT và SNR (từ WiFi mmWave) để khai thác hết khả năng của chúng. 91919191

---

# Ứng dụng thực tiễn

- **Dẫn đường trong nhà (Indoor Navigation):** Hỗ trợ người dùng tìm đường trong các không gian phức tạp như sân bay, trung tâm thương mại, bệnh viện, khuôn viên đại học. 92
- **Dịch vụ dựa trên vị trí (Location-Based Services - LBS):** Cung cấp quảng cáo, thông tin, hoặc dịch vụ tùy theo vị trí của người dùng.
- **Theo dõi tài sản và con người:** Giám sát vị trí của thiết bị y tế trong bệnh viện, robot tự hành trong nhà kho, hoặc nhân viên trong các khu vực lớn.
- **An ninh và khẩn cấp:** Xác định vị trí của người gọi cứu hộ trong một tòa nhà.

---

# Nhận xét tổng quan

Đây là một bài khảo sát rất chi tiết và có giá trị, cung cấp một cái nhìn toàn cảnh về lĩnh vực đang phát triển nhanh chóng là ứng dụng học sâu vào định vị trong nhà bằng WiFi.

- **Bài báo khẳng định:** Học sâu đã mang lại những tiến bộ vượt bậc so với các phương pháp truyền thống, với nhiều hệ thống đạt được độ chính xác dưới mét.
- **Không có giải pháp toàn năng:** Lựa chọn giữa tín hiệu (RSS, CSI) và kiến trúc mạng (ANN, CNN) là một sự đánh đổi giữa **độ chính xác** và **chi phí triển khai** (tài nguyên tính toán, sự phức tạp, yêu cầu phần cứng).
- **Hướng đi tương lai:**
  - **Thực tế & Gần gũi:** Một hệ thống dựa trên **RSS kết hợp với các cảm biến có sẵn trên smartphone** và sử dụng các **mạng nơ-ron đơn giản (như ANN)** là hướng đi khả thi và dễ triển khai nhất trong tương lai gần. 93
  - **Tối ưu & Chính xác cao:** Đối với các ứng dụng đòi hỏi độ chính xác cao nhất và có thể chấp nhận xử lý trên máy chủ, một hệ thống sử dụng **CNN** với tín hiệu **CSI (hoặc RTT trong tương lai)** sẽ là giải pháp tối ưu. 94
