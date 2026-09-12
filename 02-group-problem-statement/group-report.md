# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|:---:|-----------|:-----------:|---------------------------------------------------------------|
| 1   | **Lưu Quang Khải** | 2A202602599 | **Nhóm trưởng (Team Leader & Facilitator)** — Chủ trì điều phối, clear ý tưởng cho từng thành viên, đánh giá thống nhất chủ đề, đề xuất workflow hệ thống và tích hợp dữ liệu Excel |
| 2   | Mai Quang Dũng    | 2A202602966 | Co-Facilitator & AI Workflow Designer — Hỗ trợ điều phối thảo luận, cùng thiết kế sơ đồ workflow và hoàn thiện Problem Statement |
| 3   | Lê Thanh Tình     | 2A202602449 | Domain Initiator & Computer Vision Specialist — Tác giả đề xuất bài toán gốc, chuyên trách giải pháp Watershed và thị giác máy tính |
| 4   | Ngô Lê Thủy Tiên | 2A202602614 | QA Reviewer & Metric Validator — Phản biện chỉ số đo lường, rà soát edge cases, kiểm soát chất lượng báo cáo |
| 5   | Ngô Anh Khoa      | 2A202603418 | Research & Technical Benchmark Writer — Nghiên cứu đối chuẩn các công cụ hiện có (OpenCFU, ImageJ, Interscience) và viết tài liệu kỹ thuật |
| 6   | Nguyễn Khánh Linh | 2A202602409 | User Experience & Lab Interview Analyst — Phỏng vấn chuyên gia phòng lab vi sinh, phân tích khảo sát người dùng và trải nghiệm thao tác |

**Candidate problem nhóm chọn (1 câu):**
AI Workflow đếm khuẩn lạc tự động trên đĩa Petri trong phòng thí nghiệm vi sinh bằng Watershed kết hợp AI Vision, hỗ trợ giao diện Overlay chấm màu để NCV kiểm tra nhanh (click ±1) và tự động xuất kết quả Excel.

---

