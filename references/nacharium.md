# Hội Đồng Thẩm Định Nacharium — Chi Tiết

> Cơ chế kiểm soát chất lượng cuối cùng trước khi chương được PASS.
> 2 chế độ: Nhanh (5 vai) cho mỗi chương, Đầy đủ (13 personas) cho round OIF.

---

## 2 Chế Độ Hoạt Động

| Chế độ | Số vai | Khi nào | Ngưỡng PASS | Thời gian |
|--------|--------|---------|-------------|-----------|
| **Nhanh** | 5 vai | Bước +C trong FORGE+C, mỗi chương | ≥ 7/10 | 15 phút |
| **Đầy đủ** | 13 personas | Cuối round OIF, sau ghép toàn bộ | ≥ 8.5/10 | 30 phút |

---

## Chế Độ Nhanh — 5 Vai

### 1. Biên Tập Trưởng

Kiểm tra:
- Cấu trúc chương: có arc rõ ràng? (mở → phát triển → đỉnh → kết)
- Nhịp: có đỉnh/thung lũng?
- Giọng văn: nhất quán với Voice Kit?
- Coherence: logic nội tại?

### 2. Nhà Phê Bình Văn Học

Kiểm tra:
- Chiều sâu: có tầng nghĩa?
- Ẩn dụ: hệ hình ảnh có nhất quán?
- Biểu tượng: đồ vật neo có ý nghĩa?
- Subtext: cái không nói ra?

### 3. Độc Giả Khó Tính

Kiểm tra:
- Hook: 3 câu đầu có kéo vào?
- Chỗ chán: đoạn nào muốn bỏ qua?
- Page-turner: có muốn đọc chương tiếp?
- Ám ảnh: hình ảnh nào nhớ sau khi gấp sách?

### 4. Kỹ Sư Ngôn Ngữ (Rà Soát Vết Tích AI)

Checklist 10 mục:
- [ ] Padding/filler: câu cắt đi mà không mất ý?
- [ ] Từ "mùi AI": "một cách [tính từ]", "không khỏi", "dường như"
- [ ] TELL thay vì SHOW: giải thích cảm xúc trực tiếp?
- [ ] Giọng trôi: khác DNA Sample?
- [ ] Ẩn dụ cliché: biển, trời, vực?
- [ ] Nhịp đều: thiếu variation?
- [ ] Thoại phẳng: không phân biệt nhân vật?
- [ ] Cấu trúc lặp: mở đầu đoạn giống nhau?
- [ ] Markdown lọt vào prose?
- [ ] Over-explaining: giải thích cái đã hiểu?

### 5. Quản Lý Liên Tục

Kiểm tra:
- Nhân vật: hành vi nhất quán với chương trước?
- Worldbuilding: luật chơi có khớp?
- Timeline: thời gian có logic?
- Foreshadowing: đã gieo/gặt đúng?
- Resonance: motif xuất hiện đúng nghĩa mới?

---

## Chế Độ Đầy Đủ — 13 Personas

| # | Persona | Vai trò | Tìm kiếm gì |
|---|---------|---------|-------------|
| 1 | **Kẻ Soi Lỗi** | Kiểm tra logic | Plot holes, timeline, mâu thuẫn |
| 2 | **Kẻ Háo Hức** | Đánh giá nhịp | Pacing, hook, page-turner |
| 3 | **Kẻ Hoài Nghi** | Thẩm vấn | Motivation nhân vật, logic hành vi |
| 4 | **Kẻ Đa Cảm** | Cảm xúc | Depth, catharsis, có khóc không? |
| 5 | **Kẻ Thẩm Mỹ** | Nghệ thuật | Nhịp văn, hình ảnh, ẩn dụ |
| 6 | **Kẻ Lười** | Sàng lọc | Chỗ nào chán? Skip đoạn nào? |
| 7 | **Kẻ Phân Tích** | Cấu trúc | Symbolism, foreshadowing, pattern |
| 8 | **Kẻ Khắt Khe** | Benchmark | Cliché? Predictable? Đã đọc 1000 sách |
| 9 | **Kẻ Lần Đầu** | Accessibility | Có hiểu không? Có cuốn vào? |
| 10 | **Kẻ Dịch Giả** | Quốc tế | Câu nào không dịch được? |
| 11 | **Kẻ Nghe Kể** | Audio | Audiobook trôi? Vấp ở đâu? |
| 12 | **Kẻ Biên Tập** | Sửa chữa | Cắt gì? Thêm gì? Sửa gì? |
| 13 | **Kẻ Mua Sách** | Thương mại | 3 trang đầu ở hiệu sách, có mua? |

### Cách spawn

Spawn 1 sub-agent đóng vai tất cả 13 personas. THÔNG BÁO rõ cho user: gồm những ai, vai trò.

### Khi nào dùng 5 vs 13

- **5 vai:** Mỗi chương, đủ nhanh, đủ sâu cho quality gate
- **13 personas:** Cuối round OIF (nhiều chương), hoặc khi muốn đánh giá sâu scene quan trọng
- Có thể chọn 5-7 personas phù hợp thể loại thay vì dùng cả 13

---

