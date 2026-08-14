# Memo Teardown — NotebookLM → Gemini Notebook

**Nhóm:** Grounded · **Thành viên:** Cao Nhật Minh — 2A202601721; Dương Văn Vũ — 2A202601663; Phạm Khánh Linh — 2A202601507

**Vì sao chọn sản phẩm này:** Gemini Notebook là ví dụ rõ về một AI product đi từ “chat có căn cứ trên nguồn user nạp” sang workflow học tập, nghiên cứu và phân tích nằm trong hệ sinh thái Gemini/Search. Chuỗi đổi tên, mở input, đổi output và bán theo tier cho thấy các quyết định sản phẩm liên kết với nhau, thay vì chỉ là changelog.

## §1. Timeline các cập nhật lớn

| Thời điểm | Cập nhật | Context lúc đó | Nguyên lý |
|---|---|---|---|
| **12/07/2023** | Project Tailwind đổi tên thành **NotebookLM**, thử nghiệm hạn chế tại Mỹ; chat grounded trong nguồn user nạp và có citation. [Google](https://blog.google/innovation-and-ai/technology/ai/notebooklm-google-ai/) | Thị trường đã quen chatbot “biết mọi thứ” nhưng lo hallucination. | Ràng buộc nguồn là tính năng: cạnh tranh bằng câu trả lời truy vết được, không phải trả lời mọi thứ. |
| **06/06/2024** | Mở 200+ quốc gia, Gemini 1.5 Pro; thêm Google Slides, URL web và hiểu hình/biểu đồ. [Google](https://blog.google/innovation-and-ai/products/notebooklm-goes-global-support-for-websites-slides-fact-check/) | Long context và multimodal trở nên khả thi hơn. | Mở rộng loại dữ liệu vào để user dồn corpus dự án vào một nơi, tăng switching cost. |
| **11/09/2024** | Ra **Audio Overviews** dạng hai AI host; có thể tải về. [Google](https://blog.google/innovation-and-ai/products/notebooklm-audio-overviews/) | Sản phẩm research tốt nhưng còn ngách và ít được biết đến. | Đổi cách tiêu thụ kiến thức: từ đọc/tra cứu sang nghe khi đi lại; output trở thành kênh phân phối. |
| **13/12/2024** | UI **Sources · Chat · Studio**; ra NotebookLM Plus với limit cao hơn, shared notebook, analytics và bảo mật tổ chức. [Google](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-new-features-december-2024/) | Đã có triệu user và nhu cầu dùng theo team/tổ chức. | Bán độ sâu workflow, collaboration và compliance thay vì chỉ bán token/model. |
| **19/05/2025** | Ra app iOS/Android: nghe offline/nền, share web/PDF/YouTube trực tiếp vào notebook. [Google](https://blog.google/innovation-and-ai/products/notebooklm-app/) | Audio đã tạo nhu cầu dùng khi di chuyển. | Mobile là điểm capture dữ liệu mới, không chỉ là bản thu nhỏ của web. |
| **09–11/2025** | Learning Guide, Flashcards, Quizzes và report tùy biến; flashcards/quizzes lên mobile. [Web](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-student-features/) · [Mobile](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-app-quizzes-flashcards/) | Student trở thành tệp dùng lặp lại, đặc biệt trong mùa học/thi. | Vertical hóa theo JTBD học tập: từ “hiểu” sang “nhớ và tự kiểm tra”. |
| **11/2025** | Deep Research cho phép tìm và dựng danh sách nguồn web có trích dẫn. [Nguồn thứ cấp — cần đối chiếu](https://glasp.co/articles/notebooklm-2026) | Mô hình BYO-source lộ vấn đề cold start: user mới không có sẵn bộ nguồn. | Nới ràng buộc ở tầng thu thập nguồn, nhưng giữ nguồn hiển thị/citation để bảo toàn niềm tin. |
| **16/07/2026** | Đổi tên thành **Gemini Notebook**; thêm secure cloud computer để chạy code trên nguồn; công bố hơn 30 triệu user và 600.000+ tổ chức. [Google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook/) | Google gom các bề mặt AI vào thương hiệu Gemini và bundle AI Pro/Ultra. | Đổi brand equity lấy distribution; nâng job từ đọc/hiểu tài liệu lên thực thi phân tích trên tài liệu. |

**Vì sao chọn những mốc này:** Chỉ giữ các mốc làm thay đổi ít nhất một trong bốn yếu tố: ai dùng, dữ liệu đầu vào, output/workflow hoặc cách Google kiếm tiền/giữ chân. Đã loại các thay đổi mang tính changelog như version App Store, đổi domain, thay model dưới nắp capo, và các output chỉ tiếp tục logic Studio/Audio đã có. Mốc Deep Research cần được xác minh thêm bằng nguồn Google trước khi dùng trong bản nộp cuối.

## §2. Tệp user & JTBD

| | Early adopters | Tệp hiện tại |
|---|---|---|
| Đặc điểm | Tác giả nonfiction, researcher, graduate student, analyst/consultant có sẵn nhiều Google Docs/PDF, quen thử LLM và chấp nhận UI thử nghiệm. Họ tự xây bộ nguồn trước khi hỏi AI. | Student/học sinh, gồm cả người học cần hỗ trợ tập trung; knowledge worker như PM, manager, analyst, researcher; và mobile user trong hệ Google. Họ thường bắt đầu từ một việc gấp: thi, họp, PDF, web hoặc video. |
| JTBD chính | “Khi viết/nghiên cứu từ hàng chục tài liệu, giúp tôi tìm đúng trích dẫn, thấy liên hệ giữa ý và lập outline/timeline để không mất dòng suy nghĩ.” | **Student:** “Khi sắp thi và có giáo trình dài, giúp tôi hiểu–nhớ–tự kiểm tra ít mệt hơn.” **Professional:** “Khi cần bắt kịp dự án, giúp tôi tổng hợp tài liệu/họp thành brief, PRD hoặc deck có căn cứ nhanh hơn.” **Mobile:** “Khi gặp nguồn hay, giúp tôi lưu và tiêu thụ nó ngay thay vì để trong read-later.” |
| Trước đó họ làm bằng cách nào | Cmd/Ctrl-F qua PDF/Docs, note/outline thủ công, Scrivener/Google Docs, bookmark, tự ghép trích dẫn và timeline. | Đọc lại/highlight giáo trình, Anki/Quizlet, transcript + Docs/Notion, nhiều tab browser, upload file từng lần vào ChatGPT/Claude hoặc dùng TTS. |

**Dịch chuyển tệp:** Mốc 06/06/2024 mở rộng quốc gia và loại nguồn; 11/09/2024 Audio Overviews biến research tool thành trải nghiệm dễ tiêu thụ/chia sẻ; 19/05/2025 mobile hạ ma sát capture và Google cho biết tổng user tăng gấp đôi vài tuần sau đó. Flashcards, quizzes và Learning Guide trong 09–11/2025 hoàn tất JTBD học tập, đưa student thành wedge tăng trưởng rõ ràng. [Mobile growth signal](https://blog.google/innovation-and-ai/products/developing-notebooklm/)

**Switching cost (map 4 forces):**

| Force | Điều quan sát được | Hàm ý |
|---|---|---|
| Push | Quá nhiều PDF, transcript, tab và note; khó tìm lại nguồn và biến chúng thành đầu ra. | User thử sản phẩm để thoát “information debt”, không phải chỉ vì muốn dùng AI. |
| Pull | Citation, nhiều output từ cùng một bộ nguồn, Audio/quiz/flashcard và mobile share sheet. | Tạo aha moment nhanh, nhất là với học tập và research có nguồn rõ ràng. |
| Anxiety | Sai sót/hallucination, privacy, nỗi lo Google đổi/đóng sản phẩm, lỗi và thiếu parity mobile. | Rào cản lớn với công việc cần độ tin cậy hoặc workflow chuyên sâu. |
| Habit | Anki/Quizlet, Docs/Notion/Obsidian/Zotero và thói quen tự đọc/kiểm chứng. | Gemini Notebook cần đứng trong workflow hiện có; không thể thay hoàn toàn chúng. |

Switching cost hiện ở mức vừa phải vì user vẫn mang PDF/Docs sang sản phẩm khác được. Nó tăng dần khi notebook tích lũy corpus dự án, prompt/workflow, output và liên kết Gemini/Google; nhưng đối thủ có import tốt và độ tin cậy cao vẫn có thể kéo user đi.

## §3. Dự đoán hướng đi (6–12 tháng tới)

**Trạng thái:** Nhóm đã loại hai dự đoán ban đầu sau vòng phản biện vì bằng chứng chưa đủ chặt; chỉ giữ dự đoán dưới đây.

**Dự đoán chốt** *(loại: đe dọa Big Tech)*

- **Dự đoán:** Gemini Notebook sẽ trở thành lớp ngữ cảnh của Gemini và AI Mode Search: user bắt đầu bằng câu hỏi/truy vấn, lưu nguồn vào notebook, rồi dùng notebook để hỏi sâu, kiểm chứng citation và tạo report/deck. Web app độc lập vẫn giữ vai trò deep-work workspace với bộ nguồn bền vững.
- **Lập luận:** Step 1 cho thấy hướng đi liên tục giảm ma sát đầu vào — URL/Slides, Discover Sources, mobile share sheet và research web. Step 2 cho thấy tệp hiện tại bắt đầu bằng nhiệm vụ gấp, không phải corpus có sẵn; buộc họ vào một app riêng sẽ thêm bước. Google đã đồng bộ notebooks với Gemini ngày 08/04/2026, đổi tên sang Gemini Notebook ngày 16/07/2026 và nói sẽ đưa notebooks vào AI Mode Search, trong khi vẫn giữ standalone research product. [Gemini integration](https://blog.google/innovation-and-ai/products/gemini-app/notebooks-gemini-notebooklm/) · [Rename/Search direction](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook/)

**Dấu hiệu kiểm chứng:** AI Mode Search có thể tạo/tiếp tục notebook trực tiếp từ kết quả; Gemini đưa chat, file và search result vào notebook với đồng bộ hai chiều; standalone app ưu tiên phân tích/output nâng cao, còn Gemini/Search ưu tiên khởi tạo và khám phá nguồn.

**Điều kiện bác bỏ:** Dự đoán sai nếu sau 12 tháng AI Mode Search chỉ liên kết ra trang Gemini Notebook và không tạo context chung, hoặc Google tách notebook khỏi Gemini/Search do privacy, consent hay chất lượng citation.

## §4. AI Log

| Việc | AI làm hay nhóm làm? | Nhóm kiểm chứng/phán đoán lại thế nào? |
|---|---|---|
| Thu thập timeline và nguồn App Store/Google Play/Google Blog | AI thu thập, chuẩn hóa ngày và link. | Nhóm chọn 8 mốc theo tiêu chí: phải đổi user, input, output/workflow hoặc monetization. |
| Phân tích early adopters, tệp hiện tại và JTBD | AI tổng hợp Google Blog, App Store review, Reddit và báo chí. | Nhóm phân biệt bằng job/cách làm cũ, không gắn nhãn chung chung như “mọi người” hay “developer”. |
| Dự đoán 6–12 tháng | Mỗi thành viên/agent viết nháp độc lập. | Nhóm phản biện: bỏ dự đoán feature/monetization vì phần mới và bằng chứng segment chưa đủ; giữ dự đoán Gemini + Search vì có tín hiệu công khai trực tiếp. |
| Chọn luận điểm xuyên suốt memo | Nhóm làm.| Nhóm chốt cách đọc timeline là chuỗi quyết định sản phẩm: nguồn có kiểm soát → nhiều dạng hiểu → workflow học tập/phân tích → distribution qua Gemini. |
| Loại mốc và dự đoán yếu | Nhóm làm | Nhóm không đưa changelog/version App Store vào timeline; loại hai dự đoán đầu vì chưa đủ dữ kiện mới và chưa chứng minh được segment cụ thể. |
| Chịu trách nhiệm với dự đoán cuối | Nhóm làm | Nhóm giữ dự đoán Gemini Notebook trở thành lớp context cho Gemini/Search, đồng thời ghi dấu hiệu kiểm chứng và điều kiện bác bỏ để có thể đánh giá lại sau 6–12 tháng. |
