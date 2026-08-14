# Step 1 — Timeline & Revert nguyên lý: NotebookLM → Gemini Notebook

**Sản phẩm:** NotebookLM (Google Labs), đổi tên thành **Gemini Notebook** từ 16/07/2026.
**Phạm vi:** 07/2023 → 08/2026. Timeline dùng tên *NotebookLM* cho các mốc trước 07/2026.

> **Cách đọc bảng này:** cột **Cập nhật** là dữ kiện có nguồn. Cột **Context** và **Nguyên lý** là diễn giải chiến lược của nhóm — đọc như một chuỗi quyết định, không phải changelog.
> **Quy tắc chọn mốc:** một hàng chỉ được vào bảng nếu nó đổi ít nhất **một trong bốn thứ**: (1) *ai dùng*, (2) *dữ liệu nào được đưa vào*, (3) *output/workflow nào sinh ra*, (4) *Google kiếm tiền / giữ chân bằng cách nào*. Đổi tính năng mà không đổi bốn thứ này → không phải quyết định sản phẩm.

---

## §1. Bảng timeline (8 cột mốc)

| # | Thời điểm | Cập nhật | Context lúc đó | Nguyên lý |
|---|---|---|---|---|
| 1 | **12/07/2023** | Project Tailwind đổi tên thành **NotebookLM**, mở thử nghiệm hạn chế tại Mỹ. Chat bị **ràng buộc trong bộ nguồn người dùng tự nạp**, mọi câu trả lời có citation trỏ ngược về đoạn gốc. [Google Blog](https://blog.google/innovation-and-ai/technology/ai/notebooklm-google-ai/) | ChatGPT ra 11/2022 đã set kỳ vọng "chatbot biết tuốt"; cả ngành đua nhau làm trợ lý vạn năng và cả ngành đang chảy máu vì hallucination. Google — bên có nhiều thứ để mất nhất về uy tín — **không** đua trên sân đó, mà mở một sân khác. | **Ràng buộc là tính năng — và là cách định nghĩa lại "tốt".** Ngành đo "tốt" = biết mọi thứ. NotebookLM đo "tốt" = *không nói gì ngoài tài liệu của bạn, và luôn chỉ được chỗ*. Cùng model, đổi định nghĩa "tốt" → ra một sản phẩm khác. Moat không nằm ở model (Google không giữ được lợi thế đó) mà nằm ở **corpus user tự mang vào** — thứ đối thủ không copy được. |
| 2 | **06/06/2024** | Mở **200+ quốc gia**, chạy trên **Gemini 1.5 Pro**; mở nguồn từ Docs/PDF sang **Slides, URL web**, và đọc được ảnh/biểu đồ trong tài liệu. [Google Blog](https://blog.google/innovation-and-ai/products/notebooklm-goes-global-support-for-websites-slides-fact-check/) | Gemini 1.5 Pro vừa đẩy long-context lên hàng triệu token và rẻ đi rõ rệt. Trước đó "nạp cả bộ tài liệu" là bất khả thi về chi phí/chất lượng. Sản phẩm chờ nền model nâng trần rồi mới mở van. | **Wrapper mỏng nằm chờ model nâng trần, rồi tiêu số x10 đó ở phía input.** Google không dùng năng lực mới để trả lời hay hơn, mà để **cho phép đổ nhiều loại rác hơn vào**. Đây là nước đi moat: mỗi định dạng mở thêm = thêm một lý do user dồn corpus vào đây = switching cost tăng. x10 đúng chỗ: bỏ bước "chuẩn hoá tài liệu trước khi hỏi". |
| 3 | **11/09/2024** | **Audio Overviews** — biến bộ nguồn thành cuộc hội thoại podcast hai host AI, tải về được. [Google Blog](https://blog.google/innovation-and-ai/products/notebooklm-audio-overviews/) | Sản phẩm đã đúng nhưng ít người biết; AI tiêu dùng lúc này cạnh tranh bằng attention chứ không bằng benchmark. Đây là mốc NotebookLM viral, kéo lượng lớn user không-phải-researcher vào. | **x10 ở khâu *tiêu thụ*, không phải khâu *trả lời*.** Cùng một nội dung, đổi format thì đổi luôn tình huống sử dụng (đi bộ, lái xe, rửa bát) — mở ra thời gian mà đối thủ dạng chat không với tới. Kèm theo: audio là **artifact chia sẻ được** → mỗi output là một kênh phân phối. Định nghĩa "tốt" dịch tiếp: từ *trả lời đúng* → *tôi có tiêu hoá nổi không*. |
| 4 | **13/12/2024** | Đóng gói lại UI thành **Sources · Chat · Studio**; ra **NotebookLM Plus** (limit gấp ~5×, shared notebook, analytics, bảo mật tổ chức) sau pilot Business 10/2024. Rollout Gemini 2.0 Flash. [Google Blog](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-new-features-december-2024/) · [Product Hunt](https://www.producthunt.com/products/google-notebooklm-plus) | Đã có "millions of users" và "tens of thousands of organizations" dùng free. Nhu cầu team/enterprise xuất hiện tự phát. Google Labs cần chứng minh đây là sản phẩm chứ không phải demo. | **Bán độ sâu workflow, không bán token — và đặt tên khoang trước khi lấp đầy.** Plus không bán model xịn hơn; bán *limit, cộng tác, analytics, compliance* — tức bán moat workflow/team. Song song, ba khoang Sources·Chat·Studio là quyết định kiến trúc quan trọng hơn cả pricing: nó dựng sẵn cái hộc "Studio" để **mọi format tương lai (video, mind map, flashcard, report) chỉ là thêm một ô, không phải redesign**. Đặt tên đúng mental model → mở rộng mà không phá cấu trúc. |
| 5 | **19/05/2025** | Ra app **iOS + Android**: nghe Audio offline/nền, **share thẳng web/PDF/YouTube từ app khác vào notebook**. [Google Blog](https://blog.google/innovation-and-ai/products/notebooklm-app/) | I/O 2025; Gemini 2.5 Flash trở thành model mặc định (cân bằng chất lượng/tốc độ/giá) khiến chạy nền trên mobile khả thi. User đòi mobile suốt từ lúc Audio viral. | **Đổi điểm capture, không đổi lõi.** Mobile ở đây không phải "port giao diện" mà là **mở một cửa nạp dữ liệu mới**: share sheet. Vòng lặp đổi hình: trước là *ngồi xuống nghiên cứu*; giờ là *gặp nguồn khi đang lướt → ném vào notebook → nghe/hỏi lúc di chuyển*. Sản phẩm đi tới nơi **dữ liệu và attention thực sự xuất hiện**, thay vì bắt user đi tới sản phẩm. |
| 6 | **09–11/2025** | **Pivot segment sang learning:** Learning Guide, **Flashcards, Quizzes**, report tuỳ biến; đưa lên mobile 06/11/2025. Nền đã có: Studio nhiều artifact + Video Overviews 80 ngôn ngữ (07–08/2025). [Learning features](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-student-features/) · [Mobile 11/2025](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-app-quizzes-flashcards/) | Mùa back-to-school; Google đẩy mạnh Gemini for Education. Dữ liệu sử dụng cho thấy sinh viên là tệp lớn nhất và dính nhất — Google chọn phục vụ tệp đã tự tìm đến thay vì tệp mình muốn có. | **Vertical AI + đóng vòng lặp học.** Không thêm format nữa mà **thêm một vòng phản hồi**: quiz sinh ra tín hiệu mà chat không bao giờ có được — *user sai ở đâu*. Đó là dữ liệu vòng lặp, và là lần dịch chuyển thứ ba của "tốt": từ *tiêu hoá được* → **nhớ và làm được**. Verticalization ở đây là theo job-to-be-done (input = tài liệu học, output = flashcard/quiz, feedback = câu sai + giải thích có citation), không phải theo ngành. |
| 7 | **11/2025** | **Deep Research:** sản phẩm **tự đi tìm và dựng danh sách nguồn có trích dẫn từ web mở**, thay vì chỉ chờ user nạp. [Glasp tổng hợp](https://glasp.co/articles/notebooklm-2026) *(nguồn thứ cấp — cần đối chiếu thêm)* | Perplexity/ChatGPT Deep Research đã bình thường hoá chuyện agent tự duyệt web. Đồng thời điểm chết lớn nhất của mô hình BYO-source lộ rõ: **notebook trống** — user mới không biết đổ gì vào. | **Nới ràng buộc sáng lập ở tầng *thu thập*, giữ nguyên ở tầng *hiển thị*.** 2023 chọn "chỉ dùng nguồn của bạn" làm moat; 2025 tự đảo ngược chính nó — nhưng có kiểm soát: nguồn agent tìm về vẫn nằm trong panel Sources, vẫn nhìn thấy, vẫn cite được. Ràng buộc bị bỏ ở chỗ nó gây ma sát (cold start), giữ ở chỗ nó tạo niềm tin. **Một nguyên lý được giữ đúng chỗ nó tạo giá trị, không giữ như giáo điều.** |
| 8 | **16/07/2026** | Đổi tên thành **Gemini Notebook** (logo gradient Gemini); mỗi notebook có **"secure cloud computer"** — viết & chạy code phân tích ngay trên nguồn đã nạp, giới hạn cho AI Ultra / Workspace tier cao. Quy mô lúc này: **~30 triệu user, 600.000+ tổ chức**. Từ 01/08/2026 chuyển sang notebook.google.com. [Google Blog](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook/) · [9to5Google](https://9to5google.com/2026/07/16/notebooklm-gemini-notebook/) | Google đang gom mọi bề mặt AI về một thương hiệu Gemini để bán bundle (AI Pro/Ultra). NotebookLM là sản phẩm Labs hiếm hoi có brand equity riêng đủ mạnh — và Google vẫn chọn bỏ cái tên đó. | **Đổi brand equity lấy distribution + nâng trần "tốt" từ *đọc* lên *thực thi*.** Hai quyết định trong một: (a) hy sinh nhận diện riêng của ~30M user để lấy entitlement/upsell/bundling của hệ Gemini — moat chuyển từ *sản phẩm* sang *gói thuê bao*; (b) cloud computer nâng job từ *hiểu tài liệu* lên *chạy phân tích trên tài liệu*, và **gate nó theo tier** — lặp lại đúng công thức 12/2024: tính năng sâu nhất là tính năng bán được. |

---

## §2. Vì sao chọn 8 mốc này

Đọc dọc bảng, đây không phải 8 tính năng mà là **một lập luận có hướng**:

> *Chọn một ràng buộc (1) → mở van dữ liệu vào ràng buộc đó (2) → đổi cách output đi ra (3) → đóng gói & thu tiền (4) → đổi điểm nạp dữ liệu (5) → đóng vòng phản hồi cho một tệp cụ thể (6) → nới ràng buộc ban đầu khi nó thành ma sát (7) → bán mình vào hệ phân phối lớn hơn và nâng trần job (8).*

Ba dịch chuyển của định nghĩa **"tốt"** là xương sống: *đúng & có bằng chứng* (2023) → *tiêu hoá được* (2024) → *nhớ và làm được* (2025) → *tính toán được* (2026). Mỗi lần "tốt" đổi nghĩa là một cột mốc; giữa hai lần đổi nghĩa chỉ là thi công.

Điểm đáng chú ý nhất: NotebookLM **chưa bao giờ đua "chatbot trả lời mọi thứ"**. Nó xây một lớp `nguồn có kiểm soát → nhiều dạng hiểu → học/quyết định` rồi mới mở distribution, pricing và segment lên trên lớp đó.

---

## §3. Các mốc đã cân nhắc và loại ra

| Mốc ứng viên | Vì sao **không** đủ tư cách là quyết định sản phẩm |
|---|---|
| **10/05/2023 — Project Tailwind demo tại I/O** | Là *thông báo ý định*, không phải quyết định đã thực thi: chưa có user, chưa có dữ liệu vào, chưa có vòng lặp. Quyết định thật nằm ở 07/2023 khi chốt ràng buộc source-grounding và mở cho user thật. Xếp vào Context của hàng 1. |
| **17/10/2024 — Bỏ nhãn "Experimental" + pilot Business** | Đổi *nhãn*, chưa đổi bốn thứ. Pilot chưa có giá, chưa có gói, chưa có entitlement. Quyết định monetization thật sự chốt ở 13/12/2024 với Plus — đưa 10/2024 vào Context hàng 4 thay vì cho một hàng riêng. |
| **03/04/2025 — Mind Maps + Discover Sources** | **Mind Map** là một artifact mới trong Studio — thi công đúng cái hộc đã dựng ở hàng 4, không phải hướng mới. **Discover Sources** thì đúng là mầm của một quyết định lớn, nhưng nó chỉ là gợi ý nguồn; quyết định thật (agent tự dựng cả danh sách nguồn) chín ở Deep Research 11/2025 — nên tính vào hàng 7. |
| **29/07 & 25/08/2025 — Video Overviews + 80 ngôn ngữ** | Đây là mốc **khó loại nhất**, và tiêu chí phân định là: *nó có tạo ra nguyên lý mới hay chỉ thi hành nguyên lý đã quyết?* Video Overview chạy đúng nguyên lý của Audio Overview (hàng 3): x10 ở khâu tiêu thụ. 80 ngôn ngữ mở rộng thị trường nhưng không đổi job, không đổi cách kiếm tiền, không đổi vòng lặp. → Ghi vào Context hàng 6 làm nền, không cho hàng riêng. *(Phản biện hợp lý: 80 ngôn ngữ đổi "ai dùng" ở quy mô lớn — nhóm chấp nhận đây là ranh giới mỏng nhất trong bảng.)* |
| **17/07/2025 — Featured Notebooks** | Có vẻ là quyết định (đổi "dữ liệu nào vào": từ user tự nạp → Google/publisher cấp sẵn). Nhưng nó dừng ở mức **thử nghiệm distribution/onboarding**, không đổi lõi và không có dấu hiệu trở thành trục chiến lược; bài toán cold-start mà nó nhắm tới bị Deep Research (hàng 7) giải triệt để hơn. Loại vì **bị hàng 7 hấp thụ**. |
| **13/10/2025 — Video Overviews dùng Nano Banana** | Thay model dưới nắp capo. Chất lượng lên, nhưng ai dùng / dữ liệu vào / output / cách kiếm tiền đều không đổi. Đây là *changelog*. |
| **03/2026 — chuyển sang Gemini 3.x** · **01/08/2026 — đổi domain** | Nâng cấp hạ tầng và địa chỉ. Không có quyết định sản phẩm nào phải cân nhắc đánh đổi ở đây. |
| **Toàn bộ version history App Store** (Drive Picker, notebook search, tải Slide PDF, push notification, two-click artifact, deep links…) | Đúng nghĩa changelog: giảm ma sát trong workflow đã có. Chúng là **bằng chứng** cho hướng đi ở hàng 5–6, không phải mốc. Đưa 14 mục này vào bảng chính là dấu hiệu sai đường mà brief cảnh báo. |
| **29/07/2025 — bài hậu trường về feedback loop qua form/Discord** | Là nguồn *phương pháp*, không phải mốc trên trục thời gian sản phẩm. Dùng cho §2/§4 của memo (cách Labs tìm PMF), không dùng ở §1. |

**Tóm tắt tiêu chí loại:** *(a)* thông báo ý định chưa thực thi, *(b)* đổi nhãn/hạ tầng/model dưới nắp capo, *(c)* thi hành một nguyên lý đã được quyết ở mốc trước, *(d)* bị một mốc sau hấp thụ hoàn toàn.

---

## §4. Nguồn

**Nguồn gốc (Google Blog) — độ tin cậy cao:**
- [Introducing NotebookLM (12/07/2023)](https://blog.google/innovation-and-ai/technology/ai/notebooklm-google-ai/)
- [NotebookLM goes global, Gemini 1.5 Pro (06/06/2024)](https://blog.google/innovation-and-ai/products/notebooklm-goes-global-support-for-websites-slides-fact-check/)
- [Audio Overviews (11/09/2024)](https://blog.google/innovation-and-ai/products/notebooklm-audio-overviews/)
- [Custom Audio + Business pilot (17/10/2024)](https://blog.google/innovation-and-ai/products/notebooklm-update-october-2024/)
- [NotebookLM Plus, UI ba khoang (13/12/2024)](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-new-features-december-2024/)
- [Mobile app (19/05/2025)](https://blog.google/innovation-and-ai/products/notebooklm-app/)
- [Video Overviews + Studio (29/07/2025)](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-video-overviews-studio-upgrades/)
- [80 ngôn ngữ (25/08/2025)](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebook-lm-audio-video-overviews-more-languages-longer-content/)
- [Learning features](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-student-features/) · [Flashcards & quizzes mobile (06/11/2025)](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-app-quizzes-flashcards/)
- [Đổi tên Gemini Notebook (16/07/2026)](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook/)

**Nguồn thứ cấp — dùng để đối chiếu, đã đánh dấu trong bảng:**
- [9to5Google — rename (16/07/2026)](https://9to5google.com/2026/07/16/notebooklm-gemini-notebook/) · [Glasp — Deep Research 11/2025](https://glasp.co/articles/notebooklm-2026) · [Product Hunt — NotebookLM Plus](https://www.producthunt.com/products/google-notebooklm-plus) · [Wikipedia — NotebookLM](https://en.wikipedia.org/wiki/NotebookLM)

**Cảnh báo nguồn cần lưu ý khi bảo vệ bài:**
- Mốc **Deep Research (11/2025)** hiện chỉ có nguồn thứ cấp (Glasp) trong kho step_0 — cần tìm bài công bố gốc của Google trước khi đưa vào memo cuối.
- Google Play **không công khai version history**; không suy diễn mốc Android lịch sử từ đó.
- App Store chỉ hiển thị một cửa sổ bản gần đây, thay đổi theo storefront — không phải archive vĩnh viễn.
