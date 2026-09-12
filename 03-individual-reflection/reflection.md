# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Lưu Quang Khải
- Mã học viên: 2A202602599
- Nhóm: Nhóm EQ200 (6 thành viên)
- Candidate problem nhóm chọn: AI Workflow đếm khuẩn lạc tự động trên đĩa Petri trong phòng thí nghiệm vi sinh bằng Watershed kết hợp AI Vision, hỗ trợ giao diện Overlay chấm màu để NCV kiểm tra nhanh (click ±1) và tự động xuất kết quả Excel.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Tự scan 10 problem từ công việc Kỹ sư AI hằng ngày (Git merge, PR review, dependency impact, context switching); dùng AI bổ sung góc nhìn và số đo cụ thể. | Đưa ra 3 candidate chất lượng cao đại diện cho nhóm Software/Git workflow, giúp nhóm có dữ liệu phong phú ở Phase 3. |
| Pitch Problem Card | Pitch Problem Card #1 ("Khó đánh giá tác động sau merge / resolve conflict") trong 2 phút, nêu bật bottleneck đọc diff 20-60' và nguy cơ regression. | Bài được nhóm đánh giá cao về tính logic và đưa vào Shortlist (Top 5) để chấm điểm đồng thuận. |
| Challenge bài của bạn khác | Đặt câu hỏi phản biện bài #16 của Tình (vi sinh) về rủi ro cụm khuẩn dính chùm và thiết bị chụp; phản biện bài #1 và #4 về rủi ro thiếu ground-truth khách quan. | Thúc đẩy Tình và nhóm đưa ra giải pháp dùng thuật toán Watershed xử lý cụm khuẩn và chuẩn hóa góc chụp bằng smartphone/webcam giá rẻ. |
| Gom trùng / cluster | Phân tích và gom 18 candidate của 6 thành viên thành 5 cụm (A đến E), tách riêng cụm Bio-Vision Lab với các cụm Software, Meeting và Document. | Giúp cả nhóm nhìn thấy bức tranh toàn cảnh, không bị rối trước 18 ý tưởng và định vị cụm Bio-Vision là cụm có tiềm năng AI cao nhất. |
| Chọn candidate problem | Với vai trò Nhóm trưởng, chủ trì phiên chấm điểm theo 7 tiêu chí; lắng nghe và clear ý tưởng cho từng thành viên; điều phối thống nhất chủ đề. | Dẫn dắt nhóm thống nhất 100% chọn bài toán đếm khuẩn lạc đĩa Petri (#16) vì tính khả thi và impact vượt trội (đạt 35/35 điểm). |
| Validation / research | Tham gia rà soát kịch bản phỏng vấn kỹ thuật viên lab; nghiên cứu khoảng trống của các công cụ ImageJ và OpenCFU. | Giúp nhóm nhận diện takeaway cốt lõi: không làm tool desktop phức tạp nhiều tham số mà tập trung vào Web UI tinh gọn và auto-export Excel. |
| Workflow nhóm | Đề xuất và cùng nhóm hoàn thiện sơ đồ Current State 6 bước (15-20') và Future State 5 bước (< 2'); trực tiếp thiết kế luồng export kết quả tự động sang Excel. | Định hình workflow mạch lạc, rút ngắn hơn 80% thời gian xử lý và xóa bỏ hoàn toàn bước gõ tay vào bảng tính Excel. |
| Problem Statement | Rà soát và siết chặt các trường của Problem Statement v0 và v1, đặc biệt là ranh giới Boundary (LÀM vs KHÔNG LÀM) và Success Metric. | Định hình bản Problem Statement chặt chẽ, thực tế, không bị tham vọng viển vông (không làm định danh loài, không cố đếm đĩa TNTC > 300 CFU). |
| Rule / Workflow / Agent | Điều phối nhóm trả lời 5 câu hỏi chốt; phản biện các ý kiến đề xuất làm Bio-Robotics Agent tự động hóa hoàn toàn. | Giữ nhóm kiên định chọn cấp độ Workflow kết hợp Rule định dạng Excel ở bước cuối, bảo đảm tính an toàn và khả thi trong phạm vi lab. |
| Decision | Chủ trì đánh giá bảng tiêu chí Go / Not Yet / No-Go; cùng nhóm thiết lập kế hoạch pilot 30 đĩa và 3 điều kiện rollback cụ thể. | Nhóm tự tin đưa ra quyết định GO dựa trên bằng chứng định lượng rõ ràng và quy trình pilot an toàn. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Dấu tay rõ nhất của tôi là vai trò Nhóm trưởng chủ trì điều phối giúp nhóm chuyển hướng đồng thuận dứt khoát sang bài toán vi sinh, đồng thời trực tiếp đề xuất và hoàn thiện cấu trúc workflow hệ thống 5 bước tích hợp khâu tự động xuất dữ liệu Excel, xóa bỏ hoàn toàn thao tác gõ tay thủ công.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý thêm các góc nhìn problem từ bối cảnh kỹ sư AI theo 4 lăng kính. | Giúp mở rộng lăng kính "pain từ người khác" (thiếu context khi sửa code đồng nghiệp, khó truy vết regression). | Đưa ra các ý tưởng quá rộng và viển vông như "AI tự động merge toàn bộ PR", "Agent tự sửa cả codebase". | Loại bỏ toàn bộ các ý tưởng viển vông, tự lọc ra các điểm nghẽn có trải nghiệm thật và tự ước lượng số đo baseline (phút, lần/tuần). |
| Problem Card | Phản biện điểm yếu của Problem Card #1 (đánh giá impact sau merge). | Chỉ ra rủi ro khái niệm "impact" quá rộng và cảnh báo số liệu hiện tại mới là ước lượng cá nhân. | Gợi ý dùng AI phân tích toàn bộ AST repo mà không lường trước chi phí tính toán và sự phụ thuộc ngôn ngữ. | Thu hẹp phạm vi vào việc draft impact map và test checklist, nhấn mạnh kỹ sư là human boundary bắt buộc duyệt. |
| Workflow | Hỗ trợ format sơ đồ ASCII và rà soát các điểm handoff trong quy trình trước/sau. | Trình bày sơ đồ trực quan, gợi ý bước chuẩn hóa ánh sáng và nền chụp ảnh đĩa Petri. | Tự ý bỏ qua bước con người kiểm tra (đề xuất AI tự lưu thẳng vào database mà không cần NCV xác nhận). | Bổ sung bước then chốt: NCV xem Overlay mask chấm màu và dùng chuột click ±1 sửa lỗi trong 45s trước khi xuất Excel. |
| Research | Tìm kiếm tài liệu và đối chuẩn các công cụ đếm khuẩn lạc tự động hiện có trên thị trường. | Cung cấp nhanh tên các công cụ nổi tiếng (OpenCFU, ImageJ, Interscience Scan). | Tự bịa số liệu về độ chính xác (hallucinate) và không cung cấp được đường link kiểm chứng chuẩn xác. | Tự tay truy cập và xác thực link chính thức từ SourceForge, ImageJ.net và Interscience; trích xuất điểm yếu thực tế của từng tool. |
| Problem Statement | Đóng vai phản biện (Devil's Advocate) để tìm chỗ mơ hồ trong Problem Statement v0. | Chỉ ra rằng điều kiện chụp ảnh đầu vào và dải mật độ CFU tối ưu chưa được nêu rõ ràng. | Viết lại Problem Statement với ngôn từ tiếp thị hoa mỹ, mang tính quảng cáo giải pháp hơn là bài toán kỹ thuật. | Giữ lại format kỹ thuật chặt chẽ, bổ sung giới hạn dải đo vi sinh chuẩn (30 - 300 CFU) và quy định rõ Boundary LÀM / KHÔNG LÀM. |
| Rule / Workflow / Agent | Phản biện tính cần thiết giữa các cấp độ Rule, Workflow và Agent. | Cung cấp góc nhìn về các rủi ro kỹ thuật khi cố xây dựng hệ thống Agent phức tạp. | Xu hướng thiên vị Agent để nghe "thông minh" và "tiên tiến" hơn dù không phù hợp thực tế. | Kiên quyết cùng nhóm chốt mức Workflow; AI chỉ xử lý khâu thị giác máy tính và phân tách vùng, máy chạy Rule ở bước xuất Excel. |
| Decision | Gợi ý các kịch bản rủi ro cần kiểm tra trong đợt thử nghiệm pilot. | Đưa ra checklist các trường hợp biên (đĩa thạch nứt, bọt khí, khuẩn đổi màu). | Đề xuất thời gian thử nghiệm kéo dài hàng tháng trời không khả thi với một pilot nhỏ. | Tự chốt phạm vi pilot tinh gọn trên 30 đĩa Petri thực tế với 3 tiêu chí đo lường cụ thể và 3 điều kiện dừng (rollback) dứt khoát. |

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Khi lắng nghe phần trình bày top 3 problem của các thành viên trong nhóm, tôi thực sự bất ngờ trước sự đa dạng về góc nhìn giữa các bài toán phần mềm quen thuộc và bài toán đếm khuẩn lạc vi sinh đầy tính thực tế của Tình. Ban đầu, tôi khá tâm đắc với đề xuất phân tích tác động code sau merge của bản thân, nhưng khi cùng nhóm đối chiếu với 7 tiêu chí đánh giá, tôi nhận thấy bài toán vi sinh có nỗi đau nhức nhối hơn và đo lường trực quan hơn rất nhiều. Trong quá trình thảo luận, nhóm từng có lúc suýt rơi vào bẫy solution-first khi có thành viên đề xuất xây dựng một Bio-Robotics Agent tự động hóa toàn diện từ khâu gắp đĩa đến định danh vi khuẩn cho "ngầu". Với vai trò Nhóm trưởng, tôi đã chủ động điều phối, giúp từng bạn bóc tách bản chất điểm nghẽn và kéo cả nhóm về với nguyên tắc: quy trình tuyến tính này chỉ cần một AI Workflow tinh gọn có chốt chặn con người. Dấu tay rõ nét nhất của tôi trong sản phẩm cuối là việc chủ trì phiên chấm điểm để cả 6 thành viên đồng thuận 100% chuyển hướng đề tài, đồng thời trực tiếp đề xuất và hoàn thiện kiến trúc workflow hệ thống 5 bước. Tôi cũng đặc biệt chú trọng thiết kế khâu tự động xuất dữ liệu ra file Excel có kèm đầy đủ metadata, giúp xóa bỏ triệt để thao tác nhập liệu thủ công dễ gây sai số của nghiên cứu viên. Qua bài tập này, tôi nhận ra điều khó nhất khi viết Problem Statement chính là xác lập ranh giới Boundary: phải cực kỳ dũng cảm để vạch rõ những việc hệ thống "KHÔNG LÀM", như từ chối tự động phê duyệt nếu thiếu xác nhận của người dùng hay từ chối đếm các đĩa mật độ quá dày (TNTC). Nếu có cơ hội làm lại, tôi sẽ challenge nhóm sớm hơn và quyết liệt hơn ở khâu chuẩn hóa thiết bị chụp ảnh đầu vào (giá đỡ và đèn LED tản sáng), bởi chất lượng ảnh chụp chính là yếu tố sống còn quyết định sự thành bại của thuật toán Watershed.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI
