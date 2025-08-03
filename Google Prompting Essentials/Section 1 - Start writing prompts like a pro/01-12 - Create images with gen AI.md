## Tạo hình ảnh với AI sinh tạo

### Khái niệm về modalities (phương thức)

**[[Modalities]]** (phương thức) là các định dạng khác nhau mà các công cụ AI sinh tạo nhận hoặc tạo ra thông tin:

- **Text** (văn bản)
- **Images** (hình ảnh)
- **Video** (video)
- **Audio** (âm thanh)
- **Code** (mã nguồn)

**Lưu ý quan trọng:**

- Các công cụ [[Gen AI]] khác nhau có khả năng làm việc tốt hơn với những modalities nhất định
- Cần kiểm tra công cụ AI bạn đang sử dụng để biết nó có khả năng sử dụng hoặc tạo ra modalities nào


### So sánh prompting text và image

#### Prompting cho text

Sử dụng khung **[[TCREI Framework]]** (Thoughtfully Create Really Excellent Inputs):

**Ví dụ prompt text:**

```
Tạo tiêu đề cho poster quảng cáo concert rock ở New Orleans. Concert chỉ diễn ra một đêm duy nhất, và tiêu đề nên khuyến khích khán giả đừng bỏ lỡ.
```

**Kết quả mẫu:** "NOLA. This is it: Unforgettable Rock, One Night Only"

#### Prompting cho image

Cần **điều chỉnh ngôn ngữ** với mô tả sinh động hơn:

**Yêu cầu bổ sung:**

- Kích thước, màu sắc, vị trí của các vật thể trong hình
- Thẩm mỹ tổng thể mong muốn
- Mô tả chi tiết và cụ thể


### Ví dụ thực hành: Tạo poster concert

#### Prompt image cơ bản:

```
Tạo hình ảnh một cây guitar điện cho poster. Phong cách chụp ảnh (photographic style). Guitar nên lấp lánh hoặc sáng bóng và tạo cảm giác phấn khích. Guitar nên ở tiền cảnh và tạo cảm giác như đang lơ lửng trên bầu trời.
```


#### Kỹ thuật iterate và refine

**Bước 1:** Đánh giá kết quả ban đầu

- Gemini tạo ra 4 hình ảnh khác nhau để lựa chọn

**Bước 2:** Refine prompt để cải thiện

```
Bây giờ, làm cho bầu trời có bão với sét đánh vào guitar.
```

**Bước 3:** Tiếp tục iterate

- Có thể giữ hình ảnh hiện tại hoặc tiếp tục đánh giá và lặp lại
- Thêm chi tiết liên quan từ mỗi kết quả mới cho đến khi có hình phù hợp


### Nguyên tắc quan trọng

**Framework cho image generation:**

- Vẫn sử dụng khung [[TCREI]] nhưng có một số điều chỉnh
- **Task và Format:** Chỉ định rõ loại hình ảnh và phong cách
- **Vivid Descriptions:** Mô tả sinh động về kích thước, màu sắc, vị trí, thẩm mỹ
- **Context:** Cung cấp bối cảnh sử dụng
- **Iterate:** Liên tục cải thiện dựa trên kết quả

**Quy trình làm việc:**

1. Prompt cơ bản với mô tả rõ ràng
2. Đánh giá kết quả
3. Refine prompt với chi tiết bổ sung
4. Lặp lại cho đến khi đạt kết quả mong muốn

**Liên kết:** [[Modalities]], [[Gen AI]], [[TCREI Framework]], [[Image Generation]], [[Prompt Engineering]], [[Visual Communication]]

