# 1. Mở đầu: Chatbot là gì?

Hẳn bạn đã từng nhắn tin hỏi thông tin trên website một công ty nào đó, và ngay lập tức nhận được câu trả lời như thể đang chat với một nhân viên tư vấn thật sự. Hoặc đơn giản hơn, bạn đã thử hỏi Siri "Hôm nay thời tiết thế nào?" hay nhờ Google Assistant đặt báo thức. Đó chính là chatbot - một chương trình máy tính được thiết kế để trò chuyện với con người thông qua văn bản hoặc giọng nói, gần giống như cách bạn trò chuyện với một người thật.

Nghe có vẻ đơn giản phải không? Nhưng thật sự chatbot ngày nay đã tiến hóa vượt xa những "chatbot cổ điển" mà bạn có thể từng gặp cách đây vài năm. Những chatbot ngày xưa chỉ có thể trả lời theo những kịch bản có sẵn, giống như một menu lựa chọn cứng nhắc: "Nhấn 1 để hỏi về giá", "Nhấn 2 để hỏi về địa chỉ"... Còn chatbot hiện đại? Chúng có thể hiểu ngữ cảnh, ghi nhớ cuộc hội thoại, thậm chí "sáng tạo" ra câu trả lời chưa từng được lập trình sẵn.

## 1.1. Bài viết này sẽ giúp bạn hiểu gì?
Trong bài viết này, chúng tôi sẽ đưa bạn đi từ những khái niệm cơ bản nhất về chatbot, cho đến việc giải mã cách hoạt động của các AI chatbot hiện đại - những "siêu trí tuệ nhân tạo" như ChatGPT, Google Bard hay Claude. Đặc biệt, chúng ta sẽ tập trung vào các chatbot được xây dựng dựa trên Large Language Models (LLM) - những mô hình ngôn ngữ lớn đang làm thay đổi cách chúng ta tương tác với máy móc.

## 1.2. Hãy cùng phân biệt hai "thế hệ" chatbot:
<p align="center">
  <img src="https://aioconquer.aivietnam.edu.vn/static/uploads/20260116_095833_3e05dc57.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 1.1. Hai thế hệ chatbot</em>
</p>

### a. Rule-based Chatbot (Chatbot dựa trên quy tắc)

- Hoạt động theo kịch bản được lập trình sẵn
- Giống như một cây quyết định: "Nếu người dùng nói A thì trả lời B"
- Ưu điểm: Dễ kiểm soát, chính xác trong phạm vi hẹp
- Nhược điểm: Không linh hoạt, không hiểu câu hỏi ngoài kịch bản

### b. AI-powered Chatbot (Chatbot dựa trên AI)

- Sử dụng Machine Learning và Deep Learning để "học" cách trả lời
- Có khả năng hiểu ngữ cảnh, xử lý ngôn ngữ tự nhiên phức tạp
- Ưu điểm: Linh hoạt, có thể xử lý vô số tình huống khác nhau
- Nhược điểm: Phức tạp hơn, đôi khi khó dự đoán

Và đây là điều thú vị: Chatbot AI hiện đại không chỉ "thông minh" hơn về mặt kỹ thuật, mà còn mang lại trải nghiệm gần gũi và tự nhiên hơn rất nhiều so với những người tiền nhiệm của chúng. Vậy bí mật đằng sau sự tiến hóa này là gì? Chúng ta sẽ cùng khám phá!

# 2. Vì sao chúng ta cần AI chatbot?

Trước khi đi sâu vào "bên trong" một chatbot hoạt động như thế nào, có lẽ bạn đang tự hỏi: "Tại sao chúng ta lại cần đến AI chatbot? Chatbot đơn giản theo quy tắc không đủ sao?"
Câu trả lời nằm ở ba yếu tố quan trọng: Quy mô, Tốc độ, và Trải nghiệm người dùng.

## 2.1. Quy mô: Phục vụ hàng triệu người cùng lúc
Hãy tưởng tượng bạn là chủ của một công ty thương mại điện tử lớn. Mỗi ngày có hàng chục nghìn khách hàng truy cập website và đặt câu hỏi: "Đơn hàng của tôi đến khi nào?", "Sản phẩm này có màu xanh không?", "Làm sao để đổi trả hàng?"...
Với chatbot rule-based truyền thống, bạn sẽ phải:

