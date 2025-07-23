# Thông tin bài báo

- **Tên bài báo:** Indoor Positioning Using WiFi Fingerprint (Định vị trong nhà sử dụng Vân tay WiFi) 1
- **Tác giả:** Ranimol Joseph 2, Swapna B Sasi 3
- **Tổ chức:** Khoa học Máy tính và Kỹ thuật, Trường Kỹ thuật Jyothi, Cheruthuruthy, Thrissur, Ấn Độ 4444
- **Năm xuất bản:** 2018 (©2018 IEEE) 5
- **Từ khóa:** [[Indoor Positioning System|Indoor Positioning System (Hệ thống định vị trong nhà)]], WiFi, [[WiFi Fingerprinting|Fingerprinting (Vân tay)]], [[Autoencoder|Stacked Autoencoder (Bộ tự mã hóa xếp chồng)]], [[ANN|Deep Neural Network (Mạng nơ-ron sâu)]] 6

# Mục tiêu nghiên cứu

Mục tiêu chính của bài báo là đề xuất một kỹ thuật [[Indoor Positioning System|định vị trong nhà]] bằng cách sử dụng phương pháp

**[[WiFi Fingerprinting|vân tay WiFi (WiFi fingerprinting)]]**. 7Cụ thể, nghiên cứu tập trung vào việc áp dụng một

**[[ANN|mạng nơ-ron sâu (Deep Neural Network - DNN)]]** với kiến trúc **[[Autoencoder|bộ tự mã hóa xếp chồng (Stacked Autoencoder - SAE)]]** để xác định vị trí tương đối của người dùng, bao gồm họ đang ở **tòa nhà nào** và **tầng nào**. 8

# Bối cảnh và động lực

- **Vấn đề:** Hệ thống Định vị Toàn cầu (Global Positioning System - GPS) hoạt động rất hiệu quả cho việc định vị ngoài trời nhưng lại mất tín hiệu khi ở trong các tòa nhà. 9999Do đó, [[Indoor Positioning System|định vị trong nhà (Indoor Positioning)]] vẫn là một bài toán đầy thách thức. 10
- **Động lực:** Sự phát triển mạnh mẽ của các thiết bị di động và thiết bị thông minh đã tạo ra nhu cầu lớn cho các ứng dụng theo dõi, giám sát người và vật thể trong nhà. 11
- **Lợi ích:**
  - Tìm kiếm những người bị mắc kẹt trong các tòa nhà khi có sự cố. 12121212
  - Giám sát bệnh nhân trong bệnh viện. 1313
  - Theo dõi nhân viên trong văn phòng để kiểm tra sự có mặt và phân tích mô hình làm việc nhằm nâng cao năng suất. 14

# Các khái niệm chính

- **[[Indoor Positioning System|Hệ thống Định vị trong nhà (Indoor Positioning System - IPS)]]:** Là hệ thống giúp xác định vị trí của người hoặc vật thể bên trong các công trình xây dựng bằng cách sử dụng các tín hiệu vô tuyến, từ trường hoặc các loại cảm biến khác. 15151515
- **[[WiFi Fingerprinting|Vân tay WiFi (WiFi Fingerprinting)]]:** Là một phương pháp định vị phổ biến, bao gồm hai giai đoạn:
  1. **[[Offline Phase|Giai đoạn Ngoại tuyến (Offline phase)]]:** Thu thập và ghi lại **[[RSSI|Cường độ Tín hiệu Thu được (Received Signal Strength - RSS)]]** từ các [[Access Points|điểm truy cập WiFi (Access Points)]] tại nhiều vị trí đã biết trước tọa độ. Dữ liệu này được lưu trữ trong một cơ sở dữ liệu, tạo thành một "[[Radio Map|bản đồ vân tay]]" tín hiệu. 161616
  2. **[[Online Phase|Giai đoạn Trực tuyến (Online phase)]]:** Thiết bị của người dùng quét mẫu [[RSSI|RSS]] tại vị trí hiện tại, sau đó tìm kiếm trong cơ sở dữ liệu để tìm ra mẫu "vân tay" tương đồng nhất và từ đó suy ra vị trí của người dùng. 17171717
