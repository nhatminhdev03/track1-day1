# CP2 — Tệp user & JTBD: NotebookLM

**Bài làm cá nhân**  
**Sản phẩm:** NotebookLM (Google Labs)  
**Cách đọc nguồn:** “early adopter” dưới đây là chân dung tổng hợp có kiểm soát từ bối cảnh launch 2023 và ví dụ use case chính thức; “tệp hiện tại” là chân dung tổng hợp từ Product Hunt, Reddit và Google Blog 2024–2025. Không coi một comment đơn lẻ là đại diện toàn bộ người dùng.

## 1. Nguồn đã đọc

| Nguồn | Loại | Điều rút ra |
|---|---|---|
| [Introducing NotebookLM — Google, 12/07/2023](https://blog.google/innovation-and-ai/technology/ai/notebooklm-google-ai/) | Launch post | Early access nhỏ ở Mỹ, chỉ Google Docs; Google nói chuyện với students, professors và knowledge workers; ví dụ medical student, author, content creator, entrepreneur. |
| [HN launch thread, 2023](https://news.ycombinator.com/item?id=36697119) | Community sớm | Thảo luận của nhóm kỹ thuật/AI early adopters về privacy, source grounding và Discord/waitlist. |
| [Google NotebookLM trên Product Hunt, 20/05/2025](https://www.hunted.space/product/google-notebooklm-2/launches/google-notebooklm-3) | Product Hunt archive | Tệp 2025 đã bao gồm students, creators, researchers, professionals; một reviewer nêu research, source attribution và xử lý bài báo học thuật là “killer feature”. |
| [NotebookLM Plus — Google, 13/12/2024](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-new-features-december-2024/) | Product update | Studio, Interactive Audio và Plus mở rộng sang power users/teams/enterprises. |
| [Mind Maps & study features — Google, 03/04/2025](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-studying-help/) | Product update | Google ghi nhận hàng chục nghìn trường dùng cho study assistance, writing support, research và interactive learning. |
| [Mobile app — Google, 19/05/2025](https://blog.google/innovation-and-ai/products/notebooklm-app/) | Product update | Offline Audio, share web/PDF/YouTube từ điện thoại; giảm rào cản sử dụng ngoài desktop. |
| [Reddit: cảnh báo không phụ thuộc NotebookLM cho việc học](https://www.reddit.com/r/notebooklm/comments/1o1dhc9/beware_of_relying_on_notebooklm_for_schoolwork/) | Community/review trái chiều | User 1–2 sao về outcome cho thấy công cụ phù hợp cho review, hiểu và luyện tập có kiểm chứng — không thay thế đọc gốc hay tự học. |
| [G2 reviews](https://www.g2.com/products/google-notebooklm/reviews) | Review B2B | Review mô tả stack cũ gồm PDF reader, ghi chú, bookmark, transcription và AI summarizer; giá trị là traceability cho research/regulated work. |

## 2. Bảng so sánh hai tệp

| | Early adopters (2023–đầu 2024) | Tệp hiện tại (2024–2025) |
|---|---|---|
| **Có thể “gọi tên”** | **Minh, 28 tuổi**, nghiên cứu sinh y sinh ở Mỹ; đã dùng Google Docs để lưu paper/ghi chú, theo dõi Google Labs/AI Twitter và sẵn sàng xin waitlist. Cần đối chiếu nhiều tài liệu nhưng không muốn đưa chúng vào chatbot tổng quát. | **Linh, 20 tuổi**, sinh viên điều dưỡng năm 2; có slide, PDF bài giảng và câu hỏi ôn tập trên Drive/điện thoại. Học khi di chuyển, cần ôn có cấu trúc trước kỳ thi, nhưng vẫn phải kiểm tra lại tài liệu/giảng viên. |
| **Đặc điểm phân khúc** | Tolerance cao với beta và prompt; có sẵn bộ tài liệu số hóa, chủ yếu Google Docs; có năng lực tự fact-check. Đây là nhóm knowledge worker/academic/creator có “information overload” rõ rệt, không phải mọi người dùng ghi chú. | Mở rộng sang người học đại chúng và knowledge workers theo project. Họ không cần hiểu RAG/prompt sâu, dùng PDF, Slides, URL, YouTube; mong output phù hợp ngữ cảnh: quiz, mind map, audio/video, brief. |
| **JTBD (viết theo việc cần làm)** | *Khi đang gom ghi chú và tài liệu cho một chủ đề chuyên sâu, hãy giúp tôi truy ra, nối và tóm tắt các ý trong đúng tập Google Docs của tôi để tôi tạo được hypothesis/dàn ý có thể đối chiếu lại, thay vì đọc lại từng file.* | *Khi phải hiểu và nhớ một khối bài học/tài liệu lớn trong thời gian ngắn, hãy biến đúng tài liệu lớp/tài liệu dự án thành lời giải thích, câu hỏi luyện tập và bản nghe/xem theo mục tiêu của tôi để tôi ôn, chuẩn bị hoặc chia sẻ được — nhưng không làm tôi tin mù quáng vào AI.* |
| **Cách cũ họ làm việc** | Ctrl+F và đọc chéo nhiều Docs/PDF; highlight rồi tự tổng hợp trong Google Docs/Notion; dùng chatbot chung rồi tự kiểm từng claim/quay lại nguồn. | Đọc slide/PDF, tự ghi flashcard/Quizlet, xem YouTube, dùng Google Drive/Docs; nghe podcast hoặc hỏi ChatGPT/Gemini nhưng thiếu tập nguồn cố định và citation. |
| **Điểm đau chính** | Mất thời gian tạo liên kết giữa nguồn; chatbot tổng quát có thể bịa hoặc không biết file nào đáng tin; lo data research riêng tư. | Quá tải tài liệu, khó duy trì nhịp học và khó biến reading thành active recall; cần dùng mobile/đa phương thức nhưng sợ audio/quiz bỏ sót hay sai. |
| **Cột mốc làm tệp dịch chuyển** | **06/06/2024 global rollout + Gemini 1.5 Pro, URL/Slides/citations**: không còn chỉ là waitlist/Google Docs cho nhóm kỹ thuật. | **11/09/2024 Audio Overviews**, **17/10/2024 bỏ nhãn Experimental**, **13/12/2024 Plus/Interactive Audio**, **03/04/2025 Mind Maps & source discovery**, **19/05/2025 mobile app**: giảm rào cản, đưa use case sang học tập đa phương thức và dùng hằng ngày. |

## 3. Dịch chuyển tệp: nguyên nhân và giới hạn

Mốc gây dịch chuyển lớn nhất là **global rollout tháng 06/2024**: mở sản phẩm tới hơn 200 quốc gia/vùng lãnh thổ, thêm URL/Slides và nâng bằng Gemini 1.5 Pro. Nó biến NotebookLM từ thử nghiệm hẹp cho người sẵn sàng dùng Google Docs thành công cụ có thể tiếp nhận “tài liệu thật” của học sinh, researcher và knowledge worker.

Sau đó **Audio Overview (09/2024)**, **Mind Maps/source discovery (04/2025)** và **mobile app (05/2025)** đổi *job flow*: từ “tìm insight trong nguồn” thành “tiêu hóa, ôn và chia sẻ kiến thức theo lúc/thiết bị phù hợp”. Tuy vậy, Reddit cho thấy đây vẫn là công cụ bổ trợ: tệp học sinh dùng nó để review/chunking/quiz, không nên thay thế đọc nguồn hay thực hành.

## 4. Switching cost — map 4 forces

| Force | Biểu hiện với NotebookLM | Hàm ý sản phẩm |
|---|---|---|
| **Push của cách cũ** | Đọc chéo nhiều PDF/Slides, highlight, tự chép note và chuyển giữa PDF reader–Drive–Quizlet–chatbot rất chậm. | Source ingestion, chat có citation và Studio giải quyết workflow chứ không chỉ tạo text. |
| **Pull của lựa chọn mới** | ChatGPT, Claude, Gemini hoặc Perplexity có thể viết/tìm web tốt hơn; flashcard apps và note apps có thói quen sẵn. | NotebookLM phải chứng minh lợi thế “grounded trong bộ nguồn” và output học tập, thay vì cạnh tranh như chatbot vạn năng. |
| **Anxieties (lo ngại khi dùng/chuyển)** | Sợ hallucination, audio/quiz bỏ sót ý, hiểu sai diagram; lo privacy của tài liệu nhạy cảm; lo mất thời gian nạp/sắp xếp nguồn. | Citation, cảnh báo cần fact-check và quyền kiểm soát nguồn là điều kiện tin dùng, không phải tính năng phụ. |
| **Habit/inertia (thói quen/ma sát)** | Google Docs/Drive, quy trình note và notebook đã tổ chức, prompt/workflow quen thuộc; với team là notebook dùng chung và quy tắc kiểm chứng. Nhưng file có thể export/import, nên lock-in dữ liệu thuần túy không quá cao. | Cần tăng switching cost bằng workflow tin cậy, collaboration và continuity, không chỉ nhốt file trong sản phẩm. |

## 5. Lực giữ user mạnh nhất và phản biện

**Mạnh nhất:** *source-grounding có citation trong một workflow đã được tổ chức.* Nó trực tiếp giải quyết rủi ro lớn nhất của nghiên cứu/học tập: “câu trả lời này dựa vào đâu?” Đồng thời, notebook lưu bộ nguồn, câu hỏi và các output (guide/audio/mind map) quanh một project nên tạo thói quen quay lại.

**Nếu lực này biến mất:** nếu citation không đáng tin hoặc NotebookLM trả lời như chatbot chung không bám tập nguồn, sản phẩm sẽ mất khác biệt cốt lõi. Người dùng dễ quay về ChatGPT/Claude/Perplexity cho prompt nhanh, hoặc Drive + PDF reader + Quizlet cho học tập; chi phí chuyển đổi file không đủ lớn để giữ họ lại. Đây là lý do các review tiêu cực về bỏ sót/sai trong audio hoặc dùng AI thay đọc gốc quan trọng: chúng không chỉ là bug, mà đánh thẳng vào lý do để tin sản phẩm.

## 6. Câu hỏi cần chốt cùng nhóm

- Nhóm có đồng ý “grounded research/learning từ bộ nguồn tự chọn” là JTBD lõi, còn podcast/video/quiz là các cách hoàn thành job không?
- Chọn **global rollout + source types (06/2024)** hay **Audio Overviews (09/2024)** làm mốc segment-shift chính trong timeline Step 1? Nháp này nghiêng về mốc 06/2024 là điều kiện mở tệp, còn Audio là chất xúc tác tăng adoption/engagement.
