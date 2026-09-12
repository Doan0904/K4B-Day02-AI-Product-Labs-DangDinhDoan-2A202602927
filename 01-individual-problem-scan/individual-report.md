# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Đặng Đỉnh Đoàn
- Mã học viên: 2A202602927
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Sinb viên năm 4
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem): Đi học đào tạo từ Vin

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 |Lặp lại | Phải xếp hàng nhận vé ăn rồi tiếp tục xếp hàng bỏ vé vào hộp để nhận cơm|Sinh viên, nhân viên nhà ăn|Hai lần xếp hàng cho một suất ăn|
| 2 |Tốn thời gian|Quy trình nhận cơm gồm nhiều bước: lấy vé, bỏ vé, nhận cơm|Sinh viên|Thời gian chờ kéo dài|
| 3 |Lặp lại|Sinh viên phải tự lấy mâm và dĩa cơm trước khi nhận suất ăn|Sinh viên|Thêm một bước thao tác trong quy trình|
| 4 |Tốn thời gian|Việc lấy mâm và dĩa cơm có thể gây ùn tắc tại khu vực nhận dụng cụ ăn|Sinh viên|Dòng người bị chậm tại khu vực lấy mâm, dĩa|
| 5 |Pain từ người khác|Nhân viên nhà ăn phải xử lý việc nhận vé và kiểm tra vé trước khi phục vụ cơm|Nhân viên nhà ăn|Phải xử lý vé trước khi giao cơm|
| 6 |AI có thể tốt hơn|Chưa có hệ thống tối ưu hóa quá trình xếp hàng và phân luồng sinh viên tại nhà ăn|Sinh viên, nhân viên|Hàng chờ dài, tắc nghẽn|
| 7 |Tốn thời gian|Sau khi ăn xong, sinh viên phải tiếp tục xếp hàng để trả dĩa|Sinh viên|Phải chờ thêm một lần sau khi dùng bữa|
| 8 | | | | |
| 9 | | | | |
| 10 | | | | |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: Trao chuốt lại từ
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [ ] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [ ] Dùng ít nhất 3/4 lăng kính
- [ ] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| **1** | **Phải xếp hàng nhận vé ăn rồi tiếp tục xếp hàng bỏ vé vào hộp để nhận cơm** | - Actor rõ: sinh viên.<br>- Bottleneck cụ thể: phải xếp hàng 2 lần trong cùng quy trình nhận cơm.<br>- Có thể đo thời gian chờ và số người trong hàng. | Chưa có số liệu chính xác về thời gian chờ trung bình và số người bị ảnh hưởng. |
| **2** | **Sau khi ăn xong, sinh viên phải tiếp tục xếp hàng để trả dĩa** | - Workflow đơn giản, dễ quan sát và vẽ.<br>- Bottleneck rõ tại khu vực trả dĩa.<br>- Có thể đo thời gian chờ và số người xếp hàng. | Chưa biết thời gian chờ thực tế và mức độ ùn tắc vào các khung giờ khác nhau. |
| **3** | **Sinh viên phải tự lấy mâm và dĩa cơm trước khi nhận suất ăn** | - Actor rõ: sinh viên.<br>- Là một bước cụ thể trong workflow nhận cơm, không quá rộng.<br>- Có thể đo thời gian thực hiện và mức độ gây chậm dòng người. | Chưa chắc đây có phải bottleneck lớn hay chỉ là một bước nhỏ trong toàn bộ quy trình. |
### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — [Tên problem]

