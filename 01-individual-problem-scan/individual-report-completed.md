# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: **[Bạn điền họ và tên]**
- Mã học viên: **[Bạn điền mã học viên]**
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): **Kỹ sư AI tại công ty công nghệ, tham gia phát triển mã nguồn giải pháp AI và phối hợp code với các kỹ sư khác qua Git.**
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
  - Phát triển feature, sửa bug và tối ưu mã nguồn cho giải pháp AI.
  - Tạo branch, commit, pull/push và đồng bộ code với các nhánh của đồng nghiệp.
  - Review thay đổi mã nguồn/PR và kiểm tra ảnh hưởng tới các module liên quan.
  - Merge code, xử lý merge conflict và chạy lại build/test sau khi resolve.
  - Debug regression hoặc lỗi phát sinh sau khi tích hợp thay đổi từ nhiều người.

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

> **Lưu ý về số liệu:** Tôi chưa có log đo chính thức cho tất cả các problem. Các con số bên dưới là **baseline ước lượng ban đầu từ workflow hiện tại**, cần xác nhận lại bằng `git log`, lịch sử PR/MR, CI log và bấm giờ trong 1-2 tuần.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Lặp lại + Tốn thời gian | Khi merge nhánh của đồng nghiệp vào nhánh đang phát triển, tôi phải dừng công việc chính để đọc conflict và quyết định giữ/sửa phần code nào. | Tôi và kỹ sư cùng sửa các module liên quan | Ước lượng **2-4 lần/tuần**, khoảng **15-45 phút/lần**. Cần xác nhận bằng lịch sử merge/PR và bấm giờ. |
| 2 | Tốn thời gian + AI có thể tốt hơn | Sau khi resolve conflict hoặc merge thành công, tôi không biết chắc thay đổi vừa tích hợp ảnh hưởng tới module, API hoặc luồng xử lý nào khác nên phải đọc diff và test thủ công. | Tôi, reviewer và các kỹ sư phụ thuộc vào module đó | Ước lượng **20-60 phút/lần merge lớn** để đọc diff và test. Cần đo lại trên tối thiểu 5 lần merge. |
| 3 | Pain từ người khác + Lặp lại | Hai người có thể cùng sửa một file hoặc vùng logic liên quan mà không biết trước; tới lúc merge mới phát hiện xung đột. | Các kỹ sư làm song song trên cùng codebase | Ước lượng **1-3 tình huống/tuần** khi nhiều feature chạy song song. Có thể kiểm bằng PR/commit chạm cùng file. |
| 4 | AI có thể tốt hơn + Tốn thời gian | Khi review PR của đồng nghiệp, tôi phải tự lần theo nhiều file để hiểu thay đổi ảnh hưởng tới luồng AI, API, data flow hoặc dependency nào. | Tôi và code reviewer | Ước lượng **20-40 phút/PR** nếu chạm nhiều module. Cần bấm giờ trên tối thiểu 5 PR. |
| 5 | Lặp lại | Sau mỗi lần merge/resolve conflict, tôi phải lặp lại build, test, lint hoặc chạy thử luồng chính để kiểm tra code vẫn hoạt động. | Tôi và team phát triển | Xảy ra gần như **mỗi lần merge**, ước lượng **10-30 phút/lần**. Có thể xác nhận qua CI log/terminal history. |
| 6 | Tốn thời gian + Pain từ người khác | Khi conflict liên quan tới code do người khác viết, tôi thiếu context về lý do họ thay đổi nên phải đọc commit cũ hoặc hỏi trực tiếp đồng nghiệp. | Tôi và tác giả phần code liên quan | Ước lượng **1-2 lần/tuần**, khoảng **10-30 phút/lần**. Có thể kiểm bằng chat/PR comment và `git log`. |
| 7 | AI có thể tốt hơn | Diff sau merge có thể dài; tôi chưa có cách tự động tóm tắt “thay đổi gì, ảnh hưởng đâu, cần kiểm tra gì” theo ngữ cảnh codebase. | Tôi, reviewer và maintainer | Với merge lớn, việc đọc diff + tự lập checklist ước lượng **15-30 phút/lần**. Cần log kích thước diff và thời gian review. |
| 8 | Pain từ người khác + Tốn thời gian | Khi merge gây regression, việc truy ngược commit hoặc quyết định resolve nào gây lỗi mất thời gian vì không có impact note rõ tại thời điểm merge. | Tôi, maintainer và QA | Một lần regression có thể tốn khoảng **30-120 phút** để khoanh vùng. Cần xác nhận bằng issue/bug/incident log. |
| 9 | Lặp lại + Tốn thời gian | Tôi phải chuyển liên tục giữa IDE, terminal, Git, PR và tài liệu để hiểu trạng thái thay đổi, làm gián đoạn flow phát triển feature chính. | Tôi | Ước lượng bị ngắt luồng **3-6 lần/ngày**, mất **5-15 phút/lần** để lấy lại context. Nên self-log trong 5 ngày. |
| 10 | AI có thể tốt hơn + Pain từ người khác | Team chưa có bước chuẩn để đánh giá risk trước/sau merge: file nào nhạy cảm, test nào bắt buộc, module nào có thể bị ảnh hưởng, ai nên review. | Cả team phát triển | Ước lượng **2-5 PR/merge mỗi tuần** cần đánh giá thủ công. Cần đối chiếu quy trình PR và review log hiện tại. |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: Từ bối cảnh tôi là kỹ sư AI vừa phát triển mã nguồn vừa thường xuyên merge code với đồng nghiệp, hãy phản biện và gợi ý thêm problem theo 4 lăng kính: lặp lại, tốn thời gian, AI có thể tốt hơn và pain từ người khác. Không bắt đầu từ solution.
- Ý dùng được: khó đánh giá impact sau merge; merge conflict làm gián đoạn coding; thiếu context khi resolve code của người khác; đọc diff và xác định test cần chạy tốn thời gian; khó truy nguyên regression sau merge.
- Ý bỏ vì không phải pain thật: “AI tự merge mọi PR”, “coding agent tự sửa toàn bộ codebase”, hoặc các bài toán quá rộng/chưa từng quan sát trong workflow hiện tại.

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Sau khi resolve conflict hoặc merge thành công, tôi không biết chắc thay đổi vừa tích hợp ảnh hưởng tới module/API/luồng nào khác. | Workflow xảy ra thường xuyên; bottleneck “đánh giá impact” rõ; có thể đo bằng thời gian review/test và số regression lọt qua. | Chưa có baseline thật về số phút và tỷ lệ regression sau merge; cần log 1-2 tuần. |
| 2 | Khi conflict liên quan tới code người khác viết, tôi thiếu context để quyết định cách resolve đúng. | Actor và thời điểm rõ; conflict tạo gián đoạn trực tiếp; có thể đo số lần phải hỏi đồng nghiệp và thời gian resolve. | Không phải conflict nào cũng cần AI; một phần có thể giải bằng ownership/quy ước branch tốt hơn. |
| 3 | Khi review PR, tôi phải tự lần theo nhiều file để biết thay đổi ảnh hưởng đâu và cần chạy test nào. | Workflow review rõ; pain lặp lại; có thể đo thời gian review, số file phải trace và số lỗi phát hiện trước merge. | Chưa biết codebase hiện có dependency graph/test mapping đủ tốt để tự động hóa bằng rule hay không. |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Khó đánh giá tác động sau merge / resolve conflict

