# NotebookLM — Timeline theo chuỗi quyết định sản phẩm

> Mục tiêu: đọc NotebookLM như một chuỗi quyết định sản phẩm, không phải changelog.  
> Lưu ý: cột **Cập nhật** là dữ kiện có dẫn nguồn; **Context** và **Nguyên lý** là diễn giải chiến lược. Đây **không phải App Store-only timeline**: app mobile chỉ ra mắt ngày 19/05/2025, nên các mốc 2023–2024 được dẫn từ công bố chính thức của Google về sản phẩm web.

| Thời điểm | Cập nhật | Context lúc đó | Nguyên lý |
|---|---|---|---|
| 07/2023 | **Ra mắt NotebookLM / Project Tailwind:** chat nhưng bị ràng buộc bởi nguồn người dùng chọn, có citation. | ChatGPT đã tạo ra kỳ vọng về chatbot đa năng từ 11/2022. Google không làm thêm một chatbot “biết tuốt”, mà bắt đầu từ bài toán đáng tin cậy với tài liệu riêng của người dùng. [OpenAI — ChatGPT](https://openai.com/index/chatgpt/) · [Google — NotebookLM](https://blog.google/innovation-and-ai/technology/ai/notebooklm-google-ai/) | **Wrapper/moat + định nghĩa “tốt” khác.** “Tốt” không phải trả lời hay nhất trên Internet, mà là giúp hiểu bộ tài liệu của tôi và chỉ được bằng chứng. Nguồn dữ liệu + trích dẫn là lớp sản phẩm nằm trên model. |
| 06/2024 | **Mở toàn cầu** (200+ quốc gia), dùng Gemini 1.5 Pro; mở nguồn từ Docs/PDF sang Slides, URL và xử lý hình/charts. [Google](https://blog.google/innovation-and-ai/products/notebooklm-goes-global-support-for-websites-slides-fact-check/) | Product chuyển từ Labs thử nghiệm thành bề mặt phân phối toàn cầu; model long-context, multimodal khiến “notebook” có thể chứa loại tài liệu thực tế hơn. | **x10 workflow.** Không yêu cầu người dùng chuẩn hóa dữ liệu trước; đem AI tới đúng “đống tài liệu lộn xộn” nơi công việc nghiên cứu diễn ra. Mở input là mở rộng moat dữ liệu/workflow. |
| 09/2024 | **Audio Overviews:** biến nguồn thành cuộc hội thoại podcast hai host, có thể tải về. [Google](https://blog.google/innovation-and-ai/products/notebooklm-audio-overviews/) | AI tiêu dùng đang cạnh tranh attention; Google tìm một output không phải “bản tóm tắt văn bản” mà là trải nghiệm tiêu thụ kiến thức mới. Đây cũng là bước biến research tool thành learning product. | **Định nghĩa “tốt” theo outcome.** Giá trị không dừng ở câu trả lời đúng: người dùng phải *tiêu hoá và nhớ được* nội dung. Audio là một “format moat” khó thay bằng chat UI thuần. |
| 12/2024 | **Đóng gói lại thành Sources–Chat–Studio**, cho tương tác trực tiếp với Audio host và ra mắt **NotebookLM Plus**. [Google](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-new-features-december-2024/) | Product đã có “millions of users” và “tens of thousands of organizations”; Google bắt đầu monetize cho power user, team, enterprise/education, đồng thời rollout Gemini 2.0 Flash. | **Từ feature sang hệ điều hành workflow + pricing theo độ sâu sử dụng.** Plus bán limit cao hơn, customization, shared notebook, analytics và bảo mật tổ chức — tức bán *workflow/team moat*, không chỉ bán token/model. |
| 05/2025 | **Ra iOS và Android:** offline/background Audio, share web/PDF/YouTube vào NotebookLM, hỏi nguồn ngay trong lúc sử dụng. [NotebookLM mobile](https://blog.google/innovation-and-ai/products/notebooklm-app/) | Người dùng đã yêu cầu mobile; cùng thời điểm I/O, Gemini 2.5 Flash trở thành model mặc định trong Gemini nhờ cân bằng chất lượng/tốc độ. [Gemini 2.5 Flash](https://blog.google/products-and-platforms/products/gemini/gemini-app-updates-io-2025/) | **Vòng lặp học + capture point.** Điểm vào không còn là “ngồi xuống nghiên cứu”; gặp một nguồn khi đang lướt/di chuyển → gửi vào notebook → nghe/hỏi → quay lại nguồn. Product đi tới nơi dữ liệu và attention xuất hiện. |
| 07–08/2025 | **Video Overviews**, sau đó mở sang **80 ngôn ngữ**; Audio ngoài tiếng Anh cũng nâng từ short-form lên full-length. [Google](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebook-lm-audio-video-overviews-more-languages-longer-content/) | Khi năng lực multimodal/generative media tăng nhanh, Google chuyển từ một modality “nghe” sang một hệ output đa phương thức và toàn cầu. | **x10 accessibility, không chỉ thêm format.** Cùng một notebook có thể được hiểu bằng text, audio, video, bằng ngôn ngữ quen thuộc. Mở rộng thị trường nhưng vẫn giữ lõi “grounded in your sources”. |
| 09–11/2025 | **Pivot rõ sang learning vertical:** Flashcards, Quizzes, Learning Guide, reports tùy biến, notebook học liệu tin cậy; đưa các khả năng này lên mobile. [Learning features](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-student-features/) · [Mobile update](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-app-quizzes-flashcards/) | Mùa back-to-school, Google đồng thời đẩy Gemini/education; mục tiêu chuyển người dùng từ đọc thụ động sang ôn tập, kiểm tra hiểu biết, được giải thích theo tài liệu lớp học. | **Vertical AI + vòng lặp học.** Đây là “verticalization” theo job-to-be-done: input là tài liệu học, output là flashcard/quiz/guide, feedback là câu sai và giải thích có citation. “Tốt” được đo bằng hiểu sâu/ghi nhớ, không phải chỉ tạo nội dung nhanh. |

## Vì sao chọn các mốc này mà loại các mốc kia?

- Tôi chọn mốc khi nó thay đổi ít nhất một trong bốn thứ: **ai dùng**, **dữ liệu nào đi vào**, **output/workflow nào được tạo ra**, hoặc **Google kiếm tiền/giữ chân như thế nào**. Vì vậy Audio Overview, Plus, mobile và learning vertical là các quyết định; một bản “bug fix” không phải.
- Các mốc như Drive Picker, search notebook hay tải PDF là evidence cho hướng mobile/workflow, nhưng không phải hướng chiến lược mới. Chúng được gộp vào mốc mobile thay vì biến timeline thành changelog.
- Điểm đáng chú ý nhất: NotebookLM không chạy cuộc đua “chatbot trả lời mọi thứ”. Nó nhất quán xây lớp **grounded sources → nhiều dạng hiểu biết → học/ra quyết định**, rồi mới mở rộng distribution, pricing và segment.

## Nguồn chính

- [Google: NotebookLM — source grounding](https://blog.google/innovation-and-ai/technology/ai/notebooklm-google-ai/)
- [Google: global rollout với Gemini 1.5 Pro](https://blog.google/innovation-and-ai/products/notebooklm-goes-global-support-for-websites-slides-fact-check/)
- [Google: Audio Overviews](https://blog.google/innovation-and-ai/products/notebooklm-audio-overviews/)
- [Google: NotebookLM Plus, Studio, Gemini 2.0 Flash](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-new-features-december-2024/)
- [Google: ứng dụng mobile](https://blog.google/innovation-and-ai/products/notebooklm-app/)
- [Google: Video Overview và 80 ngôn ngữ](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebook-lm-audio-video-overviews-more-languages-longer-content/)
- [Google: learning features](https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-student-features/)

## Dẫn chứng trực tiếp từ App Store và Google Play

| Store | Dữ kiện kiểm chứng được | Cách dùng trong timeline |
|---|---|---|
| [Apple App Store Việt Nam — Gemini Notebook (App ID 6737527615)](https://apps.apple.com/vn/app/google-notebooklm/id6737527615) | Mục **Version History** công khai từng version và ghi chú phát hành. Các mốc mobile: v1.37.7 (Reports), v1.38.7 (Drive Picker), v1.40.7 (notebook sharing), v1.41.7 (notebook search/tải Slide Deck PDF), v1.46.5 (tab mới, short Video Overview, xem PDF), v1.47.6 (đổi tên Gemini Notebook), v1.51.1 (artifact attribution và file formats). | Dùng để **xác thực các mốc release mobile**; bản vá và cải tiến hẹp được gộp, không thành cột mốc chiến lược riêng. |
| [Google Play — Gemini Notebook (package `com.google.android.apps.labs.language.tailwind`)](https://play.google.com/store/apps/details?id=com.google.android.apps.labs.language.tailwind) | Xác nhận app Android chính chủ Google LLC, package chính xác, ngày cập nhật và mục **What’s new** hiện hành; hiện ghi: “NotebookLM is now called Gemini Notebook.” | Google Play **không hiển thị version history/changelog cũ công khai trên web**. Vì vậy không dùng Play làm bằng chứng duy nhất cho các mốc Android lịch sử; dùng nó để xác nhận listing chính thức và dùng blog Google cho mốc ra mắt/chuyển hướng lớn. |

**Kết luận về nguồn:**

- **Trước 19/05/2025:** chưa có app mobile; không thể có release notes App Store/Google Play. Mốc này phải dẫn từ các bài công bố chính thức của Google về NotebookLM web.
- **Từ 19/05/2025:** App Store là bằng chứng trực tiếp tốt nhất cho một phần version history iOS. Tuy nhiên Apple chỉ hiển thị một cửa sổ các bản gần đây và có thể thay đổi theo storefront; không phải archive đầy đủ, vĩnh viễn.
- Google Play chỉ cho phép kiểm chứng bản hiện hành, nên không dùng làm chứng cứ duy nhất cho các mốc Android lịch sử.

## Phụ lục A — Release notes native có thể kiểm chứng trực tiếp

**Đính chính quan trọng:** ứng dụng NotebookLM chính thức chỉ phát hành trên **App Store và Google Play vào ngày 19/05/2025**. Vì vậy, không có “release App Store/CH Play” của NotebookLM cho các năm 2023–2024. [Google, *Understand anything, anywhere with the new NotebookLM app*, 19/05/2025](https://blog.google/innovation-and-ai/products/notebooklm-app/)

### A.1 App Store (iOS/iPadOS)

Nguồn duy nhất cho bảng dưới đây là **[Version History trên Apple App Store Việt Nam](https://apps.apple.com/vn/app/google-notebooklm/id6737527615)**, App ID `6737527615`, nhà phát hành Google LLC. Apple hiển thị ngày theo năm hiện hành; các ngày dưới đây được chép từ snapshot storefront VN truy cập ngày 14/08/2026.

| Version · ngày hiển thị | Nội dung release note của Apple | Ý nghĩa ngắn |
|---|---|---|
| 1.23.3 · 02/02/2026 | Tạo Video Overviews; tùy biến infographic (orientation, ngôn ngữ, prompt); tùy biến Slides (Detailed/Presenter, độ dài, ngôn ngữ, prompt); nêu gói Ultra với quota cao hơn. | Đưa “artifact generation” thành bề mặt sản phẩm có thể tùy biến và gắn với tier trả phí. |
| 1.28.10 · 26/02/2026 | Tùy biến Video Overview (Explainer/Brief, chọn nguồn, 8 visual styles/prompt); mở source trong Drive; Chat Suggestions. | Tăng quyền kiểm soát output và nối workflow với Drive. |
| 1.29.8 · 05/03/2026 | Slide Deck Revisions bằng prompt. | Chuyển từ tạo một lần sang vòng lặp chỉnh sửa. |
| 1.30.10 · 12/03/2026 | Push notification khi tạo artifact hoàn tất, kể cả khi rời app. | Cho phép generation chạy nền trên mobile. |
| 1.32.7 · 27/03/2026 | Deep Links mở notebook/artifact trong app; Cinematic Video Overviews cho AI Ultra (English); LaTex rendering trong Chat. | Mobile được nối sâu hơn với web và mở output cao cấp theo tier. |
| 1.33.7 · 10/04/2026 | Cinematic Video Overviews mở thêm cho AI Pro và một số Workspace; Chat Streaming và Thinking. | Mở rộng entitlement và làm reasoning hữu hình trong UX. |
| 1.36.6 · 24/04/2026 | Xem notes tạo trên web trong app; chia sẻ artifact và quản lý quyền truy cập từ mobile. | Đồng bộ web–mobile và bổ sung collaboration. |
| 1.37.7 · 03/05/2026 | Tạo Reports trên mobile: Study Guide, Briefing Doc, Blog Post. | Đưa workflow tạo output từ web sang mobile. |
| 1.38.7 · 08/05/2026 | Drive Picker để thêm file Google Drive làm source. | Giảm ma sát ở bước nạp dữ liệu. |
| 1.40.7 · 22/05/2026 | Notebook sharing để cộng tác; hai cách mở hộp customization artifact. | Collaboration xuất hiện ở mobile; tinh chỉnh discoverability. |
| 1.41.7 · 29/05/2026 | Tìm notebook theo tên; tải Slide Deck thành PDF về điện thoại. | Quản lý thư viện và export output. |
| 1.46.5 · 30/06/2026 | Thay “Recent/Title” bằng “My notebooks/Shared”; Short Video Overviews dọc ~60 giây; xem PDF gốc trong source panel. | Tái cấu trúc navigation theo ownership/collaboration, thêm format tiêu thụ nhanh. |
| 1.47.6 · 16/07/2026 | “NotebookLM is now called Gemini Notebook.” | Đổi tên sản phẩm. |
| 1.49.7 · ngày hiển thị “5 days ago” trong snapshot | Two-click artifact generation: chạm tile mở customization trước khi generation chạy. | Chuẩn hóa hành vi tạo artifact có kiểm soát. |

### A.2 Google Play (Android)

Google Play không cung cấp danh sách version history công khai tương đương App Store. Tại snapshot trang chính thức, phần **What’s new** chỉ ghi: **“NotebookLM is now called Gemini Notebook.”** Trang xác nhận package `com.google.android.apps.labs.language.tailwind` và nhà phát hành Google LLC. [Google Play — Gemini Notebook](https://play.google.com/store/apps/details?id=com.google.android.apps.labs.language.tailwind)

Do đó, không suy diễn số version, ngày phát hành hay release note lịch sử Android từ Play. Những mốc Android trước đó chỉ được dùng khi có công bố Google nêu rõ phát hành trên cả hai nền tảng.

## Phụ lục B — Nguồn cho các mốc trước khi có mobile app

Các mục sau là **lịch sử sản phẩm web**, không phải release notes App Store/Google Play:

1. Martin, Raiza; Johnson, Steven. **“Introducing NotebookLM.”** Google Blog, 12/07/2023. Ra mắt NotebookLM từ Project Tailwind cho nhóm nhỏ người dùng Hoa Kỳ; mô tả source grounding. https://blog.google/innovation-and-ai/technology/ai/notebooklm-google-ai/
2. Johnson, Steven; Martin, Raiza. **“NotebookLM goes global with Slides support and better ways to fact-check.”** Google Blog, 06/06/2024. Mở trên hơn 200 quốc gia/vùng lãnh thổ, dùng Gemini 1.5 Pro, hỗ trợ Slides/URL, citations và Notebook Guide. https://blog.google/innovation-and-ai/products/notebooklm-goes-global-support-for-websites-slides-fact-check/
3. Wang, Biao. **“NotebookLM now lets you listen to a conversation about your sources.”** Google Blog, 11/09/2024. Ra mắt Audio Overviews. https://blog.google/innovation-and-ai/products/notebooklm-audio-overviews/
4. Johnson, Steven. **“NotebookLM gets a new look, audio interactivity and a premium version.”** Google Blog, 13/12/2024. Ra mắt Sources–Chat–Studio, Interactive Audio và NotebookLM Plus; nêu rollout Gemini 2.0 Flash. https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-new-features-december-2024/
