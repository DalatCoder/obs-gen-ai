# Ghi Chú Học Tập: Sử Dụng Ví Dụ Trong Prompting

## Giới Thiệu

Bạn đã từng tạo ra thứ gì đó mới bằng cách xây dựng dựa trên ví dụ trước đó, như sử dụng báo cáo thành công làm tham chiếu hoặc mô hình website hấp dẫn để thiết kế website của mình. Ví dụ cũng hữu ích cho mô hình ngôn ngữ lớn (LLMs). Bao gồm ví dụ trong prompt giúp LLM phản hồi tốt hơn với yêu cầu, đặc biệt hiệu quả để đạt đầu ra mong muốn.

## Khái Niệm "Shot" Trong Kỹ Thuật Thiết Kế Prompt

Trong kỹ thuật thiết kế prompt (prompt engineering), "shot" thường đồng nghĩa với "example" (ví dụ). Các kỹ thuật prompting được đặt tên dựa trên số lượng ví dụ cung cấp cho LLM:

- Zero-shot prompting: Kỹ thuật không cung cấp ví dụ nào trong prompt.
    
- One-shot prompting: Cung cấp một ví dụ.
    
- Few-shot prompting: Kỹ thuật cung cấp hai hoặc nhiều ví dụ trong prompt.
    

## Zero-Shot Prompting

Zero-shot prompting không bao gồm ví dụ, nên mô hình dựa chỉ vào dữ liệu huấn luyện và mô tả nhiệm vụ trong prompt. Kỹ thuật này hiệu quả nhất cho phản hồi đơn giản và trực tiếp, nhưng không phù hợp cho nhiệm vụ yêu cầu phản hồi cụ thể, tinh tế hơn.

## Few-Shot Prompting

Few-shot prompting cải thiện hiệu suất LLM bằng cách cung cấp ngữ cảnh và ví dụ bổ sung trong prompt, giúp làm rõ định dạng, cách diễn đạt hoặc mẫu chung. Kỹ thuật này hữu ích cho nhiều nhiệm vụ, như tạo nội dung theo phong cách cụ thể.

## Ví Dụ: Tạo Mô Tả Sản Phẩm

Giả sử bạn làm việc cho nhà bán lẻ trực tuyến và cần viết mô tả cho ván trượt (skateboard) theo phong cách tương tự mô tả xe đạp và giày trượt patin.

**Prompt mẫu (giữ nguyên tiếng Anh):**  
Write a one-sentence description of a product. It should contain two adjectives that describe the product. Review the examples we provide, and write the description of the skateboard in the same style.

Bicycle: Whether you’re exploring city streets or forest paths, our sleek and durable bicycle has it all.

Rollerblades: Roll into summer in style with our smooth and stylish rollerblades.

Skateboard:

(Dịch: Viết mô tả sản phẩm một câu. Nó nên chứa hai tính từ mô tả sản phẩm. Xem xét các ví dụ chúng tôi cung cấp, và viết mô tả cho skateboard theo phong cách tương tự.

Bicycle: Dù bạn đang khám phá đường phố thành phố hay lối rừng, chiếc xe đạp mượt mà và bền bỉ của chúng tôi có tất cả.

Rollerblades: Lăn vào mùa hè phong cách với đôi giày trượt patin mượt mà và stylish của chúng tôi.

Skateboard:)

Prompt bắt đầu bằng hướng dẫn chung, chỉ định xem xét ví dụ và viết mô tả skateboard theo phong cách tương tự. Mỗi ví dụ có nhãn sản phẩm, mô tả một câu với hai tính từ (ví dụ: "sleek" và "durable" cho bicycle).

## Đánh Giá Đầu Ra

Đầu ra cung cấp mô tả skateboard phù hợp tiêu chí, theo phong cách và định dạng của ví dụ. Trong trường hợp này, hai ví dụ đủ để có kết quả hữu ích.

## Lời Khuyên Về Số Lượng Ví Dụ

Không có quy tắc cố định về số lượng ví dụ tối ưu. Một số LLM tái tạo mẫu chính xác với ít ví dụ, trong khi khác cần nhiều hơn. Nếu quá nhiều ví dụ, phản hồi có thể kém linh hoạt, sáng tạo và sao chép quá sát. Hãy thử nghiệm số lượng để có kết quả tốt nhất cho nhiệm vụ cụ thể.

## Kết Luận

Few-shot prompting là kỹ thuật hiệu quả giúp hướng dẫn LLM tạo phản hồi hữu ích hơn.