```text
Problem 1 câu:
Sau khi merge hoặc resolve conflict, tôi mất nhiều thời gian đọc diff và chạy kiểm tra thủ công nhưng vẫn không biết chắc thay đổi vừa tích hợp có ảnh hưởng tới module, API, data flow hoặc luồng AI nào khác hay không.

Actor:
Kỹ sư AI trực tiếp phát triển và tích hợp code; reviewer/maintainer của các module liên quan cũng bị ảnh hưởng.

Thời điểm / bối cảnh:
Sau khi merge branch của đồng nghiệp hoặc sau khi resolve conflict, trước khi tiếp tục phát triển hoặc đưa thay đổi vào nhánh dùng chung.

Current workflow 3-7 bước:
1. Pull/fetch code mới và thực hiện merge/rebase.
2. Resolve conflict nếu có.
3. Mở Git diff để xem phần code thay đổi.
4. Tự lần theo các file/module/dependency liên quan để đoán vùng bị ảnh hưởng.
5. Tự chọn và chạy build/test/lint hoặc test thủ công.
6. Nếu phát hiện lỗi thì quay lại kiểm tra commit/conflict resolution và sửa.
7. Nếu chưa thấy lỗi thì tiếp tục push/PR/merge.

Bottleneck:
Bước 4 — tự xác định phạm vi ảnh hưởng và bước 5 — quyết định cần test gì. Đây là phần cần hiểu context codebase, dependency và ý nghĩa thay đổi chứ không chỉ đọc diff.

Impact:
Ước lượng thêm 20-60 phút cho một lần merge lớn; nếu đánh giá thiếu impact có thể tạo regression, làm phát sinh thêm 30-120 phút debug hoặc ảnh hưởng đồng nghiệp ở bước sau.

Success metric:
Giảm thời gian đánh giá impact + chọn test từ baseline 20-60 phút xuống dưới 15 phút/lần; 100% merge lớn có checklist module/test cần kiểm tra; không làm tăng regression sau merge.

Non-AI alternative:
Thiết lập CODEOWNERS, dependency map, test matrix, checklist merge cố định và CI bắt buộc theo thư mục/file thay đổi.

AI hypothesis:
AI đọc diff cùng context repo để tóm tắt thay đổi, chỉ ra module/dependency có khả năng bị ảnh hưởng và đề xuất test/checklist. Kỹ sư vẫn quyết định test nào chạy và approve kết quả.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — khoảng 45-90 phút cho merge lớn (ước lượng)

[1 Pull + merge: 5']
→ [2 Resolve conflict: 15-30']
→ [3 Đọc diff: 10-15']
→ [4 Trace impact + dependency: 15-30']  <-- bottleneck
→ [5 Chọn/chạy test: 10-20']
→ [6 Sửa nếu lỗi: biến động]

FUTURE STATE — mục tiêu 20-40 phút

[1 Pull + merge: 5']
→ [2 Resolve conflict: 10-20']
→ [3 Tool lấy diff + context repo: 1-2']
→ [4 AI draft impact map + test checklist: 1-3']
→ [5 Kỹ sư review impact + chọn test: 5-10']  <-- human boundary
→ [6 CI/test chạy và kỹ sư approve]

Fallback: nếu AI phân tích sai/thiếu context, bỏ gợi ý AI và quay về đọc diff + dependency + test checklist thủ công.
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — Resolve merge conflict khi thiếu context của code người khác

```text
Problem 1 câu:
Khi Git báo conflict ở phần code do nhiều người cùng thay đổi, tôi phải tự đọc history và hỏi đồng nghiệp để hiểu ý định của từng thay đổi trước khi quyết định cách resolve.