- Lập trình từng kịch bản cho từng loại câu hỏi
- Liên tục cập nhật khi có sản phẩm mới, chính sách mới
- Vẫn không thể xử lý các câu hỏi "ngoài kịch bản"

Nhưng với AI chatbot, hệ thống có thể:

- Tự động hiểu ngữ cảnh và ý định của khách hàng
- Trả lời hàng triệu câu hỏi khác nhau mà không cần lập trình riêng
- Học hỏi từ mỗi cuộc hội thoại để cải thiện theo thời gian

## 2.2 Tốc độ: Phản hồi tức thì, 24/7
Trong thời đại số, không ai muốn chờ đợi. Một nghiên cứu của HubSpot cho thấy 90% khách hàng mong đợi phản hồi tức thì khi họ có câu hỏi dịch vụ khách hàng. AI chatbot có thể:

- **Trả lời ngay lập tức:** Không cần thời gian chờ đợi như khi liên hệ với tổng đài
- **Hoạt động 24/7:** Không giới hạn giờ làm việc, múi giờ hay ngày nghỉ lễ
- **Xử lý đồng thời:** Một chatbot có thể "nói chuyện" với hàng nghìn người cùng lúc

Điều này không chỉ cải thiện trải nghiệm khách hàng mà còn giúp doanh nghiệp tiết kiệm chi phí vận hành đáng kể.
## 2.3. Trải nghiệm người dùng: Giao tiếp tự nhiên như con người
Đây chính là điểm mạnh nhất của AI chatbot so với các thế hệ trước. Thay vì phải nhớ các từ khóa cụ thể hoặc chọn từ menu cứng nhắc, người dùng có thể:

**Nói chuyện tự nhiên:**

- ❌ Chatbot truyền thống: "Bạn muốn kiểm tra đơn hàng? Vui lòng nhập mã đơn hàng."
- ✅ AI chatbot: "Chào bạn! Mình thấy bạn có đơn hàng #12345 đang trên đường giao. Bạn muốn biết thêm thông tin gì không?"

**Hiểu ngữ cảnh:**

- Người dùng: "Tôi muốn mua một chiếc điện thoại"
- Chatbot: "Bạn có ngân sách dự kiến bao nhiêu?"
- Người dùng: "Khoảng 10 triệu"
- Chatbot: "Vậy mình recommend cho bạn các mẫu sau..." *(chatbot nhớ được ngữ cảnh "điện thoại" và "10 triệu")*

**Cá nhân hóa:**
AI chatbot có thể phân tích lịch sử tương tác, sở thích của người dùng để đưa ra gợi ý phù hợp hơn, tạo cảm giác như đang được phục vụ bởi một trợ lý cá nhân.

## 2.4. Các ứng dụng thực tế
AI chatbot đã và đang xuất hiện ở khắp mọi nơi:
<p align="center">
  <img src="images\chatbot_usecase_mindmap.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 2.1. Các ứng dụng thực tế của AI chatbot</em>
</p>

**Dịch vụ khách hàng:**

- Ngân hàng: Kiểm tra số dư, lịch sử giao dịch, chặn thẻ
- Bảo hiểm: Tra cứu hợp đồng, hướng dẫn bồi thường
- Bán lẻ: Tư vấn sản phẩm, theo dõi đơn hàng

**Giáo dục:**

- Trợ giảng ảo: Trả lời thắc mắc của sinh viên
- Học ngoại ngữ: Luyện tập hội thoại tiếng Anh, Trung, Nhật...

**Y tế:**

- Tư vấn sơ bộ: Triệu chứng bệnh, lịch khám
- Nhắc nhở uống thuốc, chăm sóc sức khỏe

**Giải trí & Trợ lý cá nhân:**

- ChatGPT, Claude: Trợ lý viết lách, lập trình, brainstorming ý tưởng
- Siri, Google Assistant: Điều khiển thiết bị thông minh, đặt lịch hẹn

# 3. Quy trình một lượt chat diễn ra như thế nào?

Bạn từng tự hỏi: Từ lúc bạn nhấn Enter đến khi chatbot trả lời chỉ tốn vài giây, điều gì đã xảy ra?

