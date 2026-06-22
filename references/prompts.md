# Prompt Templates — 8 Prompts Copy-Paste

> 8 prompt mẫu sẵn sàng dùng + Công thức 3 Tầng.

---

## Công Thức Prompt 3 Tầng

| Tầng | Nội dung | Thiếu thì sao |
|------|----------|----------------|
| **A: LUẬT** | POV, tone, cấm gì, nhịp câu, độ dài | AI viết chung chung |
| **B: ĐẦU RA** | Template scene, checklist giác quan, ẩn dụ, vật thể neo | Scene mờ nhạt |
| **C: CÚ ĐẤM** | 1 thứ duy nhất làm người đọc mất ngủ | Scene "ổn" nhưng không đáng nhớ |

---

## Prompt A: Scene Rendering

```
SCENE RENDERING

Viết scene loại [tên template nếu có].
POV: [ngôi mấy, nhân vật nào].
Tone: [mô tả — ví dụ: lạnh, khô, sắc].

Luật:
- Show-don't-tell
- Không giải thích lore trực tiếp
- Câu ngắn dần khi căng thẳng
- Slow-motion ở [beat nào]
- Aftermath chiếm nhiều nhất

Stakes: [nhân vật mất gì nếu thất bại].

Cú đấm: kết thúc bằng [hình ảnh/câu nói ám ảnh cụ thể].

Phải có 5 chi tiết giác quan (mùi, nhiệt, texture, âm, ánh sáng).

Độ dài: 400-600 từ.
```

**Khi nào:** Render beat trong FORGE+C bước R.

---

## Prompt B: Brainstorm 15 Hướng

```
BRAINSTORM

Đưa 15 biến thể cho cùng 1 scene (cùng sự kiện), mỗi biến thể
đổi 1 thứ: POV, thứ tự thời gian, đồ vật biểu tượng, loại twist, nhịp câu.

Mỗi biến thể 3-5 dòng:
- Mục tiêu
- Xung đột
- Hình ảnh chốt

Sự kiện cần brainstorm: [mô tả sự kiện]
```

**Khi nào:** Bắt đầu chương/scene mới, mở rộng khả năng.

---

## Prompt C: Adversarial Edit

```
ADVERSARIAL EDIT

Đây là đoạn văn:
[PASTE ĐOẠN VĂN]

Hãy:
(1) Chỉ ra 7 câu đang TELL và đề xuất thay bằng hành vi/chi tiết
(2) Cắt 25% chữ mà không mất ý — đánh dấu phần cắt
(3) Tìm 5 chỗ lặp nhịp/lặp từ
(4) Đề xuất 2 câu kết mạnh hơn (không sáo rỗng)
```

**Khi nào:** Sau mỗi draft, FORGE+C bước G.

---

## Prompt D: Voice Calibration

```
VOICE CALIBRATION

Đây là DNA giọng văn của tiểu thuyết:

[PASTE 300-500 TỪ MẪU]

Duy trì tần số này:
- Nhịp điệu
- Độ dài câu
- Mật độ ẩn dụ
- Cách dùng dấu câu
- Khoảng trắng

Nếu bất kỳ câu nào trôi khỏi tần số này — viết lại ngay.
```

**Khi nào:** Đầu mỗi phiên viết mới.

---

## Prompt E: Intensity Map

```
INTENSITY MAP

Tiểu thuyết có [X] chương.
Chương đang viết là Chương [N] — [vị trí: mở đầu/giữa/cao trào/kết].

Cường độ thang 1-10:
  Chương trước = [Y]
  CHƯƠNG NÀY = [Z]
  Chương sau = [W]

Cường độ [Z] nghĩa là: [mô tả cảm giác cần tạo].

Mỗi câu phải mang trọng lượng của cường độ [Z].
```

**Khi nào:** Trước mỗi chương.

---

## Prompt F: Cross-Check

```
CROSS-CHECK

Đây là 3 đoạn then chốt từ chương trước:
[PASTE]

Đây là 3 đoạn then chốt từ chương vừa viết:
[PASTE]

Có mâu thuẫn nào về:
(1) Tính cách nhân vật — hành vi có nhất quán?
(2) Quy tắc thế giới — worldbuilding có khớp?
(3) Timeline — thời gian có logic?
(4) Chi tiết vật lý — đồ vật, địa điểm, ngoại hình?

Nếu có — chỉ ra cụ thể và đề xuất sửa.
```

