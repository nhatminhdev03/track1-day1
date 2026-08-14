# plan_step1 — Nhật ký tư duy & câu hỏi phản biện cho [Step1.md](Step1.md)

*Ghi lại cách nhóm đi từ 14 mốc ứng viên trong [step_0/](step_0/) xuống 8 cột mốc, và bộ câu hỏi để tự đập bảng của mình trước khi người khác đập.*

---

## 1. Bài toán thật của Step 1

Brief nói "chọn 6–8 mốc", nhưng cái khó không phải **cắt bớt** — mà là **có một tiêu chí cắt mà mình bảo vệ được**. Nếu không có tiêu chí, mọi lựa chọn đều thành "cái này nghe quan trọng hơn", và bảng rơi vào đúng hai cái bẫy brief cảnh báo:

- 15+ hàng toàn cập nhật nhỏ → liệt kê changelog
- nhãn kiểu "cái này để tăng trưởng" → không phải nguyên lý

Nên việc đầu tiên là **viết tiêu chí trước, rồi mới lọc**.

## 2. Tiêu chí đã chốt

**Một hàng chỉ được vào bảng nếu nó đổi ít nhất một trong bốn thứ:**

| # | Trục | Câu hỏi kiểm tra |
|---|---|---|
| 1 | Ai dùng | Tệp user có mở rộng/dịch chuyển không? |
| 2 | Dữ liệu nào vào | Loại nguồn / cách nạp nguồn có đổi không? |
| 3 | Output & workflow nào ra | Job-to-be-done có đổi không? |
| 4 | Kiếm tiền / giữ chân | Giá, gói, entitlement, switching cost có đổi không? |

Và **bốn dạng bị loại**: *(a)* thông báo ý định chưa thực thi · *(b)* đổi nhãn/hạ tầng/model dưới nắp capo · *(c)* thi hành một nguyên lý đã quyết ở mốc trước · *(d)* bị một mốc sau hấp thụ hoàn toàn.

Loại (c) là loại quan trọng nhất và cũng dễ bỏ sót nhất. Ví dụ Video Overviews (07/2025) trông rất "to" — nhưng nó chạy đúng nguyên lý đã quyết ở Audio Overviews (09/2024). Cho nó một hàng riêng là **đếm một quyết định hai lần**.

## 3. Đường đi từ 14 mốc → 8

| Bước | Việc làm | Kết quả |
|---|---|---|
| 1 | Gom mốc ứng viên từ cả 3 file step_0 (CP0 + bản nháp timeline + Product Hunt) | ~20 mốc thô, gồm cả 14 version App Store |
| 2 | Gạt toàn bộ version history App Store sang phụ lục | còn ~14 |
| 3 | Áp bộ lọc 4 trục | còn 11 |
| 4 | Áp loại (c) "thi hành nguyên lý cũ" và (d) "bị mốc sau hấp thụ" | còn 8 |
| 5 | Kiểm tra bảng có kể thành **một câu chuyện liền mạch** không | 8 hàng, đọc dọc ra một lập luận |

**Điểm bổ sung so với bản nháp có sẵn trong step_0:** bản nháp dừng ở 11/2025 và bỏ sót hai mốc lớn nhất về mặt chiến lược — **Deep Research** (tự đảo ngược ràng buộc sáng lập) và **đổi tên Gemini Notebook + cloud computer** (16/07/2026). Bản nháp đồng thời cho Video Overviews một hàng riêng, thứ mà bản này loại theo tiêu chí (c). Bảng mới kéo dài tới hiện tại (08/2026).

## 4. Vì sao cột "Nguyên lý" viết như vậy

Nguyên tắc tự đặt ra: **một nguyên lý phải nói được cái *đánh đổi* mà quyết định đó chấp nhận.** Nếu câu nguyên lý dán vào mốc nào cũng đúng thì nó là nhãn đại trà, không phải nguyên lý.

Test: thử tráo nguyên lý giữa hai hàng — nếu tráo được mà vẫn "nghe hợp lý" thì cả hai đều viết dở.

