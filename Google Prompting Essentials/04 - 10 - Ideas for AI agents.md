# Ý tưởng về AI Agents - Đại lý Trí tuệ Nhân tạo

## Giới thiệu về AI Agents

Điều gì sẽ xảy ra nếu bạn có thể biến công cụ trí tuệ nhân tạo tạo sinh (Gen AI) thành đội ngũ chuyên gia riêng, sẵn sàng giúp bạn đối phó với mọi thử thách? Điều gì sẽ xảy ra nếu họ nhanh chóng, sáng tạo và có khả năng nhập vai thông qua tất cả các tình huống để giúp bạn trong công việc? Thực tế, không cần "điều gì sẽ xảy ra" - đó chính là những gì **AI agent** (đại lý AI) được thiết kế để làm.

Bạn có thể tạo một AI agent để giúp bạn với bất kỳ điều gì bạn cần, từ viết bài phát biểu đến học về lập trình. Ở đây, bạn sẽ học cách tạo ra agent riêng và bắt đầu làm việc thông minh hơn.

## Thiết kế AI Agents

Để tạo một agent, bạn sẽ tạo prompt cho công cụ trí tuệ nhân tạo tạo sinh (Gen AI) như bình thường, tuân theo khung prompting framework, nhưng bạn sẽ **tập trung vào persona và context hơn bao giờ hết**. Càng bao gồm nhiều chi tiết về những gì bạn muốn AI agent làm và cách bạn muốn nó phản hồi, nó sẽ càng hiệu quả.

## Cách tạo AI Agent (5 bước cơ bản):

1. **Gán persona** (nhân cách) mà bạn muốn công cụ trí tuệ nhân tạo tạo sinh (Gen AI) đảm nhận
    
    - **Ví dụ:** `Act like a successful personal fitness trainer and talented nutritionist.`
        
    - _(Hãy đóng vai như một huấn luyện viên thể dục cá nhân thành công và chuyên gia dinh dưỡng tài năng.)_
        
2. **Cung cấp context** (ngữ cảnh) và chi tiết về tình huống và cuộc trò chuyện
    
    - **Ví dụ:** `I'm looking to improve my overall fitness and adopt a healthier lifestyle.`
        
    - _(Tôi đang tìm cách cải thiện thể lực tổng thể và áp dụng lối sống lành mạnh hơn.)_
        
3. **Chỉ định loại cuộc trò chuyện** hoặc các loại tương tác bạn muốn công cụ hỗ trợ, và thiết lập một số "quy tắc" cho AI agent tuân theo
    
    - **Ví dụ:** `Ask me about my workout routines and meal planning and give me feedback.`
        
    - _(Hỏi tôi về lịch trình tập luyện và lập kế hoạch bữa ăn và cho tôi phản hồi.)_
        
4. **Cung cấp cụm từ dừng** (stop phrase) bạn có thể sử dụng để kết thúc cuộc trò chuyện
    
    - **Ví dụ:** `When I want the conversation to end, I'll write, 'no pain, no gain.'`
        
    - _(Khi tôi muốn kết thúc cuộc trò chuyện, tôi sẽ viết, 'no pain, no gain.')_
        
5. **Yêu cầu công cụ cung cấp điểm chính** (takeaways) hoặc các lĩnh vực cải thiện sau khi cuộc trò chuyện kết thúc
    
    - **Ví dụ:** `At the end of our conversation, provide a summary of the advice you provided.`
        
    - _(Cuối cuộc trò chuyện, hãy cung cấp tóm tắt lời khuyên bạn đã đưa ra.)_
        

## Ứng dụng AI Agents

Bạn đã biết những gì cần có trong prompt để tạo AI agent, và trước đó, bạn đã học về hai ví dụ về cách sử dụng chúng: **AgentSim** và **AgentX**. Bây giờ, bạn sẽ khám phá thêm một vài tình huống khác cho AI agents mà bạn có thể thấy thực sự hữu ích trong công việc hoặc cuộc sống cá nhân.

## 1. Luyện tập kỹ năng (Practice Skills)

Bạn có bao giờ muốn cải thiện kỹ năng nói trước công chúng không? Hoặc luyện tập một cuộc trò chuyện khó khăn mà bạn định tiến hành? AI agents có thể giúp bằng cách đóng vai **digital coach** (huấn luyện viên kỹ thuật số) có thể cho bạn phản hồi về nhiều tình huống khác nhau và xây dựng kỹ năng của bạn trong quá trình này.

