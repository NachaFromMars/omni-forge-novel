# 12 Kỹ Thuật Cấp Cao — Chi Tiết + Prompts

> Mỗi kỹ thuật: lý do hoạt động, step-by-step, prompt mẫu, cảnh báo bẫy.

---

## KT1: PERSONA STACKING — Chồng Vai Theo Giai Đoạn

**Tại sao:** AI có DẢI GIỌNG. Persona cụ thể kéo output về đúng tần số.

**Step-by-step:**
1. Xác định giai đoạn: brainstorm, viết chiến đấu, viết tâm lý, biên tập
2. MÔ TẢ HIỆU ỨNG thay vì gọi tên tác giả. *"Câu văn nặng như chì, mỗi từ chịu trọng lực"* > *"viết như McCarthy"*
3. Kết hợp persona + constraint: persona cho GIỌNG, constraint cho LUẬT

**Prompt mẫu:**
```
Giai đoạn này bạn là biên tập viên tàn nhẫn. Giọng: lạnh, chính xác,
không khoan nhượng. Mỗi nhận xét kèm ví dụ cụ thể từ text. Không khen.
```

**⚠️ BẪY:** Gọi tên tác giả → AI bắt chước bề mặt (từ hoa mỹ) thay vì bản chất (cấu trúc, nhịp, góc nhìn). **Luôn mô tả HIỆU ỨNG.**

---

## KT2: CHAIN OF DENSITY — Nén Rồi Nở

**Tại sao:** AI viết dài hay padding. Viết từ cốt lõi ra ngoài tốt hơn viết dàn trải.

**Step-by-step:**
1. **Hạt nhân cảm xúc:** 1 câu, CẢM XÚC CỐT LÕI (VD: *"Người mẹ chọn cứu đứa con mà cô ít yêu hơn."*)
2. **NÉN:** AI tóm scene trong đúng 3 câu
3. **NỞ lần 1:** 3 câu → 1 trang
4. **NỞ lần 2:** 1 trang → 3-5 trang (thêm dialogue, sensory, inner voice)
5. **NỞ lần 3:** Chọn đoạn hay nhất, viết lại 200% cường độ

**Mẹo:** Sau mỗi lần nở: *"Câu này có phục vụ hạt nhân cảm xúc không?"* Nếu không — cắt.

---

## KT3: MIRROR DRAFT — Viết Song Song Rồi Ghép

**Tại sao:** Nhiều góc nhìn tạo chiều sâu mà một góc đơn lẻ không đạt được.

**Step-by-step:**
1. Viết góc nhìn A (nhân vật chính)
2. Cùng phiên: *"Viết lại cùng sự kiện từ góc nhìn B. KHÔNG lặp hình ảnh bản trước."*
3. Tuỳ chọn: góc nhìn C (đồ vật, người ngoài cuộc)
4. BẠN đọc tất cả, chọn dòng hay nhất mỗi bản, ghép master

**Constraint:** *"Không lặp hình ảnh"* — buộc AI tìm góc mới thực sự.

---

## KT4: DNA SAMPLE — Cho AI Nuốt Mẫu Giọng Văn

**Tại sao:** AI học từ ví dụ cụ thể gấp 10 lần so với mô tả trừu tượng.

**Step-by-step:**
1. Chọn 300-1000 từ prose hay nhất
2. Paste đầu prompt KÈM tag giải thích
3. Chỉ dẫn: *"Đây là DNA giọng văn. Mọi thứ sau đây duy trì tần số này."*

**Ví dụ tag:**
```
DNA giọng văn. Chú ý:
- Câu mở đoạn luôn dưới 7 từ
- Em-dash tạo khoảng lặng giữa hành động
- Ẩn dụ chỉ từ hệ [thực vật / kim loại / nước]
- Mô tả đau: xúc giác trước, thị giác sau
- Khoảng trắng giữa đoạn = nhân vật nghĩ nhưng không nói
```

---

## KT5: ADVERSARIAL EDITING — AI Tự Đánh AI

**Tại sao:** AI tự hài lòng. Vai "biên tập tàn nhẫn" tìm lỗi mà vai "đồng tác giả" bỏ qua.

**Prompt:**
```
Quên vai đồng tác giả. Hãy là biên tập viên tàn nhẫn nhất.
(1) Câu nào TELL thay vì SHOW? Chỉ cụ thể.
(2) Từ nào lặp trong bán kính 3 câu?
(3) Đường cong cảm xúc flat ở giữa?
(4) Câu kết ám ảnh hay "kết an toàn"?
(5) Cắt đoạn này — người đọc mất gì? Nếu không → thừa.
```

**⚠️ BẪY:** Không cho checklist → feedback chung chung vô dụng. **LUÔN cho checklist.**

---

## KT6: EMOTIONAL MAPPING — Bản Đồ Cảm Xúc

**Tại sao:** AI viết tốt hơn khi biết ĐÍCH CẢM XÚC. Toàn đỉnh cao → tê liệt. Cần thung lũng.

**3 sóng chồng nhau:**
- **Sóng lớn:** Arc chương (mở → cao trào → kết)
- **Sóng vừa:** Tension scene (câu hỏi → trả lời → câu hỏi mới)
- **Sóng nhỏ:** Nhịp câu (nhanh → chậm → nhanh)

Ba tần số phải cộng hưởng. Đảm bảo có **moment of stillness** (50-100 từ yên tĩnh) giữa các đỉnh.

---

## KT7: CONSTRAINT BREEDING — Giới Hạn Sinh Sáng Tạo

**Tại sao:** AI viết hay hơn khi bị giới hạn NHIỀU hơn. Sonnets hay VÌ có 14 dòng, không phải DÙ có.

**Ví dụ:**
```
PHẢI:
- Mọi hành động mô tả qua âm thanh và xúc giác
- Câu cao trào dưới 10 từ
- 1 đồ vật bình thường mang ý nghĩa biểu tượng

CẤM:
- Từ "mạnh mẽ", "kinh hoàng", "ghê gớm"
- Câu hỏi tu từ
- Ẩn dụ về biển hoặc bầu trời
```

---

## KT8: GHOST READER — Đọc Như Độc Giả Lần Đầu

**Prompt:**
```
Quên mọi thứ về cốt truyện. Đọc đoạn này như người chưa biết gì.
(1) 3 câu hỏi tự nhiên trong đầu người đọc
(2) Chỗ nào có thể chán và bỏ đọc
(3) Hình ảnh nào ám ảnh sau khi gấp sách
```

---

## KT9: NEGATIVE SPACE — Viết Bằng Cái KHÔNG Viết

**Cách áp dụng:**
- Nhân vật im lặng giữa hội thoại
- Scene kết giữa chừng
- Trang trống, câu bị cắt ngang, `...` kéo dài một dòng

**Nguyên tắc:** Format chính là nội dung. Khoảng trắng kể chuyện. Người đọc tự điền → ám ảnh hơn.

---

## KT10: RESONANCE LINKING — Echo Xuyên Suốt

**Cách làm:**
1. Chọn 5-7 motif lặp lại xuyên suốt
2. MỖI LẦN xuất hiện, ý nghĩa phải ĐỔI

**Ví dụ — "bàn tay nắm chặt":**
- Lần 1: sợ (trẻ con lạc đường)
- Lần 2: giận (trưởng thành, bị phản bội)
- Lần 3: buông (nắm tay người sắp chết)

Cùng hành động, 3 nghĩa — lần 3 đau gấp ngàn lần vì tích luỹ.

**Prompt:**
```
Scene này phải có [motif] xuất hiện ít nhất 1 lần,
nhưng ý nghĩa KHÁC các lần trước.
Các lần trước: [liệt kê]
```

---

## KT11: TEMPO SCRIPTING — Nhịp Trước, Chữ Sau

**Cách làm:**
1. Viết bản nhịp — chỉ nhịp, không nội dung:
```
Chậm — chậm — NHANH — nhanh — IM LẶNG — chậm — NHANH NHẤT — thì thầm.
```

2. Quy tắc:
```
NHANH = câu dưới 8 từ, không dấu phẩy
Chậm = 20-30 từ, nhiều mệnh đề
IM LẶNG = dòng trống hoặc "..."
Thì thầm = câu ngắn, 1 hình ảnh duy nhất
```

---

## KT12: 2-PASS WRITING — Viết Thô Rồi Đập Văn

**Pass 1 — Viết thô:**
```
Viết nhanh, thẳng, không trau chuốt.
Ưu tiên hành động + quyết định + xung đột. Đừng cố đẹp.
```

**Pass 2 — Đập văn:**
```
Giữ nguyên sự kiện. Nâng nhịp câu.
Tăng hình ảnh giác quan. Giảm giải thích 40%.
Thêm 3 chi tiết lạ mà đúng.
```

---

## Bảng Tra: Kỹ Thuật Theo Giai Đoạn

| Giai đoạn | Chính | Hỗ trợ |
|-----------|-------|--------|
| **Chuẩn bị** | KT4, KT6 | KT10, KT11, KT7 |
| **Viết** | KT1, KT2, KT12 | KT7, KT9 |
| **Biên tập** | KT5, KT8 | KT3 |
| **Kiểm tra** | Cross-check, Council | KT10 |

---

## Kết Hợp KT Với Kỹ Thuật Văn Học

| KT | Kỹ thuật văn học phù hợp |
|----|-------------------------|
| KT1 | Register switching (#43), Tone & Mood (116-125) |
| KT2 | Câu cụt (#29), Telling detail, Minimalism |
| KT4 | Prose rhythm (106-115), Imagery systems (126-135) |
| KT7 | Bất kỳ kỹ thuật nào làm PHẢI hoặc CẤM |
| KT9 | Khoảng lặng (#25), Silence (#50), Fragment |
| KT10 | Motif (#53), Leitmotif (#54), Echo (#56), Callback (#69) |
| KT11 | Câu ngắn/dài (#26-29), Polysyndeton/Asyndeton (#36-37) |
| KT12 | Pass 1: Động từ mạnh (#42), Asyndeton. Pass 2: Imagery, Euphony |

---

*Quay lại: [SKILL.md](../SKILL.md) · Xem thêm: [prompts.md](prompts.md) · [forge-workflow.md](forge-workflow.md)*
