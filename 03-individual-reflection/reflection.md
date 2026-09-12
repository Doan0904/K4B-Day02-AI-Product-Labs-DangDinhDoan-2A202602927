# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Đặng Đỉnh Đoàn
- Mã học viên: 2A202602927
- Nhóm: 6 thành viên (Đoàn – facilitator, Minh, Tiến, Đức, Giang, Hạ) — vai trò của tôi: **Facilitator**
- Candidate problem nhóm chọn: Sinh viên phải xếp hàng hai lần để nhận suất cơm.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Tự scan 7 problems quanh trải nghiệm nhà ăn/di chuyển; chọn top 3 (xếp hàng 2 lần, trả dĩa, tự lấy mâm dĩa), mỗi card có workflow + bottleneck + metric | Đưa vào nhóm 3 candidate cùng domain nhà ăn, tạo nền cho cluster A |
| Pitch Problem Card | Pitch card #1 "xếp hàng hai lần nhận cơm": nêu actor, workflow 4 bước, bottleneck và 2 câu hỏi muốn nhóm challenge | Bài được nhóm chấm cao nhất (34đ) và chọn làm candidate |
| Challenge bài của bạn khác | Vặn bài #5 "đợi thang máy" (có bấm giờ và can thiệp được trong phạm vi lab không) và #4 "Google Maps" (nhóm có kiểm soát được workflow của Google không) | Hai bài bị chấm thấp hơn, không vào shortlist; nhóm dồn về hướng nhà ăn |
| Gom trùng / cluster | Với vai trò facilitator, gom 6 candidate thành 3 cụm (nhà ăn / trì hoãn giờ học / lập kế hoạch cá nhân) | Nhóm thấy #1 và #2 trùng pattern nhà ăn, dồn hướng về một bài |
| Chọn candidate | Điều phối chấm 7 tiêu chí cho 3 bài shortlist, ép mỗi người nói rõ vì sao cho điểm cao/thấp; chốt đồng thuận | Nhóm chọn "xếp hàng hai lần" (34đ), có nhật ký hội tụ rõ |
| Validation / research | Điều phối khảo sát nhanh (phỏng vấn 3 bạn + poll 10 bạn) và tổng hợp; research tool/pattern chính do Tiến & Giang, tôi ráp lại thành takeaway | Chốt insight: pain tập trung giờ cao điểm ~13h, không phải cả ngày |
| Workflow nhóm | Cung cấp current/future workflow từ card cá nhân; dựng sơ đồ nhóm thành ảnh `02-group-problem-statement-workflow.png` | Nhóm có workflow trước/sau + hình minh hoạ để nộp |
| Problem Statement | Đóng góp nội dung 6 field (actor, bottleneck, metric, boundary…) từ card của mình để writer chốt v0 → v1 | PS bám sát đúng bottleneck "xếp hàng hai lần" |
| Rule / Workflow / Agent | Dẫn phần so sánh R/W/A trên cùng một bài; phân tích và phác thiết kế "Canteen Flow Agent" như hướng Phase 2 | Nhóm chốt **Workflow** là mức chọn, **Agent để Phase 2** có điều kiện |
| Decision | Dẫn bảng Final decision 6 câu; chốt "Not Yet cho phần AI — Go ngay với Rule" | Quyết định trung thực với dữ liệu (chưa có baseline bấm giờ) |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Bài toán cuối là candidate của tôi (xếp hàng hai lần nhận cơm), và tôi là người dựng sơ đồ
workflow trước/sau cùng phần phân tích Rule/Workflow/Agent + thiết kế Agent Phase 2 cho nhóm.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Nhờ AI trau chuốt lại câu chữ mô tả problem | Diễn đạt gọn, rõ hơn | Không biết trải nghiệm thật của tôi, dễ thêm ý chung chung | Chỉ giữ 7 problem tôi thật sự quan sát ở nhà ăn, bỏ ý bịa |
| Problem Card | Không dùng (tự viết card để bám sát quan sát của mình) | — | — | Tự chốt bottleneck "hai lần xếp hàng" theo thực tế |
| Workflow | Nhờ AI biến workflow của tôi thành sơ đồ PNG theo mẫu HTML | Ra hình chuyên nghiệp, nhanh | Điền thời gian ~9'/~6' là ước lượng, không phải số đo thật | Ghi rõ baseline là ước lượng, cần bấm giờ thật trước khi chốt |
| Research | Nhờ AI tìm tool/pattern tương tự + link | Gợi ra single-queue, QR check-in, "popular times", đếm người | Vài link chưa chắc chính thức, không có số liệu verify | Đánh dấu "cần kiểm link", không dùng số liệu chưa verify |
| Problem Statement | Nhờ AI phản biện field mơ hồ của PS v0 | Chỉ ra metric thời gian còn yếu vì baseline là ước lượng | Có xu hướng viết metric "cho đẹp" | Tách metric "số lần xếp hàng" (chắc chắn) khỏi metric thời gian (cần đo) |
| Rule / Workflow / Agent | Nhờ AI so sánh R/W/A và thiết kế agent | Dựng đủ giải phẫu "Canteen Flow Agent" + guardrail | Nghiêng về đề xuất Agent hơi sớm, "cho ngầu" | Kéo về Workflow, đẩy Agent xuống Phase 2 với điều kiện trigger rõ |
| Decision | Nhờ AI dựng bảng Final decision | Liệt kê đủ 6 câu hỏi kiểm | Dễ chốt "Go" vội dù chưa có baseline | Tự chốt "Not Yet cho AI — Go với Rule" cho trung thực với dữ liệu |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

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
Khi nghe top 3 của các bạn, tôi nhận ra vấn đề tôi thấy "hiển nhiên" (xếp hàng hai lần)
thật ra trùng pattern với bài trả dĩa của một bạn khác, nên gom cụm giúp cả nhóm nhìn rõ
đâu là hướng đáng đào sâu. Có một lúc nhóm hơi solution-first: khi bàn tới AI, chúng tôi
bị cuốn vào ý tưởng làm hẳn một Agent tự điều phối "cho ngầu", nghe rất hay. Nhưng khi tự
hỏi lại 5 câu chốt thì thấy phần lõi — bỏ một lần xếp hàng — chỉ cần một process fix (gộp
vé bằng QR + một hàng chờ), hoàn toàn chưa cần AI. Tôi cũng tự đổi ý sau khi chính mình
đặt câu hỏi challenge: liệu "hai lần xếp hàng" hay "tốc độ phục vụ" mới là nguyên nhân chính?
Vì chưa chắc, nhóm quyết định thêm bước validation và tôi hạ quyết định từ "làm AI" xuống
"Not Yet cho AI — Go với Rule". Đóng góp thật của tôi là bài toán cuối (candidate của tôi),
sơ đồ workflow trước/sau, và phần phân tích Rule/Workflow/Agent. Điều khó nhất khi viết
Problem Statement là metric: tôi từng để "giảm ~40% thời gian chờ" nhưng nhận ra baseline
9 phút mới chỉ là ước lượng, chưa bấm giờ thật. Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn
ngay từ đầu ở chỗ số liệu: bắt bấm giờ thật trước khi chốt bất kỳ metric nào, và hỏi sớm
hơn "bài này có thật sự cần AI không" thay vì để tới Phase 6 mới kéo lại.
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
