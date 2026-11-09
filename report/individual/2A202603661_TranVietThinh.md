# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Việt Thịnh
- MSSV: 2A202603661
- Email trường (không bắt buộc, repo có thể để public): 26ai.thinhtv@vinuni.edu.vn
- Tên nhóm: Trustmebro
- Link repo nhóm: https://github.com/Tsou0911/K5-L3A-DAY02-Trustmebro-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Pain từ người khác |Khi tôi muốn phát triển tính năng mới và đưa các requirement cho designer, designer muốn rõ ràng vấn đề để không phải hỏi lại |PM, Designer, Developer |Mỗi khi làm thì designer phải hỏi lại 2-3 lần |
| 2 |Pain từ người khác |Mỗi khi tôi code xong 1 task nào đó, đã đẩy lên môi trường dev, nhưng do mới đi làm nên mắc rất nhiều lỗi cơ bản như (convention code, format code) làm tốn thời gian review của tech lead, thay vào đó tech lead có thể dành thời gian review logic hơn |Developer, Tech Lead |Sprint lâu được release, bình thường 2 tuần release 1 lần nhưng mất thời gian lên đến cả tháng |
| 3 |Tốn thời gian |Khi tôi gia nhập 1 công ty startup mới, không có tài liệu để tôi đọc về dự án |Developer |Tôi phải đi đọc code base suốt 1 tuần để có thể hiểu, sau đó lúc vào làm phát triển tính năng mới cũng phải đọc lại lần nữa để có thể follow theo code base |
| 4 |Cần đọc, tổng hợp nhiều thông tin |Khi tôi nhận một bug report từ QA hoặc khách hàng (kèm log, screenshot, mô tả rời rạc), tôi muốn nhanh chóng khoanh vùng được nguyên nhân và đoạn code liên quan, để sửa lỗi mà không phải lần mò qua nhiều file và nhiều nguồn thông tin |Developer, QA |Mỗi bug mất khoảng 1-3 giờ chỉ để tái hiện và xác định đúng chỗ lỗi; xảy ra vài lần mỗi tuần; phải hỏi lại QA để lấy thêm thông tin về bước tái hiện |
| 5 |Lặp lại |Khi tôi viết một tính năng mới, tôi muốn có sẵn khung code, test và cấu trúc theo đúng convention của dự án, để không phải viết lại phần boilerplate (API call, xử lý lỗi, form, unit test) giống nhau mỗi lần |Developer |Mỗi tính năng tốn khoảng 1-2 giờ cho phần boilerplate; lặp lại ở mọi task; code mỗi người viết một kiểu nên khó đồng nhất |
| 6 |Tốn thời gian |Khi tôi cần cập nhật tiến độ cho PM (daily standup, báo cáo sprint, ghi chú release), tôi muốn tổng hợp tự động từ commit, PR và task đã làm, để không mất thời gian ngồi nhớ lại và viết tay |Developer, PM |Mỗi ngày mất 10-15 phút cho standup, cuối sprint mất thêm 1-2 giờ viết báo cáo; thông tin hay thiếu hoặc không khớp với thực tế code |
| 7 |Pain từ người khác |Khi PM hoặc stakeholder đổi yêu cầu giữa sprint hoặc mô tả yêu cầu mơ hồ, tôi muốn có chỗ ghi lại rõ yêu cầu và những thay đổi, để không phải làm lại phần đã xong hoặc tranh cãi về việc “ban đầu yêu cầu là gì” |Developer, PM, Designer |Cứ vài sprint lại có task phải làm lại một phần; mất 0,5-2 ngày công cho mỗi lần đổi yêu cầu; không có tài liệu để đối chiếu |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-Tôi dùng AI đển tạo ra gợi ý từ 4-7. Theo tôi thì nên giữ lại 4 và bỏ đi 5, 6, 7. Gợi ý 5 thì có pain thật nhưng khá chung chung, mơ hồ. Gợi ý 7 thì trùng với gợi ý 1 của tôi viết. Gợi ý 6 thì hiện nay có nhiều công cụ như Jira có thể tracking được những gì đã làm

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Problem #3 Vào startup mới, không có tài liệu về dự án |Pain có thật và đã có bằng chứng: đọc code ~1 tuần, rồi lại đọc lại mỗi tính năng mới. |Người mới thực tế mất bao nhiêu ngày? Tài liệu AI sinh có đủ chính xác không? |
| 2 |Problem #2 Review chậm vì lỗi cơ bản (convention, format) |Bằng chứng mạnh nhất về thời gian: release dự kiến 2 tuần nhưng thực tế kéo dài đến cả tháng, ảnh hưởng cả Developer lẫn Tech Lead. |Bao nhiêu phần của độ trễ là do lỗi convention, bao nhiêu là do Tech Lead quá tải? Nếu chủ yếu là format thì linter đã đủ, không cần AI. |
| 3 |Problem #4 Khoanh vùng bug từ báo cáo rời rạc |Khác hẳn 2 problem trên (đọc và tổng hợp nhiều nguồn), nên top 3 không bị trùng ý. |Con số 1-3 giờ mỗi bug và tần suất vài lần mỗi tuần là ước lượng, chưa phải số thật của nhóm. Cần đo lại trước khi giữ. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi vừa gia nhập một dự án startup chưa có tài liệu, tôi muốn có sẵn bản mô tả dự án để hiểu nhanh và bắt đầu làm việc, thay vì tự đọc code cả tuần|
| Actor |Developer mới vào team |
| Thời điểm / bối cảnh |Tuần đầu khi vào dự án, và mỗi lần bắt đầu một tính năng mới cần biết dùng component nào |
| Quy trình hiện tại (3–7 bước) |1. Clone repo, tự tìm cách chạy · 2. Đọc code từng file · 3. Hỏi người cũ khi bí · 4. Tự ghi chú để nhớ · 5. Khi làm tính năng mới, đọc lại để tìm component phù hợp |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2, đọc code để hiểu cấu trúc và quan hệ giữa các phần: khoảng 1 tuần |
| Impact (nếu không giải thì sao) |1 tuần cho mỗi người mới |
| Success metric (baseline → target) |Số ngày để làm task đầu tiên từ 1 tuần xuống 1 ngày; số lần phải hỏi người cũ không tăng |
| Phương án không dùng AI |Template onboarding viết tay + ADR cho quyết định mới + phân công người kèm (buddy): có thêm “vì sao”, nhưng cần người viết và chưa giải quyết phần code cũ |
| Giả thuyết về AI (nếu có) |AI soạn bản nháp tài liệu từ code (tổng quan, kiến trúc, cách chạy, component dùng chung); developer chính duyệt và bổ sung trước khi đăng |
| Cảm nhận nhanh | Workflow | 