**Ví dụ cụ thể:** Bạn là một freelance web developer muốn cải thiện kỹ năng đàm phán để chốt được nhiều deal hơn, xây dựng mối quan hệ mạnh mẽ hơn, và đảm bảo mức giá và điều khoản tốt hơn.

**Prompt mẫu:**

text

`I'm a freelance web developer. I want to brush up on my negotiation skills so I can demand higher rates, establish clear project boundaries, and create mutually beneficial relationships with my clients. Take on the persona of a seasoned business consultant with serious expertise in negotiation strategies for freelance web developers. I'd like you to assess and improve my negotiation skills by roleplaying with me through example negotiation scenarios that I might encounter at work and practical exercises, providing industry-specific advice and feedback as I respond. When I want to end the roleplay, I'll write "I'm finished." When our conversation is over, provide me with a list of personalized, actionable ways I can improve my negotiation skills.`

_(Tôi là một freelance web developer. Tôi muốn cải thiện kỹ năng đàm phán để có thể đòi hỏi mức giá cao hơn, thiết lập ranh giới dự án rõ ràng, và tạo mối quan hệ cùng có lợi với khách hàng. Hãy đóng vai một tư vấn kinh doanh dày dạn kinh nghiệm với chuyên môn sâu về chiến lược đàm phán cho freelance web developers. Tôi muốn bạn đánh giá và cải thiện kỹ năng đàm phán của tôi bằng cách nhập vai với tôi thông qua các tình huống đàm phán mẫu mà tôi có thể gặp phải trong công việc và các bài tập thực hành, cung cấp lời khuyên và phản hồi cụ thể theo ngành khi tôi phản hồi. Khi tôi muốn kết thúc nhập vai, tôi sẽ viết "I'm finished." Khi cuộc trò chuyện kết thúc, hãy cung cấp danh sách các cách cá nhân hóa, có thể thực hiện được để tôi cải thiện kỹ năng đàm phán.)_

## 2. Nhận phản hồi cụ thể (Get Specific Feedback)

AI agent có thể đưa ra gợi ý và khuyến nghị cho một nhiệm vụ cụ thể. Ví dụ, bạn có thể tạo một AI agent đóng vai **editor** (biên tập viên) và giúp bạn thay đổi hoặc cải thiện một tác phẩm viết của bạn, cung cấp phản hồi về phong cách, định dạng, giọng điệu và nhiều hơn nữa.

**Tình huống:** Bạn muốn gửi một tác phẩm viết cho tạp chí. Trước khi gửi, AI agent có thể cung cấp phê bình và gợi ý.

**Lưu ý quan trọng:** Tùy thuộc vào lượng văn bản bạn muốn đưa vào (độ dài tài liệu cần phê bình), bạn có thể cần một công cụ trí tuệ nhân tạo tạo sinh (Gen AI) với **long context window** (cửa sổ ngữ cảnh dài), cho phép xử lý một lượng lớn thông tin ở các định dạng khác nhau cùng một lúc.

**Prompt mẫu:**

text

`I'm submitting a creative writing piece to a literary magazine for a prize. The magazine is known for its fantasy and sci-fi content. The judges are accomplished fantasy writers and will be choosing a winner based on worldbuilding, originality, and technical skill.  Take on the persona of one of the magazine's judges and critique my piece through the lens of those key areas. Provide suggestions for changes and improvements to further meet the competition criteria.  The stop phrase will be "I'm ready to submit." Attached are the submission and judging guidelines, a reference piece that won the prize last year, and my story: [upload documents].`

_(Tôi đang gửi một tác phẩm viết sáng tạo cho tạp chí văn học để tham gia giải thưởng. Tạp chí nổi tiếng với nội dung fantasy và sci-fi. Các giám khảo là những nhà văn fantasy thành đạt và sẽ chọn người chiến thắng dựa trên việc xây dựng thế giới, tính nguyên bản và kỹ năng kỹ thuật. Hãy đóng vai một trong những giám khảo của tạp chí và phê bình tác phẩm của tôi qua lăng kính của những lĩnh vực chính đó. Cung cấp gợi ý về những thay đổi và cải tiến để đáp ứng hơn nữa tiêu chí cuộc thi. Cụm từ dừng sẽ là "I'm ready to submit." Đính kèm là hướng dẫn nộp bài và chấm điểm, một tác phẩm tham khảo đã thắng giải năm ngoái, và câu chuyện của tôi: [tải tài liệu lên].)_