```text
Problem 1 câu: Sinh viên phải xếp hàng hai lần để nhận suất cơm.

Actor: Sinh viên, nhân viên

Thời điểm / bối cảnh: Sau khi học buổi sáng, thời điểm 13h chiều.

Current workflow 3-7 bước:
1.Xếp hàng nhận vé
2.Xếp hàng bỏ vé
3.Nhận cơm
4.Lấy mâm dũa
5.Tới bàn ăn

Bottleneck: Hai lần xếp hàng

Impact: 
- Sinh viên mất thêm thời gian chờ đợi để nhận một suất cơm.
- Dễ xảy ra ùn tắc vào giờ cao điểm khoảng 13h.
- Ví dụ: giảm 50% tổng thời gian chờ so với quy trình hiện tại.

Success metric:
- Giảm thời gian chờ trung bình để nhận suất cơm.
- Bố trí lại quầy/khu vực nhận cơm để tạo một hàng chờ duy nhất.
- Phân luồng sinh viên hoặc bố trí thêm quầy vào giờ cao điểm.


Non-AI alternative:
- Gộp bước nhận vé và bỏ vé thành một bước.
- Bố trí lại quầy/khu vực nhận cơm để tạo một hàng chờ duy nhất.
- Phân luồng sinh viên hoặc bố trí thêm quầy vào giờ cao điểm.

AI hypothesis:
- Sử dụng AI để dự đoán lượng sinh viên đến nhà ăn theo từng khung giờ, từ đó tối ưu số quầy và phân luồng xếp hàng.
- Có thể sử dụng dữ liệu lịch học, thời gian và lượng người trong các ngày trước để dự đoán thời điểm ùn tắc.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[ ] Agent
[x] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — chưa đo phút

[1. Nhận vé: __'] → [2. Xếp hàng bỏ vé: __'] → [3. Nhận cơm: __'] → [4. Lấy mâm, dĩa: __']  <-- bottleneck: hai lần xếp hàng

FUTURE STATE — chưa đo phút

[1. Xếp hàng một lần: __'] → [2. Nhận cơm + mâm, dĩa: __'] → [3. Nhân viên review/kiểm tra: __']  <-- human boundary

Fallback: nếu AI sai thì quay về quy trình phân luồng thủ công hoặc quy trình xếp hàng hiện tại.
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — [Tên problem]

```text
Problem 1 câu:

Sinh viên phải tự lấy mâm và dĩa, tạo thêm một bước trong quy trình nhận suất cơm.

Actor:

Sinh viên, nhân viên nhà ăn

Thời điểm / bối cảnh:

Sau khi học buổi sáng, vào khoảng 13h khi lượng sinh viên đến nhà ăn đông.

Current workflow 3-7 bước:

1. Xếp hàng nhận vé
2. Xếp hàng bỏ vé
3. Nhận cơm
4. Lấy mâm, dĩa
5. Di chuyển đến khu vực ăn

Bottleneck:

Khu vực lấy mâm, dĩa có thể làm chậm dòng di chuyển của sinh viên.

Impact:

- Sinh viên phải thực hiện thêm thao tác trước khi bắt đầu ăn.
- Có thể gây ùn tắc nếu nhiều sinh viên cùng lấy mâm, dĩa.
- Làm tăng tổng thời gian từ lúc xếp hàng đến khi có thể bắt đầu ăn.

Success metric:

- Giảm thời gian lấy mâm, dĩa.
- Giảm số lượng sinh viên tập trung tại khu vực lấy mâm, dĩa.
- Ví dụ: giảm 30% thời gian thực hiện bước lấy mâm, dĩa.

Non-AI alternative:

- Bố trí lại vị trí mâm và dĩa để sinh viên dễ lấy hơn.
- Chuẩn bị sẵn mâm và dĩa theo từng cụm.
- Nhân viên hỗ trợ cấp mâm, dĩa vào giờ cao điểm.

AI hypothesis:

- Sử dụng AI để dự đoán lượng sinh viên đến nhà ăn theo từng khung giờ, từ đó chuẩn bị số lượng mâm, dĩa phù hợp trước giờ cao điểm.
- Có thể kết hợp dữ liệu lượng sinh viên để tối ưu cách bố trí khu vực lấy mâm, dĩa.

Quick gut:

[ ] No AI / process fix

[ ] Rule

[ ] Workflow

[ ] Agent

[x] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — ___ phút

[1 ...] → [2 ...] → [3 ...]  <-- bottleneck

FUTURE STATE — ___ phút

[1 ...] → [2 ...] → [3 ... review]  <-- human boundary

Fallback: ...
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — [Tên problem]