Quy trình nháp hiện tại:

```Vào team → Chạy được dự án → Đọc code → Hỏi người cũ → Ghi chú cá nhân → Làm tính năng (quay lại đọc code).

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi tôi đẩy code lên môi trường dev, tôi muốn các lỗi cơ bản (convention, format) được bắt trước, để Tech Lead chỉ phải review logic |
| Actor | 	Developer mới, Tech Lead (người review)|
| Thời điểm / bối cảnh |Sau khi hoàn thành task, trước khi Tech Lead review để lên production|
| Quy trình hiện tại (3–7 bước) |1. Dev code xong, đẩy lên dev · 2. Chờ Tech Lead review · 3. Tech Lead phát hiện lỗi convention/format và cả vấn đề logic · 4. Dev sửa · 5. Review lại · 6. Approve và deploy |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2 và 3: Tech Lead nhiều việc nên review chậm, lại mất thời gian vào lỗi cơ bản |
| Impact (nếu không giải thì sao) |Release dự kiến 2 tuần nhưng có khi kéo dài cả tháng, ảnh hưởng dev, 1 Tech Lead nhiều vòng sửa mỗi task |
| Success metric (baseline → target) |Thời gian từ “xong code” đến “approve” từ 7 ngày xuống 1 ngày, số comment về convention/format trong review giảm |
| Phương án không dùng AI |Linter, formatter, pre-commit hook và CI bắt buộc + checklist PR: bắt được lỗi format tự động, chưa bắt được quy ước ngầm của team |
| Giả thuyết về AI (nếu có) |AI review sơ bộ PR theo quy ước của dự án và gắn comment, dev sửa trước khi gửi Tech Lead |
| Cảm nhận nhanh | Rule (linter) trước, Workflow nếu còn lỗi linter không bắt được|

Quy trình nháp hiện tại:

```Code xong → Đẩy lên môi trường dev → Chờ Tech Lead review → Tech Lead review (cả convention lẫn logic) → Dev sửa theo comment → Review lại → Approve → Deploy production

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận bug report rời rạc (log, screenshot, mô tả), tôi muốn nhanh chóng biết nguyên nhân và đoạn code liên quan, để sửa lỗi mà không phải lần mò qua nhiều file|
| Actor |	Developer; QA (người báo bug) |
| Thời điểm / bối cảnh |Khi QA hoặc khách hàng báo bug trong sprint hoặc sau release |
| Quy trình hiện tại (3–7 bước) |1. Đọc bug report · 2. Hỏi lại QA về bước tái hiện · 3. Tự tái hiện lỗi · 4. Đọc log, lần theo code · 5. Xác định chỗ lỗi · 6. Sửa và test |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2 đến 5: thiếu thông tin, phải hỏi lại rồi lần mò qua nhiều file |
| Impact (nếu không giải thì sao) |	~1-3 giờ mỗi bug chỉ để khoanh vùng; vài lần mỗi tuần; ___ dev và QA bị ảnh hưởng (số hiện là ước lượng, cần đo thật) |
| Success metric (baseline → target) |Thời gian từ nhận bug đến xác định chỗ lỗi từ 4 xuống 1 lần hỏi lại QA giảm |
| Phương án không dùng AI |Template bug report bắt buộc (bước tái hiện, môi trường, log) + công cụ giám sát lỗi như Sentry: thông tin đầy đủ hơn, chưa chỉ ra chỗ lỗi trong code |
| Giả thuyết về AI (nếu có) |AI đọc bug report, log và code để gợi ý file/hàm nghi ngờ; dev xác nhận trước khi sửa |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```Nhận bug report → Hỏi lại QA bước tái hiện → Tự tái hiện lỗi → Đọc log, lần theo code → Xác định chỗ lỗi → Sửa và test

```