Actor:
Kỹ sư AI đang merge/resolve conflict và kỹ sư đã viết phần code bị conflict.

Thời điểm / bối cảnh:
Khi merge/rebase branch feature có các file hoặc vùng logic bị chỉnh sửa đồng thời bởi nhiều người.

Current workflow 3-7 bước:
1. Chạy merge/rebase và nhận danh sách conflict.
2. Mở từng file conflict, xem HEAD/incoming changes.
3. Dùng `git log`, `git blame` hoặc mở PR/commit cũ để tìm context.
4. Nếu chưa hiểu, nhắn hỏi tác giả thay đổi.
5. Quyết định giữ, kết hợp hoặc viết lại đoạn code.
6. Build/test để kiểm tra resolution.
7. Commit phần resolve.

Bottleneck:
Bước 3-4 — thu thập context và hiểu “vì sao” hai phía thay đổi code; conflict marker chỉ cho biết khác nhau ở đâu, không cho biết intent.

Impact:
Ước lượng 15-45 phút/lần conflict; trường hợp phức tạp có thể lâu hơn và làm gián đoạn feature đang phát triển. Resolve sai còn có thể tạo bug logic dù Git đã hết conflict.

Success metric:
Giảm thời gian hiểu context + resolve xuống dưới 15-20 phút cho conflict thông thường; giảm số lần phải hỏi lại tác giả; không tăng lỗi do resolve sai.

Non-AI alternative:
Giảm branch sống lâu, merge/rebase thường xuyên hơn, chia ownership rõ, PR nhỏ hơn, commit message tốt hơn và tránh nhiều người sửa cùng vùng code.

AI hypothesis:
AI tổng hợp conflict hunk + commit history + surrounding code để giải thích ý định hai phía và đề xuất 1-2 phương án resolve. Kỹ sư bắt buộc review và tự chọn phương án.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — khoảng 25-60 phút/conflict phức tạp