## Phase 3 — Group Convergence: từ 15-18 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Mai Quang Dũng | Tổng hợp thông tin kỹ thuật đa nguồn (Vin Lab, paper, đồ án) thành action items có cấu trúc | Sinh viên năm cuối, AI Engineer | Khâu liên hệ kiến thức lý thuyết mới vào đồ án thực tế và trích xuất to-do | Pain thật, rất cần thiết cho cá nhân nhưng mang tính cá nhân hóa cao, khó chuẩn hóa chung cho cả team |
| 2 | Mai Quang Dũng | Điều phối, sắp xếp lịch và ưu tiên công việc hàng ngày, cân đối deadline giữa đồ án ở trường và ở VinAI | Sinh viên, học viên | Cân nhắc mức độ ưu tiên và phân bổ thời gian khi 2 bên trùng deadline | Rất phổ biến, nhưng có thể giải quyết 60-70% bằng kỷ luật quản lý calendar và nguyên tắc Eisenhower |
| 3 | Mai Quang Dũng | Quản lý và đối chiếu lịch sử thí nghiệm ML/DL (dataset, params, metrics) rải rác giữa các máy | Nhóm làm đồ án AI | Tra cứu và tổng hợp log rải rác từ nhiều máy cá nhân về bảng so sánh | Pain point kỹ thuật chuẩn, nhưng thị trường đã có tool chuyên dụng (MLflow, WandB) nếu nhóm chịu setup |
| 4 | Ngô Lê Thủy Tiên | Rã yêu cầu khách hàng (email/biên bản họp dạng văn xuôi) thành danh sách task và subtask cụ thể trước sprint | Dev, PM, Tech Lead | Bóc tách text văn xuôi dài thành user stories, subtasks (FE/BE/DB) và acceptance criteria | Pain lớn trong Agile, nhưng khó đo lường độ chính xác tuyệt đối do phụ thuộc vào gu quản lý của từng Tech Lead |
| 5 | Ngô Lê Thủy Tiên | Reproduce bug do ticket QA/khách hàng thiếu bước tái hiện, môi trường, trình duyệt và media | Dev, QA | Vòng lặp hỏi - đáp qua lại để làm rõ context tái hiện lỗi | Tốn thời gian (~4h/tuần), nhưng rủi ro AI hallucinate cao vì đầu vào bị khuyết dữ liệu gốc nghiêm trọng |
| 6 | Ngô Lê Thủy Tiên | Dựng lại UI component từ Figma thủ công: đọc spacing, màu, font, hover state rồi gõ CSS | Frontend Developer | Gõ markup/CSS lặp đi lặp lại theo design tokens | Công việc lặp lại, nhưng scope hẹp thuần UI và hiện tại các plugin Figma AI/v0.dev đang giải quyết khá tốt |
| 7 | Ngô Anh Khoa | Đọc, giải mã công thức toán và trích xuất phương pháp từ papers khoa học cho khóa luận | Sinh viên làm khóa luận | Bước đọc sâu Methodology, giải mã ký hiệu, công thức toán và kiến trúc (55 phút/paper) | Chiếm nhiều thời gian (8-10h/tuần), nhưng liệu AI giải thích công thức toán có đủ độ sâu và độ chính xác khoa học? |
| 8 | Ngô Anh Khoa | Ghi chép, tổng hợp lecture notes và code mẫu sau mỗi buổi học thực chiến VinAI để ôn tập | Học viên VinAI | Bóc tách phần giải thích live và code mẫu trong 3 tiếng buổi học thành note có cấu trúc | Lặp lại 3 lần/tuần, nhưng nếu không có recording/transcript live thì khó tự động hóa hoàn toàn |
| 9 | Ngô Anh Khoa | Tổng hợp báo cáo tiến độ khóa luận gửi Giảng viên hướng dẫn (GVHD) vào cuối tuần | Sinh viên, GVHD | Chuyển đổi số liệu thực nghiệm và commit rời rạc thành văn bản narrative báo cáo | Cố định tối thứ Sáu, nhưng GVHD mỗi tuần có thể có yêu cầu phát sinh khác template chuẩn |
| 10 | Nguyễn Khánh Linh | Sau meeting hoặc khi có thông tin mới, team mất thời gian tổng hợp lại nội dung, phân task, xác định owner và deadline | Nhóm dự án, nhóm đồ án | Trích xuất action items từ meeting notes và gõ lại docs phân công chi tiết | Workflow họp nhóm rất rõ ràng, nhưng các nền tảng như Zoom AI hay Teams Copilot đã có tính năng recap sẵn |
| 11 | Nguyễn Khánh Linh | Tốn thời gian tìm thông tin khóa học và kiến thức đã học do rải rác trên nhiều nền tảng (Phoenix, Discord, Outlook, VLearn, GitHub) | Sinh viên, học viên | Tìm kiếm ngữ nghĩa tài liệu bài học, link nộp bài trước kỳ thi/lab | Pain point lớn mùa thi/lab; tiềm năng Semantic Search cao, nhưng vướng vấn đề phân quyền truy cập và link bị đổi |
| 12 | Nguyễn Khánh Linh | Mỗi ngày mất thời gian chọn món vừa tiện, hợp khẩu vị, ngân sách sinh viên và đủ dinh dưỡng | Sinh viên, người đi học | Ra quyết định chọn món ăn (35-50 phút/ngày, 14 lần/tuần) | Tần suất lặp lại cực cao (2 lần/ngày), bài toán recommendation hay, nhưng phụ thuộc dữ liệu quán ăn xung quanh và phí ship real-time |
| 13 | Lưu Quang Khải | Sau khi resolve conflict hoặc merge thành công, tôi không biết chắc thay đổi vừa tích hợp ảnh hưởng tới module/API/luồng nào khác | Developer, Tech Lead | Đánh giá impact và trace dependency sau khi merge code | Workflow xảy ra thường xuyên; bottleneck "đánh giá impact" rõ; tuy nhiên chưa có baseline thật về số phút và tỷ lệ regression (cần log 1-2 tuần) |
| 14 | Lưu Quang Khải | Khi conflict liên quan tới code người khác viết, tôi thiếu context để quyết định cách resolve đúng | Developer | Thiếu context code cũ để phân xử conflict đúng logic | Actor và thời điểm rõ, conflict tạo gián đoạn trực tiếp; tuy nhiên một phần có thể giải quyết bằng branch policy/quy ước nhóm tốt hơn |
| 15 | Lưu Quang Khải | Khi review PR, tôi phải tự lần theo nhiều file để biết thay đổi ảnh hưởng đâu và cần chạy test nào | Developer, Code Reviewer | Lần theo dependency graph giữa các file và chọn test suite tương ứng | Workflow review rõ, pain lặp lại; tuy nhiên chưa biết codebase có dependency graph/test mapping đủ tốt để tự động hóa bằng rule hay không |
| 16 | **Lê Thanh Tình** | **Đếm khuẩn lạc tự động trên đĩa petri trong lab vi sinh** | **Nghiên cứu viên vi sinh, Kỹ thuật viên lab** | **Thao tác thủ công bằng mắt trên hàng chục đĩa petri rất tốn thời gian (10-15'/đĩa), dễ nhầm lẫn/sót khi mật độ > 100 CFU và gõ Excel thủ công** | **Pain point cực kỳ nhức nhối, lặp lại hàng ngày; quy trình từ ảnh chụp đến kết quả Excel cực rõ ràng; giá trị thực tiễn và tính khả thi rất cao (đã có thiết kế workflow và metric chuẩn).** |
| 17 | Lê Thanh Tình | Đo diện tích lá cây (Manihot esculenta / các loài cây trồng) để đánh giá chỉ số sinh trưởng | Nhà nghiên cứu sinh lý thực vật, Kỹ sư nông nghiệp | Thao tác đo/vẽ lại bằng phần mềm thủ công (như ImageJ) tốn nhiều công sức | Cần thiết cho thí nghiệm sinh lý thực vật, nhưng là bài toán Image Segmentation hẹp, có thể giải quyết một phần bằng script ImageJ/OpenCV truyền thống |
| 18 | Lê Thanh Tình | Nhận diện & phát hiện sâu keo mùa thu (Spodoptera frugiperda) trên thực địa | Nông dân, Kỹ sư bảo vệ thực vật, Nghiên cứu viên | Phát hiện dịch hại sớm ngoài đồng ruộng trên diện tích lớn để ngăn ngừa mất mùa | Tác động kinh tế lớn, nhưng bài toán ngoài thực địa phụ thuộc nặng vào điều kiện ánh sáng tự nhiên và thiết bị biên di động (Edge AI) phức tạp |

### 3.2. Gom trùng / cluster (gom 15-18 ý thành 5 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| **A. Thị giác máy tính & Tự động hóa phòng thí nghiệm (Bio-Vision Lab)** | **#16, #17, #18** | Đếm khuẩn lạc đĩa Petri, đo diện tích lá cây, phát hiện sâu hại; điểm nghẽn là thao tác quan sát bằng mắt lặp đi lặp lại tốn thời gian, dễ mỏi mắt và nhập liệu thủ công | **Cụm có tiềm năng AI cao nhất**: quy trình khép kín, input/output rõ ràng (ảnh chụp → kết quả số liệu Excel), số đo định lượng chuẩn xác và giải quyết trực tiếp năng suất phòng lab |
| **B. Chuyển hóa văn bản thô / meeting notes thành task kỹ thuật** | #1, #4, #10 | Nhận đầu vào là văn bản dài, email, biên bản họp; điểm nghẽn là tốn công bóc tách thành các đầu việc, phân chia owner, deadline | Tiềm năng LLM tốt nhưng phụ thuộc nhiều vào yếu tố chủ quan của người quản lý, khó xây dựng ground-truth để đánh giá độ chính xác |
| **C. Nghiên cứu học thuật và tra cứu tri thức chuyên sâu** | #3, #7, #11 | Tìm kiếm, tổng hợp tài liệu học tập đa nền tảng, giải mã paper khoa học và quản lý dữ liệu thí nghiệm ML | Giá trị nhận thức cao; cần giải pháp RAG/Search nhưng có rủi ro về bản quyền và độ chính xác toán học |
| **D. Ghi chép và báo cáo định kỳ** | #8, #9 | Ghi chép bài giảng live, tổng hợp báo cáo tiến độ tuần gửi giảng viên/mentor | Quy trình lặp lại, có thể giải quyết phần lớn bằng template cố định |
| **E. Kỹ thuật phần mềm & Git workflow** | #2, #5, #6, #12, #13, #14, #15 | Quản lý deadline, tái hiện bug, dựng UI Figma, chọn món ăn, resolve conflict, review PR và trace impact sau merge | Nhiều bài toán thiên về tool chuyên dụng (Figma plugin, Git extension) hoặc quy ước branch nội bộ |

### 3.3. Shortlist (giữ các bài tiêu biểu của các thành viên để chấm điểm)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| **1. Đếm khuẩn lạc tự động trên đĩa Petri trong lab vi sinh (#16 - Tình)** | - Actor cực kỳ cụ thể: Nghiên cứu viên vi sinh, Kỹ thuật viên phòng lab nuôi cấy.<br>- Workflow 5 bước chuẩn mực từ ảnh chụp đĩa Petri đến file Excel.<br>- Bottleneck định vị chính xác: Đếm thủ công bằng mắt (10-15'/đĩa) + dễ sai khi mật độ > 100 CFU + nhập Excel thủ công.<br>- Metric định lượng rõ ràng: giảm xuống < 2 phút/đĩa, độ chính xác >= 93%. | Khuẩn lạc dính chùm hoặc bóng phản xạ trên đĩa Petri có thể gây đếm sót/trùng nếu thuật toán tách vùng (Watershed) xử lý không chuẩn. |
| **2. Rã yêu cầu khách hàng thành task sprint (#4 - Tiên)** | - Actor rõ: PM, Tech Lead, Developer.<br>- Workflow quen thuộc trong Agile/Scrum, bóc tách văn bản thô.<br>- Impact: Giảm sai lệch estimate sprint. | Thiếu ground-truth khách quan để đánh giá task sinh ra đúng hay sai; phụ thuộc nhiều vào cảm nhận cá nhân của Tech Lead. |
| **3. Tổng hợp thông tin kỹ thuật đa nguồn thành to-do (#1 - Dũng)** | - Nhu cầu cá nhân học tập và làm đồ án rất cao.<br>- Workflow 3 bước từ đọc tài liệu đến trích xuất to-do Notion.<br>- Giảm thời gian khôi phục context từ 45' xuống 15'/ngày. | Mang tính cá nhân hóa cao, thiếu tính tổng quát cho toàn bộ quy trình làm việc nhóm; phụ thuộc vào thói quen ghi chép riêng lẻ. |
| **4. Sau meeting tổng hợp nội dung, phân task, xác định owner/deadline (#10 - Linh)** | - Xảy ra liên tục hàng tuần sau mỗi buổi họp.<br>- Bottleneck trích xuất action item tốn công.<br>- Dễ đo thời gian tiết kiệm. | Rất nhiều công cụ họp trực tuyến (Zoom, Teams, Google Meet) đã tích hợp sẵn AI tóm tắt cuộc họp; khoảng trống sản phẩm độc lập bị thu hẹp. |
| **5. Đánh giá impact và trace dependency sau khi merge / resolve conflict (#13 - Khải)** | - Workflow xảy ra thường xuyên sau mỗi lần merge code.<br>- Bottleneck "đánh giá impact" định vị rất rõ. | Chưa có baseline thật về số phút và tỷ lệ regression sau merge; cần log 1-2 tuần mới có dữ liệu chuẩn. |
| **6. Đọc, giải mã công thức toán từ paper khoa học (#7 - Khoa)** | - Tốn nhiều thời gian nhất trong tuần (8-10 tiếng/tuần).<br>- Workflow rõ ràng từ tải PDF đến ghi chú Notion.<br>- Bottleneck định vị chính xác ở bước đọc hiểu Methodology (55 phút/paper). | Liệu AI giải thích công thức toán có đủ độ sâu và chính xác khoa học không, rủi ro hallucinate ký hiệu/chứng minh đại số là rất lớn. |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **Đếm khuẩn lạc tự động trên đĩa Petri (#16 - Tình)** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **Rã yêu cầu thành task sprint (#4 - Tiên)** | 5 | 5 | 4 | 4 | 4 | 4 | 5 | **31** |
| **Tổng hợp thông tin kỹ thuật đa nguồn (#1 - Dũng)** | 5 | 4 | 5 | 4 | 4 | 4 | 4 | **30** |
| **Tổng hợp meeting thành task/owner/deadline (#10 - Linh)** | 5 | 5 | 4 | 4 | 4 | 4 | 4 | **30** |
| **Đánh giá impact sau merge/conflict (#13 - Khải)** | 5 | 4 | 4 | 4 | 3 | 4 | 5 | **29** |
| **Đọc, giải mã công thức toán từ paper (#7 - Khoa)** | 4 | 4 | 5 | 4 | 3 | 4 | 4 | **28** |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
AI Workflow đếm khuẩn lạc tự động trên đĩa Petri trong phòng thí nghiệm vi sinh bằng Watershed kết hợp AI Vision, hỗ trợ giao diện Overlay chấm màu để NCV kiểm tra nhanh (click ±1) và tự động xuất kết quả Excel.
```

**Vì sao chọn (4-5 câu):**

```text
Nhóm chọn bài toán này vì đây là điểm nghẽn thực tế và nhức nhối nhất trong các phòng thí nghiệm vi sinh (như UET Microbiology Innovation).
Khâu hậu nuôi cấy hiện tại đòi hỏi nghiên cứu viên phải chấm đếm thủ công bằng mắt trên đĩa Petri, tiêu tốn từ 10 đến 15 phút cho mỗi đĩa và gây mỏi mắt nghiêm trọng.
Đặc biệt khi mật độ khuẩn lạc cao (> 100 CFU), các khuẩn dính nhau và chồng lấp rất khó phân biệt bằng mắt thường, dẫn đến việc đếm sót hoặc đếm trùng, sau đó lại phải tốn thêm thời gian gõ số liệu thủ công vào bảng tính Excel rất dễ sai số.
Bài toán có quy trình chuẩn hóa tuyến tính 5 bước cực kỳ mạch lạc từ ảnh chụp đĩa Petri đến file Excel, xác lập rõ ranh giới can thiệp AI (Watershed + AI Vision) và cơ chế chốt chặn con người (Human Review click ±1) đảm bảo an toàn tuyệt đối.
Dự án có số đo thành công (Success Metric) cụ thể, đo lường được ngay: rút ngắn thời gian từ 10-15 phút xuống dưới 2 phút/đĩa và đạt độ chính xác >= 93% so với chuyên gia đếm tay.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
- Candidate #1 (Tổng hợp thông tin kỹ thuật đa nguồn - Dũng): Dù là nỗi đau thiết thực của sinh viên và kỹ sư AI, nhưng bài toán mang tính cá nhân hóa cao, phụ thuộc sâu vào thói quen ghi chú riêng lẻ và khó chuẩn hóa thành một quy trình sản phẩm dùng chung cho cả tập thể phòng lab.
- Candidate #4 (Rã yêu cầu thành task sprint - Tiên): Dù là bài toán quản lý quen thuộc, nhưng việc đánh giá chất lượng task sinh ra phụ thuộc nhiều vào cảm tính của Tech Lead, khó xây dựng ground-truth chuẩn và khó kiểm thử tự động hóa trọn vẹn trong lab.
- Candidate #7 (Đọc, giải mã công thức toán từ paper - Khoa): Rủi ro AI hallucinate các ký hiệu toán học và biến đổi đại số phức tạp là rất cao, có thể dẫn đến việc hiểu sai hoàn toàn mô hình trong nghiên cứu khoa học, chưa kể việc kiểm chứng công thức đòi hỏi kiến thức chuyên sâu rất tốn thời gian.
- Candidate #10 (Tổng hợp meeting notes - Linh): Các nền tảng họp trực tuyến lớn (Zoom AI Companion, MS Teams Copilot, Lark) đã tích hợp sẵn tính năng tóm tắt và bóc tách action items, rào cản công nghệ thấp và khó tạo ra giá trị khác biệt.
- Candidate #13 (Đánh giá impact sau merge - Khải): Cần thời gian log dữ liệu baseline thực tế ít nhất 1-2 tuần, đồng thời phụ thuộc sâu vào compiler/AST của từng ngôn ngữ lập trình cụ thể, rủi ro kỹ thuật vượt quá khuôn khổ thời gian buổi lab.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
Ban đầu nhóm có sự phân vân và thảo luận sôi nổi giữa bài toán phần mềm (Sprint Task Breakdown của Tiên, Git Impact của Khải) và bài toán phòng thí nghiệm vi sinh (Đếm khuẩn lạc Petri của Tình).
Khải và Khoa ban đầu lo ngại bài toán vi sinh cần thiết bị chụp đắt tiền và thuật toán khó xử lý các cụm khuẩn lạc dính chùm phức tạp.
Với vai trò Nhóm trưởng, Khải đã chủ trì phiên thảo luận, làm rõ (clear) ý tưởng cho từng thành viên, rà soát ưu/nhược điểm từng bài toán dựa trên 7 tiêu chí khách quan. Khải cùng Tình và Dũng đã phân tích và đề xuất kiến trúc workflow hệ thống 5 bước: chuẩn hóa chụp ảnh bằng smartphone/webcam với giá đỡ cố định, kết hợp Watershed để tự động tách cụm khuẩn dính nhau, và điểm cốt lõi là thiết kế giao diện Overlay mask chấm màu cho phép NCV click ±1 sửa lỗi trực tiếp trong 45 giây trước khi tự động xuất Excel.
Nhận thấy giải pháp này giải quyết triệt để nỗi đau thực tế, có ranh giới can thiệp an toàn và tính khả thi vượt trội, Nhóm trưởng Khải cùng toàn bộ 6 thành viên (Khải, Dũng, Tình, Tiên, Khoa, Linh) đã nhất trí 100% chốt bài toán này làm Problem Statement chính thức của nhóm.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| **Interview** | 3 người (1 Trưởng phòng lab vi sinh, 1 Nghiên cứu viên nuôi cấy vi sinh vật, 1 Kỹ thuật viên xét nghiệm) | - Trưởng lab: *"Mỗi ngày phòng lab xử lý từ 40 đến 60 đĩa Petri. Kỹ thuật viên ngồi chấm đếm bằng mắt và bút lông đến chiều là mỏi mắt, hoa mắt, đĩa nào trên 100 CFU là bắt đầu đếm lệch nhau 10-15%."*<br>- Nghiên cứu viên: *"Ngán nhất là đĩa có khuẩn dính chùm hoặc mọc chồng lấn. Đếm xong ghi số ra giấy nháp rồi lại phải mở máy tính gõ từng ô Excel, rất dễ bị gõ nhầm dòng nọ sang dòng kia."*<br>- Kỹ thuật viên: *"Chỉ cần một công cụ chụp ảnh lại, AI chấm sẵn các đốm màu rồi cho tôi nhìn lướt qua bấm cộng trừ những chỗ AI sót là tiết kiệm được 80% thời gian."* | Một kỹ thuật viên lâu năm e ngại: *"Khuẩn lạc có lúc to lúc nhỏ, màu sắc lại khác nhau theo từng môi trường nuôi cấy (thạch máu, thạch MacConkey), liệu AI có nhận diện nhầm bọt khí hoặc vết xước trên mặt đĩa không?"* | Nhóm bổ sung thiết kế: Giao diện **Overlay mask chấm màu** và tính năng **Click ±1**, cho phép NCV trực tiếp thêm/bớt điểm đếm bằng một cú click chuột ngay trên màn hình trước khi xác nhận. |
| **Survey / poll** | 10 sinh viên và học viên cao học làm thí nghiệm vi sinh & CNSH | - 10/10 người (100%) khẳng định việc đếm khuẩn lạc thủ công là khâu nhàm chán và tốn thời gian nhất sau giai đoạn nuôi cấy.<br>- Thời gian trung bình: 10 - 15 phút cho mỗi đĩa Petri.<br>- Đánh giá mức độ cấp thiết cần công cụ tự động hóa: 4.8 / 5. | 2 người cho rằng nếu đĩa có mật độ quá thưa (< 30 CFU) thì đếm tay nhanh hơn mở máy chụp ảnh. | Làm rõ Boundary: Hệ thống phát huy giá trị tối đa ở dải mật độ thông thường từ 30 đến 300 CFU (dải tiêu chuẩn trong vi sinh học). |
| **Log / dữ liệu thực nghiệm** | Kiểm tra đối chiếu trên 30 đĩa Petri thực tế | Tỷ lệ đếm lệch giữa 2 kỹ thuật viên đếm độc lập khi mật độ > 100 CFU dao động từ 8% đến 16%. Thời gian gõ số liệu vào file Excel trung bình mất thêm 2-3 phút/mẫu. | Khi mật độ > 300 CFU (dày đặc như thảm), cả mắt người và AI đều không thể đếm chính xác từng khuẩn lạc riêng lẻ. | Nhóm bổ sung cảnh báo: Với đĩa mật độ quá dày (TNTC - Too Numerous To Count), hệ thống tự động gợi ý pha loãng mẫu ở nồng độ cao hơn thay vì cố đếm. |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Pain thật không chỉ nằm ở việc đếm số lượng, mà nằm ở gánh nặng thị giác và mệt mỏi nhận thức khi phải phân biệt các khuẩn lạc dính chùm trên đĩa mật độ cao (> 100 CFU), cộng thêm sự phiền toái, dễ nhầm lẫn khi phải nhập liệu thủ công từng con số vào bảng tính Excel.
```

Bằng chứng đính kèm (nếu có): `02-group-problem-statement-interview-notes.md`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **OpenCFU** | [OpenCFU SourceForge](https://opencfu.sourceforge.net/) | Tự động phát hiện và đếm khuẩn lạc từ ảnh đĩa Petri bằng thuật toán Computer Vision cổ điển | Mã nguồn mở, xử lý nhanh, không cần GPU, phân tích được kích thước khuẩn lạc | Thuần xử lý ảnh hình thái học cổ điển (Hough Transform, Thresholding); rất kém khi khuẩn lạc dính chùm; UI desktop lỗi thời; cài đặt phức tạp | Phải kết hợp Watershed Segmentation và AI Vision để tách cụm khuẩn dính nhau; cần Web UI trực quan dễ dùng |
| **ImageJ / Colony Counter Plugin** | [ImageJ Colony Counter](https://imagej.net/plugins/colony-counter) | Phân đoạn ảnh và đếm hạt trên ảnh nhị phân (Binary Mask) | Đo đạc diện tích chính xác, công cụ nghiên cứu chuẩn mực trong phòng lab | Đòi hỏi người dùng phải tự căn chỉnh hàng loạt tham số thủ công (threshold, circularity, size limit) cho từng ảnh; không tự động xuất báo cáo Excel theo mẫu | Phải tự động hóa toàn bộ khâu tiền xử lý ảnh; cung cấp 1-click export trực tiếp ra file Excel |
| **Interscience Scan 1200 / Chuyên dụng** | [Interscience Scan Systems](https://www.interscience.com/en/products/automatic-colony-counters/scan-1200/) | Máy đếm khuẩn lạc phần cứng khép kín chuyên nghiệp | Độ chính xác cực cao, buồng tối chuẩn hóa ánh sáng LED 360 độ | Giá thành cực kỳ đắt đỏ ($5,000 - $15,000), thiết bị cồng kềnh, hệ thống đóng kín, các phòng lab vừa và nhỏ hoặc sinh viên không thể tiếp cận | Xây dựng giải pháp AI Workflow phần mềm linh hoạt, tận dụng camera smartphone thông thường kết hợp giá đỡ chụp ảnh chuẩn hóa với chi phí thấp |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
Nhóm KHÔNG NÊN cố gắng chế tạo thiết bị phần cứng đắt tiền hay xây dựng phần mềm desktop nặng nề đòi hỏi căn chỉnh hàng tá tham số như ImageJ.
Nhóm NÊN build một AI Workflow tinh gọn trên nền Web: Nhận ảnh chụp đĩa Petri chuẩn hóa, sử dụng pipeline Watershed + AI Vision để tự động tách vùng và đếm khuẩn lạc, hiển thị Overlay mask chấm màu để NCV kiểm tra nhanh (click ±1), và tự động xuất thẳng kết quả vào Excel chỉ với một cú click chuột.
```

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

```text
HẬU NUÔI CẤY: Chấm đếm khuẩn lạc thủ công tốn thời gian, dễ mỏi mắt và dễ sai khi mật độ cao.

[1 Lấy đĩa Petri sau ủ: 1' - NCV] 
→ [2 Đặt đĩa lên bàn soi ánh sáng: 1' - NCV] 
→ [3 Chấm đếm thủ công bằng mắt & bút lông: 10-15'] <-- BOTTLENECK CHÍNH (> 100 CFU dễ sót/trùng)
→ [4 Ghi tạm số lượng ra giấy nháp: 1' - NCV] 
→ [5 Mở máy tính nhập thủ công vào Excel: 2-3' - NCV] <-- BOTTLENECK PHỤ (dễ sai số)
→ [6 Đối chiếu lại số liệu: 1' - NCV]

Tổng thời gian: 15 - 20 phút / đĩa Petri
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1. Lấy đĩa sau nuôi cấy | Nghiên cứu viên (NCV) | Tủ ủ vi sinh vật (37°C) | Đĩa Petri đã mọc khuẩn lạc | 1 phút / đĩa | Thao tác vật lý chuẩn bị |
| 2. Đặt đĩa lên bàn soi | NCV / Kỹ thuật viên | Đĩa Petri | Đĩa đặt cố định dưới đèn rọi | 1 phút / đĩa | Chuẩn bị góc nhìn và ánh sáng |
| 3. Chấm đếm bằng mắt | NCV / Kỹ thuật viên | Đĩa Petri trên bàn soi | Các vết chấm mực trên đáy đĩa | **10 - 15 phút / đĩa** | **BOTTLENECK CHÍNH**: Thao tác lặp lại bằng mắt, cực kỳ mỏi mắt; khi mật độ > 100 CFU các khuẩn dính chùm, chồng lấp dẫn đến đếm sót hoặc đếm trùng |
| 4. Ghi chép tạm thời | NCV | Số đếm nhẩm trong đầu | Con số ghi trên giấy nháp / sổ tay lab | 1 phút / đĩa | Handoff từ thao tác đếm sang ghi chép |
| 5. Nhập liệu vào Excel | NCV / Kỹ thuật viên | Sổ tay ghi chép | Bảng tính Excel lưu trữ thí nghiệm | **2 - 3 phút / đĩa** | **BOTTLENECK PHỤ**: Nhập liệu thủ công từng đĩa, dễ nhầm lẫn số liệu, sai lệch dòng cột |
| 6. Đối chiếu số liệu | NCV | Đĩa Petri và file Excel | Kết quả hoàn tất | 1 phút / đĩa | Kiểm tra xác suất |

**Bottleneck chính (2-3 câu):**

```text
Điểm nghẽn cốt lõi nằm ở sự kết hợp giữa "Thao tác lặp lại bằng mắt (10-15 phút/đĩa)" và "Nhập liệu Excel thủ công".
Khi đĩa có mật độ cao (> 100 CFU), việc các khuẩn lạc dính nhau khiến NCV bị hoa mắt, dẫn đến sai số đếm sót hoặc đếm trùng từ 10-15%.
Công đoạn gõ lại số liệu từ sổ tay vào Excel vừa tốn thêm thời gian, vừa là nguồn cơn phát sinh lỗi sai lệch dữ liệu thí nghiệm.
```

### 5.2. Future workflow bản nhóm

```text
XỬ LÝ BOTTLENECK NHƯ THẾ NÀO? — Quy trình từ ảnh đĩa Petri đến kết quả Excel

[1 Chụp ảnh đĩa Petri: 30s - NCV] (Chuẩn hóa đầu vào: ánh sáng, góc chụp, nền)
→ [2 Watershed + AI Vision: 10s - AI Intervention Point] (Tự tách vùng, phát hiện và đếm khuẩn lạc)
→ [3 Overlay mask chấm màu: 5s - AI/Hệ thống] (NCV kiểm tra nhanh các điểm AI đã đánh dấu)
→ [4 Click ±1 nếu cần: 45s - Human Review / Boundary] (Sửa lỗi đếm sót / đếm trùng)
→ [5 Export kết quả vào Excel: 5s - Máy/Rule] (Loại bỏ nhập liệu tay: xuất số lượng CFU và metadata)

Tổng thời gian: < 2 phút / đĩa Petri (Tối ưu từ 10-15 phút → < 2 phút)
```

| Bước | Actor | Thao tác / Công nghệ | Thời gian | Vai trò |
|---|---|---|---|---|
| **1. Chụp ảnh đĩa Petri** | NCV | Chụp ảnh với giá đỡ chuẩn hóa: ánh sáng đều, góc vuông góc, nền tương phản để đảm bảo chất lượng ảnh | 30 giây | Chuẩn hóa đầu vào (Human) |
| **2. Watershed + AI Vision** | Hệ thống / AI | Thuật toán Watershed phân đoạn tách các cụm dính chùm kết hợp mô hình AI Vision phát hiện và đếm tọa độ khuẩn lạc | 10 giây | **AI Intervention Point** |
| **3. Overlay mask chấm màu** | Hệ thống | Vẽ các đốm màu (overlay mask) lên ảnh đĩa Petri để NCV quan sát trực quan các vị trí AI đã nhận diện | 5 giây | Trực quan hóa kết quả (System) |
| **4. Click ±1 nếu cần** | NCV | NCV nhìn lướt qua màn hình, click chuột để thêm (+1) các điểm AI bỏ sót hoặc bớt (-1) các điểm AI nhận nhầm bọt khí | 45 giây | **Human Review & Boundary** |
| **5. Export kết quả vào Excel** | Hệ thống / Rule | Tự động xuất số lượng khuẩn lạc (CFU), mã mẫu, ngày giờ và độ pha loãng vào bảng tính Excel theo template chuẩn | 5 giây | Loại bỏ nhập liệu tay (Rule/Machine) |

```text
Fallback: Nếu ảnh chụp quá mờ, rung lắc hoặc đĩa thạch bị nứt vỡ khiến AI không nhận diện được, hệ thống hiển thị cảnh báo "Ảnh không đạt chuẩn, vui lòng chụp lại" hoặc cho phép NCV chuyển sang đếm thủ công trên bàn soi truyền thống.
```

**Before/after impact:**

| Metric | Trước (Hiện tại) | Sau kỳ vọng (AI Workflow) | Cách đo lường |
|---|---:|---:|---|
| **Thời gian xử lý / đĩa** | 10 - 15 phút / đĩa | **< 2 phút / đĩa** | Bấm giờ từ lúc đặt đĩa lên chụp ảnh đến khi xuất file Excel hoàn tất (tiết kiệm hơn 80% thời gian) |
| **Độ chính xác số đếm** | Dao động lớn, sai số 10-15% khi > 100 CFU | **≥ 93%** so với đếm tay chuyên gia | Đối chiếu số đếm AI sau human review với kết quả đếm độc lập của 2 chuyên gia vi sinh kỳ cựu |
| **Thao tác nhập liệu Excel** | Gõ tay thủ công 2-3 phút, dễ nhầm dòng | **Tự động 100%** (0 phút gõ tay) | Số lượng lỗi sai số khi chuyển dữ liệu từ đĩa sang Excel bằng 0 |
| **Trải nghiệm nghiên cứu viên** | Mỏi mắt, căng thẳng, hiệu suất thấp | Nhanh hơn, chính xác hơn, hiệu quả hơn | Đánh giá mức độ hài lòng của NCV qua khảo sát trải nghiệm (thang điểm 1-5) |
| **Risk mới** | Không có risk AI | AI có thể bỏ sót khuẩn dính chùm hoặc đếm nhầm bọt khí/vết bẩn | **Kiểm soát chặt chẽ**: NCV xem overlay mask chấm màu và chỉnh ±1 trước khi xác nhận |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | Nghiên cứu viên vi sinh, Kỹ thuật viên phòng thí nghiệm nuôi cấy vi sinh vật tại các trường đại học, viện nghiên cứu và doanh nghiệp (như UET Microbiology Innovation). |
| **Workflow** | Nuôi cấy vi sinh → Đặt đĩa Petri lên bàn soi → Chấm đếm thủ công bằng mắt và bút lông → Ghi số ra giấy nháp → Mở máy tính gõ thủ công vào bảng Excel. |
| **Bottleneck** | Thao tác chấm đếm thủ công bằng mắt tốn từ 10-15 phút/đĩa, gây mỏi mắt nghiêm trọng; khi mật độ khuẩn lạc > 100 CFU thì các khuẩn dính nhau, chồng lấp dẫn đến đếm sót hoặc đếm trùng; khâu nhập Excel thủ công dễ sai lệch số liệu. |
| **Impact** | Mỗi ngày tiêu tốn từ 3 đến 5 tiếng của nhân sự phòng lab cho việc đếm và nhập liệu 20-30 đĩa Petri; làm giảm năng suất thí nghiệm và tiềm ẩn rủi ro sai lệch dữ liệu nghiên cứu khoa học. |
| **Success Metric** | Giảm thời gian xử lý từ 10-15 phút xuống dưới 2 phút/đĩa; độ chính xác đạt ≥ 93% so với đếm tay chuyên gia; loại bỏ 100% việc nhập liệu tay vào Excel. |
| **Boundary** | AI chỉ hỗ trợ tách vùng, định vị và đếm số lượng khuẩn lạc (CFU) trên ảnh chụp đĩa Petri; AI KHÔNG tự động lưu kết quả nếu chưa qua NCV review overlay; AI KHÔNG phân loại hay định danh loài vi khuẩn. |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ: Điều kiện chụp ảnh đầu vào chưa được chuẩn hóa (ánh sáng, khoảng cách, camera); chưa làm rõ dải mật độ CFU tối đa mà hệ thống có thể xử lý tin cậy.
- Tôi sửa gì: Bổ sung yêu cầu chuẩn hóa đầu vào ở Bước 1 (dùng giá đỡ cố định, nền đen/trắng tương phản, đèn LED tản sáng) và giới hạn dải đo tối ưu từ 30 đến 300 CFU theo chuẩn vi sinh học quốc tế.

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [x] Thấp/Trung bình — Vì sao: Bài toán đếm số lượng đối tượng hữu hình (khuẩn lạc hình tròn/bầu dục) có chân lý đúng/sai rõ ràng. Độ mơ hồ chỉ phát sinh ở các ca khó: khuẩn lạc dính chùm, mép viền mờ hoặc bọt khí/vết xước trên đĩa thạch.
- Độ phức tạp: [x] Cao — Vì sao: Quy trình gồm chuỗi 5 bước tuần tự kết hợp đa công nghệ: Chuẩn hóa ảnh → Thuật toán hình thái học Watershed → Mô hình AI Vision phát hiện vật thể → Vẽ Overlay mask tương tác → Export file Excel theo format chuẩn.

**Bài toán nhóm nằm ở ô nào:**

```text
Ô: Medium Ambiguity — High Complexity (Độ mơ hồ vừa phải — Độ phức tạp cao).
```

**Vì sao (2-3 câu):**

```text
Đầu vào là hình ảnh đĩa Petri có nhiều biến thiên thực tế (kích thước khuẩn lạc to nhỏ khác nhau, khuẩn dính cụm, bọt khí, bóng phản xạ ánh sáng).
Quy trình xử lý đòi hỏi sự kết hợp chặt chẽ giữa thuật toán thị giác máy tính chuyên sâu (Watershed) với mô hình AI Vision, đồng thời có giao diện tương tác con người (Human Review click ±1) trước khi xuất file Excel.
```

### 6.1. So sánh Rule / Workflow / Agent (sao y lập luận chuẩn từ infographic)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | Thuật toán xử lý ảnh cổ điển (Otsu Thresholding, Hough Circle Transform, Contours detection) | Khi đĩa thạch cực kỳ sạch, mật độ rất thưa (< 30 CFU), các khuẩn lạc tròn đều hoàn hảo và không có khuẩn nào dính chùm | **Không đủ linh hoạt**: Thất bại hoàn toàn khi khuẩn lạc dính chùm chồng lấn, biến thiên hình thái, hoặc đĩa có vết bẩn/bọt khí | **Không phù hợp làm lõi**: Chỉ dùng Rule ở bước 5 để format và ghi dữ liệu ra file Excel |
| **Workflow** | **Pipeline 5 bước tuần tự**: Ảnh chuẩn hóa → Watershed + AI Vision → Overlay mask chấm màu → NCV Human Review (click ±1) → Auto-export Excel | **Phù hợp nhất**: Quy trình rõ ràng, AI xử lý bước nặng nhận diện/đếm, con người kiểm tra trước khi xuất file | Cần đảm bảo ảnh đầu vào đủ độ nét và NCV không lơ là bỏ qua bước review overlay | **CHỌN (Phù hợp nhất)**: Cốt lõi của toàn bộ giải pháp |
| **Agent** | AI Agent tự động điều khiển cánh tay robot lấy đĩa Petri, tự quyết định chỉnh tiêu cự camera, tự phân tích và tự gửi email kết quả | Khi phòng thí nghiệm tự động hóa hoàn toàn ở quy mô công nghiệp (Fully Automated Bio-Robotics) | **Chưa cần**: Hệ thống không phải tự lập kế hoạch hay tự quyết định phân nhánh nhiều bước; chi phí chế tạo quá đắt và rủi ro mất kiểm soát | **Chưa cần**: Vượt quá nhu cầu thực tế và phạm vi của lab |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. **Rule có giải được 70-80% case không?**  
   Không, vì các đĩa nuôi cấy vi sinh thực tế luôn có sự biến thiên hình thái khuẩn lạc và tỷ lệ khuẩn dính chùm cao khi mật độ > 100 CFU; Rule cổ điển chỉ giải quyết được khoảng 30-40% đĩa lý tưởng.
2. **Các bước có đi thẳng một đường không hay phải rẽ nhánh?**  
   Quy trình đi thẳng một đường tuyến tính rõ ràng: Chụp ảnh → Watershed/AI Vision đếm → Overlay chấm màu → NCV click ±1 → Xuất Excel.
3. **Có thật sự cần Agent tự lập kế hoạch + gọi tool không?**  
   Chưa cần, vì quy trình không đòi hỏi AI phải tự do khám phá hay tự lên kế hoạch động; một pipeline Workflow được lập trình sẵn là hoàn toàn tối ưu.
4. **Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?**  
   Nghiên cứu viên phát hiện ngay lập tức nhờ giao diện Overlay mask chấm màu trực quan và có thể dùng chuột click ±1 để thêm/bớt điểm đếm trong vòng 30-45 giây.
5. **Có hạ được từ Agent → Workflow → Rule không?**  
   Có, nhóm kiên định chọn giải pháp **Workflow**, kết hợp Rule định dạng dữ liệu ở bước cuối, không lãng phí tài nguyên làm Agent.

**Mức chọn:**

```text
Workflow
```

**Vì sao chọn (3-4 câu):**

```text
Nhóm chọn mức Workflow vì đây là phương án PHÙ HỢP NHẤT: quy trình 5 bước cực kỳ rõ ràng, phân định minh bạch trách nhiệm giữa máy và người.
AI đảm nhận phần việc nặng nhọc nhất là nhận diện và phân đoạn các cụm khuẩn dính nhau (Watershed + AI Vision), trong khi con người giữ vai trò chốt chặn kiểm tra (Human Review) trước khi xuất kết quả.
Cách tiếp cận này loại bỏ sự phức tạp không cần thiết của Agent, đồng thời khắc phục triệt để sự cứng nhắc, thiếu linh hoạt của Rule.
```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text
Mức Rule đơn giản (xử lý ảnh cổ điển) hoàn toàn không đủ linh hoạt để thích ứng với sự biến thiên đa dạng về hình thái, kích thước và màu sắc của khuẩn lạc trong môi trường vi sinh thực tế.
Nếu chỉ dùng Rule, tỷ lệ đếm sót và đếm sai khi khuẩn dính chùm là rất lớn, NCV vẫn phải mất rất nhiều công sức để sửa lại bằng tay, không đạt được mục tiêu tiết kiệm thời gian.
```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Nghiên cứu viên vi sinh, Kỹ thuật viên phòng thí nghiệm nuôi cấy vi sinh vật tại các trường đại học, viện nghiên cứu và phòng xét nghiệm (như UET Microbiology Innovation). |
| **Workflow** | Chụp ảnh đĩa Petri chuẩn hóa (30s) → Watershed + AI Vision tự tách vùng, phát hiện và đếm (10s) → Hiển thị Overlay mask chấm màu (5s) → NCV kiểm tra nhanh và click ±1 nếu cần (45s) → Tự động xuất kết quả vào Excel (5s). |
| **Bottleneck** | Thao tác chấm đếm thủ công bằng mắt tốn 10-15 phút/đĩa, gây mỏi mắt; khuẩn lạc dính chùm khi mật độ > 100 CFU dẫn đến đếm sót/trùng; thao tác nhập Excel thủ công dễ sai số. |
| **Impact** | Tiêu tốn 3-5 tiếng mỗi ngày của nhân sự phòng lab cho 20-30 đĩa; hiệu suất thấp và tiềm ẩn nguy cơ sai lệch số liệu trong các công bố khoa học hoặc thử nghiệm dược/thực phẩm. |
| **Success Metric** | - Thời gian xử lý: Rút ngắn từ 10-15 phút/đĩa xuống **< 2 phút/đĩa**.<br>- Độ chính xác: Đạt **≥ 93%** so với đếm tay chuyên gia.<br>- Nhập liệu: Loại bỏ 100% thao tác gõ Excel thủ công. |
| **Boundary** (làm / không làm) | **LÀM**: Tách cụm khuẩn lạc dính chùm, đếm số lượng CFU, vẽ overlay chấm màu, cho phép click ±1 tương tác, xuất file Excel chuẩn.<br>**KHÔNG LÀM**: Không tự động phê duyệt nếu thiếu xác nhận của NCV; không phân loại định danh chủng vi khuẩn; không xử lý đĩa mật độ quá dày (TNTC > 300 CFU). |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | Can thiệp **ngay sau Bước 1** (sau khi NCV chụp và tải ảnh đĩa Petri lên hệ thống) và kết thúc **trước Bước 4** (trước khi NCV tiến hành kiểm tra trên giao diện Overlay mask). |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | **Workflow**: Quy trình 5 bước tuyến tính rõ ràng, AI giải quyết bước nhận diện/đếm khó nhất và con người kiểm tra trước khi xuất file. |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | **Rủi ro lớn nhất**: AI có thể bỏ sót khuẩn lạc dính chùm hoặc đếm nhầm bọt khí/vết xước, đặc biệt khi mật độ cao hoặc khuẩn lạc không điển hình.<br>**Người thật kiểm soát**: NCV trực tiếp xem Overlay mask chấm màu và click chuột ±1 để sửa lỗi đếm sót / đếm trùng trước khi bấm nút Export Excel. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | **Yes** | Actor là NCV/Kỹ thuật viên phòng lab vi sinh; workflow 5 bước từ ảnh chụp đến kết quả Excel cực kỳ rõ nét. |
| Baseline + metric đo được chưa? | **Yes** | Baseline là 10-15 phút/đĩa và sai số 10-15% khi > 100 CFU; mục tiêu sau AI là < 2 phút/đĩa và độ chính xác ≥ 93%. |
| Data/input đủ dùng chưa? | **Yes** | Dữ liệu đầu vào là ảnh chụp đĩa Petri bằng camera thông thường hoàn toàn sẵn có trong phòng lab vi sinh. |
| AI sai, hậu quả chấp nhận được không? | **Yes** | Nếu AI đếm nhầm hoặc sót, NCV nhìn thấy ngay trên overlay mask và chỉ mất 1 cú click chuột để sửa ±1, không gây sai lệch dữ liệu cuối. |
| Có người review/owner không? | **Yes** | NCV là người trực tiếp kiểm tra và bấm nút xác nhận cuối cùng trước khi xuất file Excel. |
| Có cách non-AI đơn giản hơn không? | **Yes** (đã xem xét và loại trừ) | Các rule xử lý ảnh cổ điển (OpenCFU, ImageJ) đã được kiểm nghiệm và thất bại khi khuẩn lạc dính chùm hoặc đĩa có biến thiên hình thái. |

**Decision:**

```text
Go
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Quyết định GO được đưa ra dựa trên bằng chứng thực tế từ 100% kỹ thuật viên và nghiên cứu viên vi sinh đều khẳng định chấm đếm thủ công là khâu nhàm chán, mỏi mắt và tốn thời gian nhất sau nuôi cấy.
Bản thiết kế AI Workflow đã định hình hoàn chỉnh từ khâu chuẩn hóa đầu vào, thuật toán tách vùng Watershed kết hợp AI Vision, đến cơ chế tương tác click ±1 và xuất Excel tự động.
Giải pháp có tính khả thi kỹ thuật rất cao, mang lại giá trị định lượng vượt trội (tiết kiệm hơn 80% thời gian, đạt độ chính xác ≥ 93%) và hoàn toàn có thể triển khai thử nghiệm ngay trong phòng lab.
```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text
- Data thử nghiệm: 30 ảnh đĩa Petri thực tế từ phòng lab vi sinh với dải mật độ từ 30 đến 250 CFU (bao gồm cả đĩa khuẩn lạc rời và khuẩn dính chùm).
- Cách chạy thử: Đưa ảnh qua pipeline Watershed + AI Vision trên giao diện web mẫu, hiển thị overlay chấm màu để NCV kiểm tra và dùng chuột click ±1.
- Đo 3 số cụ thể:
  1. Thời gian NCV hoàn thành 1 đĩa từ lúc tải ảnh đến khi xuất Excel (Mục tiêu: < 2 phút/đĩa).
  2. Độ chính xác số đếm sau khi NCV xác nhận so với ground-truth đếm tay chuyên gia (Mục tiêu: ≥ 93%).
  3. Tỷ lệ số điểm NCV phải can thiệp sửa ±1 (Mục tiêu: < 7% tổng số khuẩn lạc trên đĩa).
```

**Nếu Not Yet — cần validate gì trước:**

```text
(Không áp dụng vì nhóm đã chọn GO)
```

**Nếu No-Go — làm gì thay AI:**

```text
(Không áp dụng vì nhóm đã chọn GO)
```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text
Nhóm sẽ dừng áp dụng hệ thống AI Workflow và quay về quy trình đếm thủ công truyền thống nếu qua 30 đĩa thử nghiệm pilot xảy ra 1 trong các điều kiện sau:
1. Độ chính xác của AI trước khi con người can thiệp đạt dưới 80%, khiến NCV phải bấm sửa chuột quá nhiều (> 20 lần/đĩa).
2. Tổng thời gian thao tác (chụp ảnh + chờ AI xử lý + sửa lỗi click ±1) vượt quá thời gian đếm tay thủ công (> 10 phút/đĩa).
3. Thuật toán Watershed liên tục nhận nhầm bọt khí hoặc vết xước trên đĩa thạch thành khuẩn lạc trên 3 đĩa liên tiếp.
```

---

## Phase 7 (Group Appendix) — Đánh giá đóng góp thành viên (Peer Review)

### 7.1. Bảng tổng hợp mức độ đóng góp và xếp loại thành viên

Nhóm đã tiến hành họp đánh giá chéo công khai, minh bạch dựa trên chất lượng đầu ra, mức độ chủ động và tinh thần phối hợp trong suốt các giai đoạn từ Phase 3 đến Phase 6. Toàn bộ 6 thành viên đều tham gia đầy đủ, tích cực và hoàn thành xuất sắc vai trò được phân công.

| STT | Họ và tên | Mã học viên | Vai trò chính | Nhiệm vụ cụ thể đã hoàn thành | Mức độ đóng góp | Đánh giá chung |
|:---:|---|:---:|---|---|:---:|:---:|
| 1 | **Lưu Quang Khải** | 2A202602599 | **Nhóm trưởng (Team Leader & System Workflow Lead)** | - Chủ trì điều phối toàn bộ các phiên họp, làm rõ (clear) ý tưởng và định hướng phản biện cho từng thành viên.<br>- Đánh giá, phản biện khách quan các candidates và dẫn dắt nhóm thống nhất chủ đề chung.<br>- Trực tiếp đề xuất và hoàn thiện kiến trúc workflow hệ thống (5 bước tuyến tính, ranh giới Human Review click ±1, cơ chế tự động xuất Excel).<br>- Chịu trách nhiệm tổng hợp, rà soát và hoàn thiện toàn bộ báo cáo nhóm. | 100% | **Tốt / Xuất sắc** |
| 2 | **Mai Quang Dũng** | 2A202602966 | Co-Facilitator & AI Workflow Designer | - Hỗ trợ điều phối các phiên thảo luận nhóm, quản lý tiến độ và thời gian.<br>- Cùng Nhóm trưởng cấu trúc chi tiết sơ đồ Current State (6 bước, 15-20') và Future State (5 bước, < 2').<br>- Soạn thảo và hoàn thiện Problem Statement v0/v1, tham gia lập luận lựa chọn Workflow thay vì Agent. | 100% | **Tốt / Xuất sắc** |
| 3 | **Lê Thanh Tình** | 2A202602449 | Domain Initiator & Vision Specialist | - Tác giả ý tưởng gốc (Candidate #16) đạt điểm cao nhất nhóm (35/35).<br>- Cung cấp infographic thiết kế giải pháp hoàn chỉnh (UET Microbiology Innovation).<br>- Đóng góp chuyên môn vi sinh, kiến thức về thuật toán Watershed và cơ chế click ±1 trên Overlay mask. | 100% | **Tốt / Xuất sắc** |
| 4 | **Ngô Lê Thủy Tiên** | 2A202602614 | QA Reviewer & Metric Validator | - Phản biện và chuẩn hóa hệ thống Success Metric (< 2 phút/đĩa, độ chính xác ≥ 93%).<br>- Rà soát các trường hợp ngoại lệ (khuẩn dính chùm, bọt khí, đĩa thạch quá dày TNTC).<br>- Đảm bảo tính chặt chẽ của các tiêu chí rollback và kế hoạch pilot. | 100% | **Tốt / Xuất sắc** |
| 5 | **Ngô Anh Khoa** | 2A202603418 | Research & Benchmark Writer | - Nghiên cứu đối chuẩn các giải pháp hiện hành (OpenCFU, ImageJ, Interscience Scan).<br>- Tổng hợp link tài liệu tham khảo và phân tích rõ khoảng trống thị trường.<br>- Soạn thảo các luận điểm vì sao chọn Workflow và loại bỏ Rule/Agent. | 100% | **Tốt / Xuất sắc** |
| 6 | **Nguyễn Khánh Linh** | 2A202602409 | User Experience & Lab Interview Analyst | - Thực hiện phỏng vấn nhanh nghiên cứu viên và kỹ thuật viên lab vi sinh.<br>- Phân tích dữ liệu khảo sát người dùng, thu thập các quote nguyên văn đắt giá.<br>- Đề xuất tối ưu trải nghiệm người dùng tại bước Overlay mask chấm màu. | 100% | **Tốt / Xuất sắc** |

### 7.2. Nhận xét tinh thần và thái độ làm việc nhóm

```text
- Tinh thần hợp tác: Cả 6 thành viên thể hiện tinh thần trách nhiệm rất cao, tham gia 100% các buổi họp nhóm trực tiếp và online, không có hiện tượng ỷ lại hay trễ hạn công việc.
- Chất lượng phản biện: Các buổi thảo luận diễn ra sôi nổi, thẳng thắn và mang tính xây dựng cao. Nhóm đã chuyển hướng kịp thời và dứt khoát sang bài toán Đếm khuẩn lạc đĩa Petri khi nhận thấy giải pháp có tính khả thi, định lượng đo lường và giá trị thực tế vượt trội.
- Tinh thần đồng thuận: Cả 6 thành viên đều hài lòng và nhất trí tuyệt đối với Problem Statement cuối cùng, sẵn sàng bước vào giai đoạn hiện thực hóa giải pháp ở các buổi học tiếp theo.
```

---

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 15-18 → 1 (cluster + shortlist + score)
- [x] Có validation (quote thật) + research (link kiểm được)
- [x] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [x] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [x] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do
- [x] Có bảng đánh giá đóng góp công bằng, chi tiết cho toàn bộ thành viên nhóm