### Card muốn pitch nhất

- Card số: Card số: #1 (thiếu tài liệu onboarding)
- Vì sao: Đây là card nhóm đã phân tích sâu nhất, nỗi đau rõ (~1 tuần đọc code, lại đọc lại mỗi tính năng mới) và hợp với AI ở chỗ phần lớn thông tin cần đọc nằm sẵn trong code.
- Câu hỏi muốn nhóm phản biện: Nếu AI chỉ sinh được “code làm gì” mà không biết “vì sao thiết kế như vậy”, bản nháp đó có đủ giúp người mới không, hay vẫn phải hỏi người cũ như trước?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|Impact thiếu số thật: chỉ có “1 tuần” từ một người. Nếu startup ít tuyển người mới thì giá trị thấp. |Đồng ý |Thêm số người mới mỗi năm và khảo sát 3-5 người từng onboard. |
|AI không biết phần “vì sao” và quy trình nội bộ, bản nháp có thể thiếu hoặc sai. |Đồng ý |Thêm mục “Chưa biết, cần người bổ sung”, kèm link tới code để đối chiếu và ADR cho quyết định mới.|
|Đã có công cụ sẵn (DeepWiki, Code Wiki), sao phải tự dựng? |Đồng ý |Ghi rõ điều kiện: repo public thì thử công cụ có sẵn trước; chỉ dựng riêng nếu repo private hoặc công cụ không đạt. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