[1 Git báo conflict: 1']
→ [2 Đọc conflict: 5-10']
→ [3 Tìm commit/history/context: 10-20']  <-- bottleneck
→ [4 Hỏi đồng nghiệp nếu cần: 5-15'+ chờ]
→ [5 Resolve + test: 10-20']

FUTURE STATE — mục tiêu 15-30 phút

[1 Git báo conflict: 1']
→ [2 Thu conflict + commit context tự động: 1-2']
→ [3 AI giải thích intent + phương án resolve: 1-3']
→ [4 Kỹ sư review/chọn/sửa resolution: 5-10']  <-- human boundary
→ [5 Build/test: 5-15']

Fallback: nếu context không đủ hoặc AI đề xuất không đáng tin, kỹ sư dùng `git log`/PR và hỏi tác giả như workflow hiện tại.
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — Review PR khó xác định vùng ảnh hưởng và test cần chạy

```text
Problem 1 câu:
Khi review PR có thay đổi ở nhiều file/module, tôi phải tự trace code để hiểu phạm vi ảnh hưởng và tự suy luận test nào cần chạy, làm review chậm và vẫn có nguy cơ bỏ sót regression.

Actor:
Kỹ sư AI/code reviewer và tác giả PR.

Thời điểm / bối cảnh:
Khi review PR trước khi merge vào nhánh dùng chung, đặc biệt với PR chạm tới core logic, API, pipeline AI hoặc shared utilities.

Current workflow 3-7 bước:
1. Đọc title/description của PR.
2. Xem danh sách file và diff.
3. Mở các hàm/class liên quan để hiểu context.
4. Trace call path/dependency sang module khác.
5. Đoán vùng ảnh hưởng và test cần chạy.
6. Comment/review hoặc checkout branch để chạy thử.
7. Approve hoặc yêu cầu sửa.

Bottleneck:
Bước 3-5 — từ diff cục bộ phải suy ra impact toàn hệ thống và chọn đúng test; đây là phần tốn nhiều context switching.

Impact:
Ước lượng 20-40 phút cho PR có nhiều module; review chậm làm PR chờ lâu, còn review thiếu impact có thể để regression đi qua.

Success metric:
Giảm thời gian “hiểu impact + lập test checklist” xuống dưới 10 phút/PR; mọi PR rủi ro cao đều có module impacted + test checklist trước approve; không tăng bug lọt qua review.

Non-AI alternative:
PR template bắt buộc author ghi impacted modules/tests; CODEOWNERS; CI path filters; dependency graph và test matrix theo thư mục.

AI hypothesis:
AI phân tích PR diff + symbol/dependency context để draft impact summary và test checklist cho reviewer. Reviewer kiểm lại trước khi dùng để quyết định approve.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — khoảng 30-50 phút/PR phức tạp

[1 Đọc PR: 3-5']
→ [2 Đọc diff: 10-15']
→ [3 Trace code/dependency: 10-20']  <-- bottleneck
→ [4 Xác định test: 5-10']
→ [5 Comment/chạy test/approve: 5-15']

FUTURE STATE — mục tiêu 15-25 phút

[1 Tool lấy PR diff + symbol context: 1-2']
→ [2 AI draft impact summary + test checklist: 1-3']
→ [3 Reviewer kiểm diff và xác nhận impact: 8-12']  <-- human boundary
→ [4 Chạy CI/test + review cuối: 5-10']

Fallback: nếu AI summary không khớp diff hoặc thiếu dependency, reviewer bỏ summary và review thủ công theo workflow cũ.
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

> Theo quy ước của worksheet, **pitch và challenge là phần bạn phải tự trình bày bằng hiểu biết của bản thân, không dùng AI để viết thay**. Vì vậy phần dưới xác định candidate mạnh nhất nhưng để bạn tự diễn đạt lời pitch/challenge.

**Card tôi muốn pitch nhất:**

```text
Problem Card #1 — Khó đánh giá tác động sau merge / resolve conflict.
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
[BẠN TỰ VIẾT 2-3 CÂU SAU KHI ĐỌC CARD #1]

Gợi ý tự nói:
- Workflow hiện tại có bước nào làm bạn mất thời gian nhất?
- Baseline nào bạn đã thực sự quan sát/đo được?
- Nếu bỏ sót impact sau merge thì hậu quả thực tế với bạn/team là gì?
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
[BẠN TỰ ĐẶT 1-2 CÂU HỎI]

Gợi ý tự soi:
- Pain này có thật sự cần AI hay dependency map + CI/test matrix đã đủ?
- Làm thế nào đo được AI giảm thời gian mà không làm tăng regression?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:
  - Baseline hiện tại chủ yếu là ước lượng, chưa có log đủ mạnh.
  - “Impact” có nguy cơ quá rộng nếu không giới hạn vào loại module/test cụ thể.
  - Một phần bài toán có thể giải bằng process/rule như PR nhỏ, CODEOWNERS, dependency map và CI.
  - AI không nên tự resolve hoặc tự approve merge vì sai ở đây có thể tạo regression khó phát hiện.
- Tôi sửa gì:
  - Thu hẹp AI vào bước **draft impact summary + test checklist** thay vì tự quyết định merge.
  - Giữ kỹ sư là human boundary: đọc diff, chọn test và approve.
  - Đặt mục tiêu đo thời gian trước/sau và theo dõi regression trong pilot.
  - Ghi rõ baseline hiện tại là ước lượng và cần xác nhận bằng dữ liệu thật.

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Đã chọn 1 card pitch + câu hỏi challenge (phần lời pitch/challenge cần tôi tự diễn đạt theo quy định của lab)