**Khi nào:** FORGE+C bước C.

---

## Prompt G: Ghost Reader

```
GHOST READER

Quên mọi thứ về cốt truyện. Đọc đoạn này như người chưa biết gì:

[PASTE ĐOẠN VĂN]

Liệt kê:
(1) 3 câu hỏi tự nhiên nảy ra trong đầu người đọc
(2) Chỗ nào có thể chán và bỏ đọc
(3) Hình ảnh nào ám ảnh sau khi gấp sách
```

**Khi nào:** Sau KT5 Adversarial Edit, hoặc bất kỳ lúc nào cần đánh giá.

---

## Prompt H: Council — Hội Đồng Nacharium

```
COUNCIL — HỘI ĐỒNG THẨM ĐỊNH NACHARIUM

Đây là chương [N] vừa viết:
[PASTE CHƯƠNG]

Đây là DNA giọng văn:
[PASTE DNA SAMPLE]

Đây là 3 đoạn then chốt chương trước:
[PASTE]

Hãy thẩm định với 5 vai:
1. BIÊN TẬP TRƯỞNG: cấu trúc, nhịp, giọng văn, coherence
2. NHÀ PHÊ BÌNH: chiều sâu văn chương, ẩn dụ, subtext
3. ĐỘC GIẢ KHÓ TÍNH: chỗ chán, chỗ hay, có muốn đọc tiếp?
4. KỸ SƯ NGÔN NGỮ: vết tích AI, padding, giọng phèn, từ lặp
5. QUẢN LÝ LIÊN TỤC: mâu thuẫn nhân vật, worldbuilding, timeline

Chấm điểm 1-10 cho: Giọng văn / Cảm xúc / Kỹ thuật / Coherence / Ám ảnh
Kết luận: PASS hay FAIL? Nếu FAIL — chỉ ra cụ thể cần sửa gì.
```

**Khi nào:** FORGE+C bước +C, sau Cross-check.

---

## Prompt Elevate (Bổ sung)

```
ELEVATE

Đây là 3 câu hay nhất trong chương:
1. [câu 1]
2. [câu 2]
3. [câu 3]

Đây là đẳng cấp cần đạt. Đọc lại toàn bộ chương dưới đây
và nâng MỌI câu lên cùng đẳng cấp với 3 câu này.
Giữ nguyên sự kiện và cấu trúc.

[PASTE TOÀN BỘ CHƯƠNG]
```

**Khi nào:** FORGE+C bước E.

---

## Hệ Thống Lệnh Tắt — Paste Vào System Prompt

```
Bạn hiểu các lệnh tắt sau. Khi tôi gõ lệnh, chuyển ngay sang chế độ tương ứng:

BRAINSTORM = Bùng nổ 10-15 ý tưởng đa dạng, không tự kiểm duyệt
VIẾT = Chuyển chế độ văn chương: prose đẹp, nhịp điệu, cảm xúc
PHÂN TÍCH = Đánh giá khách quan: điểm mạnh/yếu, gợi ý cải thiện
OUTLINE = Tạo dàn ý chi tiết, xác định turning points, arc rõ ràng
10X = 10 biến thể của ý tưởng vừa nêu
TWIST = Thêm plot twist bất ngờ nhưng hợp logic
DEEPER = Đào sâu tâm lý/động cơ/vết thương nhân vật
CONFLICT+ = Tăng xung đột và stakes
SENSORY = Thêm chi tiết giác quan: mùi, vị, âm, nhiệt, texture
DIALOGUE = Viết đoạn đối thoại với giọng riêng cho từng nhân vật
REVERSE = Đảo ngược/subvert expectation
EMOTION = Tăng cường chiều sâu cảm xúc mà KHÔNG sến
COUNCIL = Spawn Hội đồng Nacharium thẩm định. Chấm điểm 1-10. Rà soát vết tích AI.
OIF = Bắt đầu Omni Infinity Forge loop. Seed → Novelist → Council → Final → Seed mới.
```

---

*Quay lại: [SKILL.md](../SKILL.md) · Xem thêm: [techniques.md](techniques.md) · [forge-workflow.md](forge-workflow.md)*