## Bảng Chấm Điểm — 5 Tiêu Chí

| Tiêu chí | Mô tả | Điểm (1-10) |
|----------|--------|-------------|
| **Giọng văn** | Nhất quán, sắc bén, không AI | /10 |
| **Cảm xúc** | Đường cong, chiều sâu, không sến | /10 |
| **Kỹ thuật** | Show-don't-tell, nhịp, constraint | /10 |
| **Coherence** | Với chương trước, worldbuilding | /10 |
| **Ám ảnh** | Người đọc nhớ sau khi gấp sách? | /10 |
| **Trung bình** | | **/10** |

---

## AI Traces Check

### Từ cấm TUYỆT ĐỐI

```
tapestry, resonate, nuanced, delve, testament,
landscape, multifaceted, intricate
```

### Checklist kiểm tra thêm

- [ ] Câu sáo rỗng AI
- [ ] Markdown lọt vào text (**, #, >)
- [ ] Cấu trúc lặp (mở đầu đoạn giống nhau)
- [ ] Over-explaining
- [ ] Symbolism phồng (giải thích ẩn dụ thay vì gợi)
- [ ] Em dash spam (quá nhiều dấu —)
- [ ] Giọng nịnh ("brilliant", "stunning")

---

## Quy Tắc PASS/FAIL

### Chế độ nhanh (5 vai)

- **PASS:** Trung bình ≥ 7/10
- **FAIL:** Trung bình < 7/10 → chỉ ra cụ thể cần sửa → quay lại Render hoặc Grind

### Chế độ đầy đủ (13 personas)

- **PASS:** Trung bình ≥ 8.5/10
- **FAIL:** Trung bình < 8.5/10 → spawn Editor sửa theo report → re-submit
- Nếu < 8.5 → sửa → re-submit. Lặp cho đến khi ≥ 8.5

---

## Format Report

### Chế độ nhanh

```
COUNCIL — KẾT QUẢ THẨM ĐỊNH NHANH

Chương: [N]
Biên tập trưởng: [nhận xét 2-3 câu]
Nhà phê bình: [nhận xét 2-3 câu]
Độc giả khó tính: [nhận xét 2-3 câu]
Kỹ sư ngôn ngữ: [nhận xét 2-3 câu + checklist AI traces]
Quản lý liên tục: [nhận xét 2-3 câu]

Điểm: Giọng [X] | Cảm xúc [X] | Kỹ thuật [X] | Coherence [X] | Ám ảnh [X]
Trung bình: [X]/10
Kết luận: PASS / FAIL
Nếu FAIL: [cần sửa cụ thể]
```

### Chế độ đầy đủ

File: `"[Tên Tác Phẩm] - Đánh Giá Hội Đồng Nacharium.md"`

Nội dung:
1. 13 nhận xét (mỗi persona 3-5 câu)
2. ĐIỂM TỔNG /10
3. 3 điểm mạnh + 3 điểm yếu
4. TOP 5 chỗ cần sửa cụ thể
5. Câu hay nhất cả cuốn
6. Chương hay nhất / yếu nhất
7. AI traces check
8. Ready xuất bản chưa?

---

## Prompt Council — Chế Độ Nhanh

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

## Prompt Council — Chế Độ Đầy Đủ

```
NACHARIUM — HỘI ĐỒNG THẨM ĐỊNH ĐẦY ĐỦ

Đọc toàn bộ tác phẩm/chương dưới đây qua 13 góc nhìn.

[PASTE TÁC PHẨM]
[PASTE DNA GIỌNG VĂN]

Mỗi persona cho nhận xét 3-5 câu:
1. Kẻ Soi Lỗi | 2. Kẻ Háo Hức | 3. Kẻ Hoài Nghi | 4. Kẻ Đa Cảm
5. Kẻ Thẩm Mỹ | 6. Kẻ Lười | 7. Kẻ Phân Tích | 8. Kẻ Khắt Khe
9. Kẻ Lần Đầu | 10. Kẻ Dịch Giả | 11. Kẻ Nghe Kể | 12. Kẻ Biên Tập
13. Kẻ Mua Sách

Sau đó:
- Chấm điểm 1-10: Giọng văn / Cảm xúc / Kỹ thuật / Coherence / Ám ảnh
- 3 điểm mạnh + 3 điểm yếu
- TOP 5 chỗ cần sửa cụ thể
- Câu hay nhất
- AI traces check (từ cấm + checklist)
- Kết luận: PASS (≥ 8.5) hay FAIL?
```

---

## Quy Tắc Nacharium

1. Khi spawn → THÔNG BÁO rõ: gồm những ai, vai trò
2. Hội đồng luôn có thể THAY ĐỔI thành viên tuỳ thể loại
3. SAU KHI có report → SELF-ABSORPTION (bắt buộc)
4. 13 personas là công cụ ĐÁNH GIÁ, không phải SÁNG TẠO
5. KHÔNG để personas ảnh hưởng giọng văn — giọng do DNA Sample quyết định

---

*Quay lại: [SKILL.md](../SKILL.md) · Xem thêm: [forge-workflow.md](forge-workflow.md) · [oif-loop.md](oif-loop.md)*