```text
Problem 1 câu:

Sau khi ăn xong, sinh viên phải tiếp tục xếp hàng để trả dĩa.

Actor:

Sinh viên, nhân viên nhà ăn

Thời điểm / bối cảnh:

Sau khi ăn trưa, đặc biệt vào thời điểm đông sinh viên khoảng 13h.

Current workflow 3-7 bước:

1. Ăn xong
2. Thu dọn dĩa và thức ăn thừa
3. Mang dĩa đến khu vực trả dĩa
4. Xếp hàng chờ trả dĩa
5. Trả dĩa cho nhân viên

Bottleneck:

Xếp hàng tại khu vực trả dĩa.

Impact:

- Sinh viên mất thêm thời gian chờ sau khi đã ăn xong.
- Có thể gây ùn tắc tại khu vực trả dĩa vào giờ cao điểm.
- Nhân viên phải tiếp nhận và xử lý từng lượt trả dĩa.

Success metric:

- Giảm thời gian chờ trung bình khi trả dĩa.
- Giảm số lượng sinh viên xếp hàng tại khu vực trả dĩa.
- Ví dụ: giảm 50% thời gian chờ so với quy trình hiện tại.

Non-AI alternative:

- Bố trí thêm điểm trả dĩa vào giờ cao điểm.
- Thiết kế lại khu vực trả dĩa để tạo luồng di chuyển một chiều.
- Phân loại vị trí bỏ thức ăn thừa và trả dĩa để giảm thời gian xử lý.

AI hypothesis:

- Sử dụng AI để dự đoán lượng sinh viên cần trả dĩa theo từng khung giờ, từ đó điều phối nhân viên và số điểm trả dĩa phù hợp.
- Có thể sử dụng dữ liệu lượng sinh viên theo thời gian để phát hiện và dự đoán thời điểm ùn tắc.

Quick gut:

[ ] No AI / process fix

[ ] Rule

[ ] Workflow

[ ] Agent

[x] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — chưa đo phút

[1. Ăn xong] → [2. Mang dĩa đến khu vực trả] → [3. Xếp hàng] → [4. Trả dĩa]  <-- bottleneck: xếp hàng

FUTURE STATE — chưa đo phút

[1. Ăn xong] → [2. Phân luồng đến điểm trả dĩa phù hợp] → [3. Nhân viên tiếp nhận/kiểm tra]  <-- human boundary

Fallback: nếu AI dự đoán hoặc phân luồng sai thì sử dụng quy trình trả dĩa thủ công và nhân viên điều phối trực tiếp.
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem: Sinh viên phải xếp hàng hai lần để nhận suất cơm.

Actor: Sinh viên, nhân viên nhà ăn

Current workflow:
[Nhận vé] → [Xếp hàng bỏ vé] → [Nhận cơm] → [Lấy mâm, dĩa]

Bottleneck: Hai lần xếp hàng trong cùng một quy trình nhận cơm.

Future workflow:
[Nhận vé + phân luồng] → [Nhận cơm + mâm, dĩa] → [Kiểm tra/điều phối]
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Đây là một workflow lặp lại hằng ngày và bottleneck rất rõ vì sinh viên phải xếp hàng hai lần chỉ để nhận một suất cơm. Có thể đo thời gian chờ trung bình, số người trong hàng và tổng thời gian từ lúc bắt đầu xếp hàng đến khi nhận được suất ăn. Nếu tối ưu được quy trình, có thể giảm thời gian chờ và tình trạng ùn tắc vào giờ cao điểm.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
Hai lần xếp hàng có thực sự là nguyên nhân chính khiến sinh viên phải chờ lâu, hay bottleneck nằm ở tốc độ phục vụ của nhân viên?

Nếu gộp hai bước xếp hàng thành một thì có làm phát sinh bottleneck mới tại quầy nhận cơm không?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:
- Tôi sửa gì:

### Self-check nộp phần 01
- [ ] Có 5+ problems + top 3 Cards đủ field
- [ ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ ] Đã chọn 1 card pitch + câu hỏi challenge