| Viết dở (nhãn đại trà) | Viết được (có đánh đổi, có tên) |
|---|---|
| "Audio để tăng trưởng" | "x10 ở khâu **tiêu thụ**, không phải khâu trả lời — đổi format là đổi *tình huống sử dụng*, mở ra thời gian mà chat không với tới" |
| "Plus để kiếm tiền" | "Bán **độ sâu workflow**, không bán token — và đặt tên khoang (Sources·Chat·Studio) trước khi lấp đầy" |
| "Mobile để giữ chân user" | "Đổi **điểm capture**, không đổi lõi — share sheet là một cửa nạp dữ liệu mới, không phải port giao diện" |
| "Đổi tên cho đồng bộ thương hiệu" | "Đổi **brand equity lấy distribution** — hy sinh nhận diện của 30M user để lấy entitlement của gói Gemini" |

## 5. Phát hiện lớn nhất khi revert nguyên lý

**Định nghĩa "tốt" của NotebookLM đổi nghĩa 4 lần — và mỗi lần đổi nghĩa là đúng một cột mốc.**

```
đúng & có bằng chứng (2023)
   → tiêu hoá được (2024)
      → nhớ và làm được (2025)
         → tính toán được trên tài liệu (2026)
```

Giữa hai lần "tốt" đổi nghĩa chỉ là thi công. Đây hoá ra là **tiêu chí lọc mốc mạnh nhất** — mạnh hơn cả bộ 4 trục, vì nó trả lời được câu "vì sao mốc này là *quyết định* chứ không phải *bản vá*".

Phát hiện thứ hai: **hàng 1 và hàng 7 mâu thuẫn nhau về mặt bề mặt** (2023 chốt "chỉ dùng nguồn của bạn" làm moat → 2025 để agent tự đi tìm nguồn). Đây là chỗ đáng khai thác nhất cho §3 dự đoán của memo: một sản phẩm dám tự phá ràng buộc sáng lập của mình khi ràng buộc đó chuyển từ *tạo niềm tin* sang *tạo ma sát* — nhưng chỉ phá ở tầng **thu thập**, giữ nguyên ở tầng **hiển thị**.

## 6. Chỗ yếu nhóm tự nhận

1. **Deep Research (11/2025)** hiện chỉ có nguồn thứ cấp (Glasp) trong kho step_0 → phải tìm bài công bố gốc của Google, hoặc hạ mốc này xuống và gộp vào hàng 8.
2. **Loại Video Overviews + 80 ngôn ngữ là ranh giới mỏng nhất trong bảng.** 80 ngôn ngữ đổi "ai dùng" ở quy mô lớn — có lập luận hợp lý để cho nó một hàng. Nhóm chọn loại và ghi rõ lý do thay vì giấu.
3. Cột **Context** có phần suy diễn (ví dụ "dữ liệu sử dụng cho thấy sinh viên là tệp lớn nhất") — chưa có số công khai chứng minh. Cần đánh dấu là giả thuyết khi bảo vệ.
4. Timeline này đọc lịch sử **từ phía Google**. Chưa có mốc nào phản ánh áp lực cạnh tranh trực tiếp (Perplexity, ChatGPT Projects, Claude Projects) — nếu có thời gian, nên bổ sung một lớp "đối thủ làm gì ngay trước mốc đó" vào cột Context.

---

## 7. Câu hỏi phản biện

### 7.1 Câu hỏi chính — *"Đâu là cột mốc nhóm đã cân nhắc rồi loại ra? Vì sao nó không đủ tư cách là quyết định sản phẩm?"*

**Trả lời gọn để bảo vệ trước lớp:**