- **[[RSSI|Cường độ Tín hiệu Thu được (Received Signal Strength - RSSI)]]:** Là thước đo cường độ của tín hiệu WiFi mà thiết bị nhận được từ một điểm truy cập. Trong nghiên cứu này, giá trị [[RSSI]] là các số âm, tính bằng dBm, dao động từ -104dBm (tín hiệu rất yếu) đến 0dBm (tín hiệu rất mạnh). 18181818Giá trị dương 100 được dùng để biểu thị rằng điểm truy cập đó không được phát hiện. 19191919
- **[[Autoencoder|Bộ tự mã hóa xếp chồng (Stacked Autoencoder - SAE)]]:** Là một mạng nơ-ron được tạo thành từ nhiều lớp **[[Autoencoder|bộ tự mã hóa (Autoencoder)]]**. Nó được sử dụng để học các đặc trưng (features) của dữ liệu đầu vào một cách không giám sát và giảm chiều dữ liệu. 20202020Trong bài báo, SAE được dùng để nén dữ liệu [[RSSI]] từ 520 chiều xuống một không gian nhỏ hơn. 2121
- **[[ANN|Mạng nơ-ron sâu (Deep Neural Network - DNN)]]:** Là mạng nơ-ron nhân tạo có nhiều lớp ẩn (hidden layers) nằm giữa lớp đầu vào (input layer) và lớp đầu ra (output layer). 22

# Phương pháp và kỹ thuật

Hệ thống được xây dựng dựa trên phương pháp [[WiFi Fingerprinting|vân tay WiFi]] và mô hình [[Deep Learning|học sâu]].

### 1. Kiến trúc tổng thể

Hệ thống bao gồm các bước:

1. **Thu thập tín hiệu:** Thiết bị người dùng quét và ghi nhận tín hiệu WiFi từ các [[Access Points|điểm truy cập (Access Points)]] xung quanh. 2323
2. **Xây dựng cơ sở dữ liệu vân tay:** Ở [[Offline Phase|giai đoạn ngoại tuyến]], cường độ tín hiệu ([[RSSI]]) tại các vị trí cụ thể được đo đạc và lưu vào cơ sở dữ liệu cùng với thông tin vị trí (tòa nhà, tầng). 24242424
3. **Xác định vị trí:** Ở [[Online Phase|giai đoạn trực tuyến]], mô hình sẽ nhận dữ liệu [[RSSI]] hiện tại và dự đoán vị trí dựa trên cơ sở dữ liệu đã huấn luyện. 25

### 2. Mô hình học máy

Mô hình chính là một **[[ANN|Mạng Nơ-ron Sâu (DNN)]]** sử dụng **[[Autoencoder|Bộ tự mã hóa xếp chồng (SAE)]]**, được huấn luyện qua hai giai đoạn:

- **Giai đoạn 1: Tiền huấn luyện không giám sát (Unsupervised Pre-training)**
  - **Mục đích:** Giảm chiều dữ liệu và trích xuất các đặc trưng hữu ích từ tín hiệu [[RSSI]].
  - **Kiến trúc:** Một [[Autoencoder|bộ tự mã hóa (Autoencoder)]] được sử dụng.
    - **Đầu vào (Encoder Input):** Vector 520 giá trị [[RSSI]] từ các [[Access Points|điểm truy cập WiFi]]. 26262626
    - **Đầu ra (Decoder Output):** Vector [[RSSI]] được tái tạo lại, có cùng kích thước 520. 27272727
  - **Huấn luyện:** Mô hình SAE được huấn luyện để tái tạo đầu vào một cách chính xác nhất có thể (giảm thiểu lỗi giữa tín hiệu gốc và tín hiệu tái tạo). 28
- **Giai đoạn 2: Tinh chỉnh có giám sát (Supervised Fine-tuning)**
  - Sau khi tiền huấn luyện, phần
    **bộ giải mã (decoder)** của SAE được loại bỏ. 29
  - Phần
    **bộ mã hóa (encoder)** đã được huấn luyện được giữ lại và kết nối với một **bộ phân loại (classifier)** ở lớp đầu ra. 30
  - Toàn bộ mạng (encoder + classifier) sau đó được huấn luyện trên dữ liệu có nhãn (dữ liệu [[RSSI]] kèm theo thông tin tòa nhà và tầng) để có thể dự đoán chính xác vị trí. 31313131

### 3. Tập dữ liệu (Dataset)

- **Tên:** [[UJIIndoorLoc Dataset]]. 32323232
- **Quy mô:** Gồm 21.048 mẫu đo WiFi, trong đó có 19.937 mẫu cho huấn luyện (training) và 1.111 mẫu cho kiểm định (validation). 33Dữ liệu được thu thập từ 25 thiết bị Android khác nhau. 34
- **Thuộc tính:** Mỗi mẫu có 529 thuộc tính: 35
  - **520 thuộc tính đầu tiên:** Là giá trị [[RSSI]] của 520 [[Access Points|điểm truy cập WiFi (WAP)]]. 36
  - **9 thuộc tính còn lại:** Kinh độ, vĩ độ, ID tòa nhà, ID tầng, ID không gian, vị trí tương đối, ID người dùng, ID điện thoại và dấu thời gian (timestamp). 37