**Cơ chế hoạt động của AI chatbot (NLP)**<br/>
Cách hoạt động của các chatbot sử dụng NLP (Natural Language Processing) thực chất bao gồm một chuỗi các bước khá logic để hiểu và trả lời người dùng một cách tự nhiên. Mình giải thích ngắn gọn, đơn giản như sau:

<p align="center">
  <img src="images/AI_chatbot_WorkFlow.svg" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.1. Quy trình xử lý một lượt chat của AI chatbot sử dụng NLP</em>
</p>

**1. Xử lý đầu vào** (Input Processing)

Khi bạn gửi tin nhắn, chatbot sẽ phân tích đoạn văn: tách thành từng từ (tokenization), xác định loại từ (danh từ, động từ…), và nhận diện các thông tin quan trọng như tên người, ngày tháng, địa điểm… Nói đơn giản là bước “đọc và hiểu sơ bộ” nội dung bạn vừa nhập.
<p align="center">
  <img src="images\input_processing.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.2. Xử lý đầu vào (Input Processing)</em>
</p>

**2. Nhận diện ý định (Intent Recognition)**

Sau khi phân tích, chatbot xác định mục đích chính của bạn: bạn đang hỏi thông tin, yêu cầu làm gì đó, phản hồi, hay chỉ trò chuyện thôi? Bước này thường dùng mô hình phân loại để gán một nhãn ý định (intent). Nhờ vậy bot biết nên tra dữ liệu, gọi API, hay sinh câu trả lời tự nhiên.
<p align="center">
  <img src="images\intent_recognition.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.3. Nhận diện ý định (Intent Recognition)</em>
</p>

**3. Quản lý hội thoại (Dialogue Management)**

Ở bước này, hệ thống quyết định “mạch" hội thoại:

- Dùng ngữ cảnh trước đó (những gì đã nói trong cuộc chat) để giữ câu trả lời liên tục, hợp lý.
- Chọn hành động tiếp theo: trả lời trực tiếp, gọi API (ví dụ tra lịch bay), cập nhật trạng thái, hay hỏi - thêm.
- Hệ thống quản lý giống như người điều phối cuộc trò chuyện để không bị lạc đề hoặc quên thông tin quan trọng.

**4. Tạo câu trả lời (Response Generation)**

Dựa trên ý định và ngữ cảnh, bot sẽ:<br/>
- Tìm thông tin từ cơ sở dữ liệu
- Thực hiện một hành động nào đó (như tra cứu, đặt lệnh)
- Hoặc tự tạo câu trả lời tự nhiên bằng các kỹ thuật sinh ngôn ngữ (natural language generation).
<p align="center">
  <img src="images\dialogue_management.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.4. Quản lý hội thoại và sinh câu trả lời</em>
</p>

**5. Học hỏi và cải thiện**

Không chỉ trả lời rồi thôi, chatbot còn có khả năng học từ các cuộc trò chuyện trước đó.
Thông qua dữ liệu tương tác, phản hồi của người dùng và các lần sửa lỗi, hệ thống dần cải thiện khả năng hiểu ngôn ngữ, nhận diện ý định chính xác hơn và đưa ra câu trả lời phù hợp hơn theo thời gian.

Nhờ cơ chế này, chatbot càng được sử dụng nhiều thì càng “thông minh” và linh hoạt hơn.
<p align="center">
  <img src="images\feedback.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.5. Chatbot học hỏi và tối ưu dựa trên phản hồi người dùng</em>
</p>

**6. Trả lời người dùng**

Cuối cùng, bot gửi lại câu trả lời dưới dạng văn bản (hoặc giọng nói), sao cho dễ đọc và thân thiện nhất có thể.
<p align="center">
  <img src="images\chat-ui.gif" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.6. Chatbot phản hồi sao cho dễ đọc và thân thiện nhất với người dùng</em>
</p>

*Quy trình này nghe có vẻ dài dòng nhưng thực tế nó diễn ra chỉ trong vài giây. Tất cả đều được xử lý tự động để mang lại cho bạn cảm giác như đang trò chuyện với một người bạn thực sự chứ không phải một cỗ máy vô tri.*

# 4. Main technologies in AI chatbot

Unlike their rule-based counterparts, AI chatbots use advanced technologies in AI to not only optimize its accuracy but also how natural it sounds when answering user questions. It also enables the chatbots to respond based on different context.