> Mốc bị loại đáng tiếc nhất là **Video Overviews (29/07/2025) và mở 80 ngôn ngữ (25/08/2025)**.
>
> Nó không đủ tư cách vì tiêu chí phân định của nhóm không phải "mốc này to hay nhỏ", mà là **"nó tạo ra một nguyên lý mới, hay chỉ thi hành nguyên lý đã quyết trước đó?"**. Video Overview chạy đúng nguyên lý mà Audio Overview (09/2024) đã chốt: *x10 ở khâu tiêu thụ, biến notebook thành artifact chia sẻ được*. Cho nó một hàng riêng là đếm cùng một quyết định hai lần — và đó chính là cách một timeline trượt thành changelog.
>
> Ba mốc bị loại đáng nói tiếp theo, mỗi mốc một lý do khác nhau:
> - **Project Tailwind tại I/O (05/2023)** — thông báo ý định, chưa có user, chưa có vòng lặp. Quyết định thật nằm ở 07/2023.
> - **Bỏ nhãn Experimental (10/2024)** — đổi nhãn, chưa đổi giá/gói/entitlement. Quyết định monetization thật chốt ở 12/2024.
> - **Featured Notebooks (07/2025)** — đây là mốc khó xử nhất, vì nó *có* đổi "dữ liệu nào vào" (publisher cấp thay vì user nạp). Loại vì nó dừng ở thử nghiệm onboarding và bài toán nó nhắm tới (cold-start notebook trống) bị **Deep Research 11/2025 hấp thụ và giải triệt để hơn**.
>
> Chi tiết đầy đủ 9 nhóm mốc bị loại ở [§3 của Step1.md](Step1.md).

### 7.2 Bộ câu hỏi tự đập bảng

**Về việc chọn mốc**
1. Nếu xoá một hàng bất kỳ, câu chuyện có còn liền mạch không? Nếu còn → hàng đó không xứng đáng có mặt.
2. Có hàng nào chỉ vào bảng vì nó *nổi tiếng* (viral Audio) chứ không phải vì nó *đổi hướng* không?
3. Bảng có mốc nào là **quyết định KHÔNG làm** không? Timeline hiện chỉ toàn cái đã ship — mà quyết định lớn nhất của NotebookLM lại là một cái **không** làm: không đua chatbot vạn năng. Có nên cho "cái không làm" một chỗ đứng rõ hơn?
4. Nếu một nhóm khác cũng làm NotebookLM, họ có nhiều khả năng chọn 8 mốc nào? Chỗ mình khác họ, mình có lập luận không hay chỉ là khác?

**Về cột Nguyên lý**
5. Tráo nguyên lý hàng 3 sang hàng 6 — có "nghe vẫn hợp lý" không? Nếu có, cả hai đều viết chưa đủ sắc.
6. Nguyên lý nào trong bảng **dự đoán được** mốc tiếp theo? Một nguyên lý đúng phải có sức tiên đoán, không chỉ mô tả hậu nghiệm.
7. Có nguyên lý nào thực chất là "Google có tiền và có distribution" được nói tránh đi không? (Đây là rủi ro thật với một sản phẩm Big Tech — nhiều nước đi của NotebookLM **không** lặp lại được nếu bạn là startup.)

**Về cột Context**
8. Mỗi hàng có nêu được **đối thủ vừa làm gì** hoặc **model nào vừa mạnh lên** không, hay chỉ mô tả tình hình nội bộ Google? *(Đây là chỗ yếu đã tự nhận ở mục 6.4.)*
9. Có chỗ nào đang lẫn **tương quan** với **nhân quả** không — ví dụ "Gemini 1.5 Pro ra nên mở global", hay thực ra là "quyết định mở global có từ trước, model chỉ vừa kịp"?

**Về tính trung thực của bảng**
10. Có mốc nào **thất bại** không? Bảng hiện tại toàn nước đi thắng — điều đó thường có nghĩa là mình đang viết lịch sử theo lối *survivorship*, không phải theo chuỗi quyết định thật.
11. Nếu đổi tên Gemini Notebook (07/2026) hoá ra làm mất user, hàng 8 có còn được gọi là nguyên lý không, hay chỉ là một canh bạc chưa có kết quả?

---

## 8. Việc tiếp theo (bắc cầu sang Step 2)

- [ ] Tìm nguồn gốc Google cho **Deep Research 11/2025**; nếu không có → gộp vào hàng 8 và ghi rõ.
- [ ] Bổ sung lớp **đối thủ** vào cột Context cho hàng 3, 6, 7 (Perplexity, ChatGPT/Claude Projects).
- [ ] Map hàng 5, 6 sang **§2 dịch chuyển tệp user** của [memo-example.md](memo-example.md) — mobile + learning vertical là hai mốc gây dịch chuyển rõ nhất.
- [ ] Dùng mâu thuẫn hàng 1 ↔ hàng 7 làm hạt giống cho **§3 dự đoán**: ràng buộc nào của sản phẩm sẽ là ràng buộc tiếp theo bị chính nó phá?