## 3. Học điều gì đó mới (Learn Something New)

AI agent có thể giúp bạn học thêm về một chủ đề xa lạ hoặc thậm chí giúp bạn học một kỹ năng hoàn toàn mới bằng cách đóng vai một chuyên gia.

**Tình huống:** Bạn có khách hàng nói tiếng Tây Ban Nha và muốn học ngôn ngữ này để xây dựng mối quan hệ tốt hơn và hợp tác chặt chẽ hơn với họ trong các dự án.

**Prompt mẫu:**

text

`I'm trying to learn Spanish to better communicate with my clients who live in Guatemala. Take on the persona of a skilled Spanish tutor and help me learn Spanish. I want you to teach me Spanish by delivering increasingly difficult lessons, crafting educational activities and scenarios, chatting with me in Spanish, and quizzing me. Correct my errors when I respond and call out areas of improvement. Provide feedback in English only. When I want to end the lesson, I'll write "adios." After we finish our conversation, provide me with a personalized list of vocabulary words, conjugations, and tips I should study to become a better Spanish speaker.`

_(Tôi đang cố gắng học tiếng Tây Ban Nha để giao tiếp tốt hơn với khách hàng sống ở Guatemala. Hãy đóng vai một gia sư tiếng Tây Ban Nha lành nghề và giúp tôi học tiếng Tây Ban Nha. Tôi muốn bạn dạy tôi tiếng Tây Ban Nha bằng cách cung cấp các bài học khó dần, tạo các hoạt động giáo dục và tình huống, trò chuyện với tôi bằng tiếng Tây Ban Nha, và kiểm tra tôi. Sửa lỗi của tôi khi tôi phản hồi và chỉ ra các lĩnh vực cần cải thiện. Chỉ cung cấp phản hồi bằng tiếng Anh. Khi tôi muốn kết thúc bài học, tôi sẽ viết "adios." Sau khi chúng ta kết thúc cuộc trò chuyện, hãy cung cấp danh sách cá nhân hóa các từ vựng, liên từ và mẹo tôi nên học để trở thành người nói tiếng Tây Ban Nha tốt hơn.)_

## 4. Hợp tác trong dự án (Collaborate on a Project)

Trong khi AI agents tuyệt vời trong việc giúp đỡ với các mục tiêu và nhiệm vụ rộng lớn, chúng cũng tuyệt vời trong việc tập trung vào các mục cụ thể mà bạn cần hoàn thành trong danh sách việc cần làm.

**Tình huống:** Bạn là một nhà nghiên cứu quy hoạch đô thị tìm kiếm tài trợ bổ sung cho một dự án mới.

**Prompt mẫu:**

text

`I'm a city planning researcher seeking a grant for a revitalization project. I need assistance crafting a compelling and competitive grant proposal. Take on the persona of an experienced grant writer with expertise in revitalization grants and act as my collaborative partner. Let's work together on the proposal, brainstorming ideas, refining the language, and ensuring it aligns with the grant's requirements and evaluation criteria. We'll focus on developing the following key components: Project Summary: A concise and engaging overview of the project's purpose, goals, and expected outcomes Project Description: A detailed explanation of the project's activities, methodology, and timeline Budget breakdown: A comprehensive and itemized budget, justifying each expense and demonstrating financial responsibility As I write each section with you, provide insights for how to strengthen them, making sure my work is clear, persuasive, and impactful. The goal is for the proposal to align with the funder's priorities and showcase the project's potential for significant impact. When I want to end our session, I'll write "We're done." After our conversation ends, provide a list of takeaways and learnings from our working session that I can consider next time I write a revitalization grant. Here is information about the grant and its evaluation criteria: [upload document].`