**4.1. NLP - Natural Language Processing:**

Natural Language Processing (NLP) allows AI systems to identify language and characters and to interpret grammar, context in text, speech, or conversations. By applying NLP, chatbots can effectively provide natural and comprehensively responses based on user’s context, unlocking more general and accurate information to user.

Key technologies of NLP using in AI chatbots:
Tokenization: Break down raw text into smaller units, which can be words, subwords, characters, or sentences, to make unstructured text understandable for machines. It helps to the keywords to process, analyze and understand human language to respond appropriately.
Example: "Book a flight tomorrow" → ["Book", "a", "flight", "tomorrow"]

<p align="center">
  <img src="images\part4_tokenization.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 4.1. Tokenization</em>
</p>

- Named Entity Recognition — NER: Recognize words, subwords in context and classifies them into groups such as human name, organization, location, time, product to help chatbots respond based on these entities.
Example: "What's the weather in Chicago tomorrow?" → Chicago is the entity to describe the location for chatbots to answer question about weather.

<p align="center">
  <img src="images\part4_NER.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 4.2. NER - Named Entity Recognition</em>
</p>

- Sentiment analysis: Identify and quantify opinions, emotions, and attitudes in text, speech, classifying them as positive, negative, or neutral to understand subjective information. It helps chatbots respond with a more pleasing, emotional tone to users.

<p align="center">
  <img src="images\part4_sentiment_analysis.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 4.3. Sentiment Analysis</em>
</p>

**4.2. AI models / Machine Learning / LLM:**

These technologies are the brain of AI chatbot, the data is trained, reinforced to help optimize the chatbot responses.

Machine Learning: Machine Learning algorithms helps train the chatbot how to process and respond to user based on predefined data.

Deep Learning: Allow chatbots to continuously learn from interactions, improving their ability to handle complex conversations

Large Language Models (LLMs): are trained on massive amounts of linguistic data, including grammar, spelling, and multiple languages. These models are used in chatbot training as a core approach to enable chatbots to accurately analyze user conversations and generate more natural and human-like responses.

<p align="center">
  <img src="images\part4_ML_DL_LLM_GenAI.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 4.4. Technologies uses to train AI chatbot</em>
</p>

In addition to the technologies mentioned above, Generative AI is now being used in chatbot training to improve performance. Generative AI turns chatbots from basic question-and-answer tools into AI agents, making conversations feel more like real human consultations. Instead of giving fixed or repetitive answers, chatbots can provide more flexible responses and reason to offer suggestions beyond their training data, while still staying relevant to the context of the conversation.

**4.3. Feedback and Continuous Learning:**

In addition to answering user questions, AI chatbots can continue learning based on users’ current responses. Data is continuously updated from ongoing conversations with both the current user and other users on the same topics, allowing the chatbot to optimize and expand its knowledge. As a result, the chatbot becomes smarter over time.

# 5. Comparative examples

## 5.1. Chatbots vs human assistants: what are the similarities and differences?

Imagine that you walk into a phone store and ask:

*“Does this phone have good battery life?”*

A human assistant would:

* Listen to your question
* Understand that you care about battery life, which is often seen as the “lifeline” of a smartphone
* Give advice based on real experience and the current context
* Ask follow-up questions to understand your needs better

An AI chatbot, however, handles the question in a different way:

* It does not “listen”; it reads text
* It does not “understand” in a human sense, but analyzes language patterns
* It uses learned data to predict the most suitable answer

In other words, modern chatbots mainly generate responses based on probability. They do not truly understand or reason like humans.

## 5.2. Comparing popular chatbots: ChatGPT, Gemini, and Copilot

 Although they are all called “AI chatbots,” each system is **designed for a different purpose**.

| **Chatbot**             | **Main purpose**                     | **Key strengths**                                                                               | **Best used when**                                                                    | **Context / Text Window (general)**                                   | **Main technical limitations**                                        |
| ----------------------- | ------------------------------------ | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| **ChatGPT**             | General conversation                 | Explains knowledge, answers questions, and writes content across many topics                    | When users want to “chat,” explore different topics, or need clear explanations       | Large – supports long conversations and remembers many previous turns | Can produce confident but incorrect answers; depends on training data |
| **Gemini (Google)**     | Information search and summarization | Searches and summarizes data from multiple sources; deeply integrated with the Google ecosystem | When users need to search for information, analyze data, or work with Google services | Very large – optimized for long texts and multiple sources            | Results can be too general; strongly depends on search context        |
| **Copilot (Microsoft)** | Work assistance                      | Helps with coding, writing emails, and working with Office documents                            | When users need direct support in daily work tasks                                    | Medium to large – optimized for work-related context                  | Limited outside work tasks; depends on the Microsoft ecosystem        |


