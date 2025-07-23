# WiFi Fingerprinting

**WiFi Fingerprinting** là một phương pháp [[Indoor Positioning System|định vị trong nhà]] phổ biến, sử dụng đặc trưng tín hiệu WiFi để xác định vị trí.

## Nguyên lý hoạt động

WiFi Fingerprinting dựa trên nguyên lý rằng mỗi vị trí trong không gian có một "dấu vân tay" tín hiệu WiFi đặc trưng, được tạo ra bởi:

- **Đa đường (Multipath):** Tín hiệu phản xạ từ tường, vật thể
- **Suy hao (Attenuation):** Tín hiệu suy giảm qua vật liệu
- **Nhiễu (Interference):** Ảnh hưởng từ các nguồn tín hiệu khác

## Quy trình hai giai đoạn

### [[Offline Phase]] - Giai đoạn Ngoại tuyến

1. **Khảo sát môi trường:** Xác định các [[Reference Points]]
2. **Thu thập dữ liệu:** Đo [[RSSI]] từ các [[Access Points]]
3. **Xây dựng [[Radio Map]]:** Lưu trữ dữ liệu vân tay
4. **Tiền xử lý:** Làm sạch và chuẩn hóa dữ liệu

### [[Online Phase]] - Giai đoạn Trực tuyến

1. **Đo tín hiệu hiện tại:** Thu thập [[RSSI]] thời gian thực
2. **So khớp mẫu:** Tìm vân tay tương tự trong [[Radio Map]]
3. **Ước tính vị trí:** Sử dụng thuật toán [[Machine Learning]]

## Thuật toán phổ biến

### Truyền thống

- **[[KNN|k-Nearest Neighbors]]:** Tìm k vân tay gần nhất
- **Weighted k-NN:** Có trọng số theo khoảng cách
- **Support Vector Machine (SVM)**
- **Naive Bayes**

### Hiện đại ([[Deep Learning]])

- **[[ANN|Artificial Neural Networks]]**
- **[[CNN|Convolutional Neural Networks]]**
- **[[LSTM|Long Short-Term Memory]]**
- **[[Autoencoder|Autoencoders]]**

## Loại tín hiệu

### [[RSSI]] (Received Signal Strength Indicator)

- **Ưu điểm:** Dễ thu thập, phổ biến
- **Nhược điểm:** Không ổn định, nhiễu cao

### [[CSI]] (Channel State Information)

- **Ưu điểm:** Chi tiết hơn, ổn định hơn
- **Nhược điểm:** Khó thu thập, cần phần cứng chuyên dụng

### [[RTT]] (Round Trip Time)

- **Ưu điểm:** Đo khoảng cách trực tiếp
- **Nhược điểm:** Công nghệ mới, ít thiết bị hỗ trợ

## Ưu điểm

- ✅ **Chi phí thấp:** Tận dụng hạ tầng WiFi có sẵn
- ✅ **Không cần phần cứng thêm:** Sử dụng smartphone thông thường
- ✅ **Độ chính xác khả quan:** 1-3 mét trong điều kiện tốt
- ✅ **Phủ sóng rộng:** WiFi có mặt ở hầu hết các tòa nhà

## Nhược điểm

- ❌ **Không ổn định:** Tín hiệu thay đổi theo thời gian
- ❌ **Ảnh hưởng môi trường:** Người di chuyển, thay đổi nội thất
- ❌ **Tốn công thu thập:** Giai đoạn offline tốn thời gian
- ❌ **Bảo trì liên tục:** Cần cập nhật [[Radio Map]]

## Thách thức nghiên cứu

### Thu thập dữ liệu

- **Crowdsourcing:** Tận dụng dữ liệu từ cộng đồng
- **Robot/UAV:** Thu thập tự động
- **SLAM:** Xây dựng bản đồ đồng thời

### Xử lý dữ liệu

- **Data augmentation:** Tăng cường dữ liệu
- **Transfer learning:** Học chuyển giao
- **Federated learning:** Học liên kết

### Cải thiện độ chính xác

- **Sensor fusion:** Kết hợp với IMU, từ kế
- **Multi-modal:** Kết hợp nhiều loại tín hiệu
- **Context awareness:** Nhận biết ngữ cảnh

## Tài liệu tham khảo

- [[A Review of Open Access WiFi Fingerprinting Datasets for Indoor Positioning]]
- [[A survey of deep learning approaches for WIFI-based indoor positioning]]
- [[Indoor Localization with WiFi Fingerprinting Using Convolutional Neural Network]]
- [[Indoor Positioning Using WiFi Fingerprint]]
- [[Machine Learning Based Indoor Localization Using Wi-Fi RSSI Fingerprints - An Overview]]