_(Tôi là một nhà nghiên cứu quy hoạch đô thị đang tìm kiếm tài trợ cho một dự án phục hồi. Tôi cần hỗ trợ tạo một đề xuất tài trợ hấp dẫn và cạnh tranh. Hãy đóng vai một nhà viết tài trợ có kinh nghiệm với chuyên môn về tài trợ phục hồi và đóng vai đối tác hợp tác của tôi. Hãy cùng nhau làm việc trên đề xuất, động não ý tưởng, tinh chỉnh ngôn ngữ, và đảm bảo nó phù hợp với các yêu cầu và tiêu chí đánh giá của tài trợ. Chúng ta sẽ tập trung phát triển các thành phần chính sau: Tóm tắt dự án: Tổng quan ngắn gọn và hấp dẫn về mục đích, mục tiêu và kết quả mong đợi của dự án; Mô tả dự án: Giải thích chi tiết về các hoạt động, phương pháp và thời gian của dự án; Phân tích ngân sách: Ngân sách toàn diện và chi tiết, biện minh cho từng chi phí và thể hiện trách nhiệm tài chính. Khi tôi viết từng phần với bạn, hãy cung cấp hiểu biết về cách củng cố chúng, đảm bảo công việc của tôi rõ ràng, thuyết phục và có tác động. Mục tiêu là để đề xuất phù hợp với ưu tiên của nhà tài trợ và thể hiện tiềm năng tác động đáng kể của dự án. Khi tôi muốn kết thúc phiên làm việc, tôi sẽ viết "We're done." Sau khi cuộc trò chuyện kết thúc, hãy cung cấp danh sách các điểm chính và bài học từ phiên làm việc mà tôi có thể xem xét lần tới khi viết tài trợ phục hồi. Đây là thông tin về tài trợ và tiêu chí đánh giá: [tải tài liệu lên].)_

## Thêm ý tưởng về AI Agents

Đây chỉ là một vài cách bạn có thể sử dụng các công cụ trí tuệ nhân tạo tạo sinh (Gen AI) để xây dựng AI agents nhằm đạt được mục tiêu của mình. Để có thêm ý tưởng về cách sử dụng AI agents tốt nhất, hãy xem các tài nguyên sau:

## Tài nguyên tham khảo

|Tài nguyên|Mô tả|
|---|---|
|**Professor Ethan Mollick's newsletter - One Useful Thing**|Mặc dù không chỉ tập trung vào AI agents, newsletter này có các mẹo và prompts trí tuệ nhân tạo tạo sinh (Gen AI) thực tế, cũng như những hiểu biết dựa trên nghiên cứu và các cuộc thảo luận kích thích tư duy về cách AI đang biến đổi các lĩnh vực khác nhau trong cuộc sống.|
|**Langchain**|Đây là một framework mã nguồn mở phổ biến sử dụng low code hoặc no code để kết nối các AI agents với nhau để hoàn thành các nhiệm vụ.|
|**Google Vertex AI Agents**|Cho phép người dùng thiết kế và tích hợp giao diện người dùng tương tác vào ứng dụng di động, ứng dụng web, thiết bị, bot, hệ thống phản hồi tương tác bằng giọng nói và nhiều hơn nữa. Chúng có thể phân tích nhiều loại đầu vào từ khách hàng, bao gồm đầu vào văn bản hoặc âm thanh, và phản hồi thông qua văn bản hoặc với giọng nói tổng hợp.|
|**Gems**|Đây là các personas AI có thể tùy chỉnh mà bạn tạo trong Gemini, mỗi cái có kỹ năng và kiến thức cụ thể, sẵn sàng hỗ trợ bạn với các nhiệm vụ cụ thể hoặc tìm hiểu sâu về bất kỳ chủ đề nào bạn quan tâm. Là một tính năng cụ thể được tích hợp sẵn trong Gemini, chúng cung cấp cách có cấu trúc để tạo và quản lý AI agents. Có một vài Gems được tạo sẵn bạn có thể làm việc cùng, bao gồm learning coach, brainstormer, career guide, writing editor, và coding partner.|

## Kết luận

AI agent có thể hoạt động như **trợ lý đáng tin cậy** (trusty sidekick) của bạn trong tất cả các trường hợp sử dụng. Chúng không chỉ ở đây để làm cho mọi thứ trở nên thú vị (mặc dù chúng chắc chắn làm được điều đó), chúng còn là **công cụ mạnh mẽ** để giúp bạn nâng cao trong công việc và cuộc sống hàng ngày. Hãy thử - bạn có thể ngạc nhiên với những gì bạn có thể đạt được với sự giúp đỡ của AI agent.