<p align="center">  
<em>Table 5.1. Comparison between AI chatbots</em>
</p>

Simply put:

* ChatGPT is like a knowledgeable friend
* Gemini is like a research assistant
* Copilot is like a work colleague

All three are built on **Large Language Models** (LLMs)—models trained on massive amounts of data to generate new text.

The main differences are in **how they are deployed and the context in which they are used**, not in which one is “more intelligent.”

# 6. Common problems and limitations of AI chatbots 

## 6.1. Chatbots can misunderstand but sound very confident

One common issue with AI chatbots is that **their answers may sound reasonable but still be wrong**.

This happens because chatbots do not verify information like humans do. Instead, they predict the most likely answer based on learned data. When a question is unclear, lacks context, or falls outside the model’s training scope, the chatbot may still “guess” and produce a convincing response.

This is a core limitation of language models: they process language using statistical patterns and do not truly understand the real world.

## 6.2. Chatbots cannot fully replace humans

Even though they are very useful, AI chatbots have clear limitations:

* They do not have real emotions
* They do not fully understand social context
* They do not take responsibility for decisions
* In fields such as education, healthcare, or customer service, chatbots usually play a supporting role. They help reduce workload for humans rather than fully replacing them.

Many studies suggest that chatbots work best when they are designed to support humans, not to act as “artificial humans.”

## 6.3. Chatbots strongly depend on training data

The quality of an AI chatbot directly depends on:
* The amount of training data
* The quality of that data
* How the model is updated and fine-tuned

If the data is incomplete or biased, the chatbot may produce incorrect or biased answers. Data bias remains one of the biggest challenges in NLP today.

For this reason, chatbots are not “set-and-forget” systems—they need continuous training, evaluation, and improvement.

*Through this article, you have gained an overview of AI chatbots—from basic concepts and reasons for their development to how a single conversation is processed and the core technologies behind them. By combining natural language processing with modern AI models such as Large Language Models, chatbots today go beyond fixed scripts. They can handle context, generate flexible responses, and gradually improve over time.As a result, AI chatbots are becoming useful tools in many areas, including customer support, learning, work, and entertainment. They help save time, improve user experience, and open up many possibilities for future applications.*

**REFERENCES**

* Brown, T. B., Mann, B., Ryder, N., Subbiah, M., Kaplan, J., Dhariwal, P., … Amodei, D. (2020). Language models are few-shot learners. Advances in Neural Information Processing Systems, 33, 1877–1901. [https://arxiv.org/abs/2005.14165](https://arxiv.org/abs/2005.14165)

* Hovy, D., & Prabhumoye, S. (2021). Five sources of bias in natural language processing. Language and Linguistics Compass, 15(8), e12432. [https://doi.org/10.1111/lnc3.12432](https://doi.org/10.1111/lnc3.12432)

* Jurafsky, D., & Martin, J. H. (2023). Speech and language processing (3rd ed., draft). Stanford University. [https://web.stanford.edu/~jurafsky/slp3/](https://web.stanford.edu/~jurafsky/slp3/)

* Shum, H.-Y., He, X., & Li, D. (2018). From Eliza to XiaoIce: Challenges and opportunities with social chatbots. arXiv. [https://arxiv.org/abs/1812.08989](https://arxiv.org/abs/1812.08989)

* Zhang, Y., Sun, S., Galley, M., Chen, Y.-C., Brockett, C., Gao, X., … Dolan, B. (2024). A complete survey on LLM-based AI chatbots. arXiv. [https://arxiv.org/abs/2406.16937](https://arxiv.org/abs/2406.16937)

* GeeksforGeeks. (n.d). What is Natural Language Processing? [https://www.geeksforgeeks.org/nlp/what-is-natural-language-processing-nlp-chatbots/](https://www.geeksforgeeks.org/nlp/what-is-natural-language-processing-nlp-chatbots/)