# Kết quả và số liệu

Mô hình được huấn luyện trong 20 kỷ nguyên (epochs). 38 Bảng dưới đây thể hiện giá trị hàm mất mát (loss) và độ chính xác (accuracy) trên

**tập dữ liệu huấn luyện** qua từng kỷ nguyên.

**Bảng 1: Giá trị Loss và Accuracy của mạng trên tập huấn luyện** 39

| Epoch | Loss | Accuracy |

| :--- | :--- | :--- |

| 1 | 0.3145 | 0.8850 (88.50%) |

| 2 | 0.1361 | 0.9541 (95.41%) |

| 3 | 0.1056 | 0.9640 (96.40%) |

| ... | ... | ... |

| 19 | 0.0361 | 0.9870 (98.70%) |

| 20 | 0.0389 | 0.9868 (98.68%) |

- **Độ chính xác tổng thể:** Bài báo kết luận rằng mạng đạt độ chính xác **khoảng 93%** sau 20 kỷ nguyên. 40
  - _Lưu ý:_ Con số 93% có thể là độ chính xác trên tập kiểm định (validation set), là thước đo hiệu năng thực tế của mô hình. Trong khi đó, bảng trên cho thấy độ chính xác trên tập huấn luyện lên tới 98.7%.

# Đánh giá, ưu – nhược điểm

### Ưu điểm

- **Chi phí thấp:** Tận dụng được hạ tầng mạng WiFi có sẵn mà không cần lắp đặt thêm thiết bị chuyên dụng. 41
- **Hiệu quả:** Mô hình [[ANN|DNN]] cho thấy hiệu suất cao trong việc xác định đúng tòa nhà và tầng, với độ chính xác khoảng 93%. 42
- **Không cần phần cứng đặc biệt:** Chỉ cần một thiết bị di động có khả năng bắt sóng WiFi.

### Nhược điểm

- **Chưa định vị chính xác:** Hệ thống chỉ xác định được vị trí tương đối (tòa nhà, tầng) chứ chưa xác định được tọa độ (x, y) chính xác của người dùng. 43
- **Tốn công thu thập dữ liệu:** Quá trình xây dựng cơ sở dữ liệu vân tay ở giai đoạn ngoại tuyến đòi hỏi nhiều thời gian và công sức đi lại để đo đạc tín hiệu. 44

# Thách thức và hướng cải tiến

- **Thách thức:** [[Indoor Positioning System|Định vị trong nhà]] là một bài toán phức tạp và chưa có giải pháp toàn cầu nào phù hợp cho mọi ứng dụng. 45
- **Hướng cải tiến (Future Work):** Các tác giả đề xuất hướng phát triển trong tương lai là cải tiến hệ thống để có thể **xác định vị trí chính xác** (tọa độ cụ thể) của người dùng, thay vì chỉ dừng lại ở vị trí tương đối. 46

# Ứng dụng thực tiễn

- **An toàn và Cứu hộ:** Xác định vị trí người bị nạn bên trong các tòa nhà. 47474747
- **Y tế:** Theo dõi và giám sát vị trí của bệnh nhân trong các cơ sở y tế lớn. 4848
- **Quản lý doanh nghiệp:** Giám sát sự hiện diện của nhân viên, phân tích luồng di chuyển trong văn phòng để tối ưu hóa không gian và năng suất làm việc. 49494949

# Nhận xét tổng quan

Đây là một bài báo trình bày một cách tiếp cận chuẩn mực và hiệu quả cho bài toán [[Indoor Positioning System|định vị trong nhà]]. Việc kết hợp phương pháp **[[WiFi Fingerprinting|vân tay WiFi]]** cổ điển với kỹ thuật **[[Deep Learning|học sâu (Deep Learning)]]** hiện đại là điểm nhấn chính, cho thấy tiềm năng lớn của AI trong việc giải quyết các vấn đề kỹ thuật thực tiễn.

Mô hình sử dụng SAE để giảm chiều dữ liệu [[RSSI]] là một kỹ thuật thông minh và phù hợp. Kết quả đạt được rất khả quan cho tác vụ phân loại (xác định tầng và tòa nhà). Tuy nhiên, nghiên cứu vẫn còn một hạn chế lớn là chưa giải quyết được bài toán hồi quy (regression) để ước tính tọa độ chính xác, và đây cũng là hướng phát triển mà chính các tác giả đã chỉ ra.
