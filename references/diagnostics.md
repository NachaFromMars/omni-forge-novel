# Chẩn Đoán & Sửa Lỗi — Chi Tiết

> 10 bệnh thường gặp + bệnh nâng cao. Mỗi bệnh: triệu chứng, nguyên nhân, thuốc, prompt sửa.

---

## 10 Bệnh Thường Gặp

### 1. AI Padding

**Triệu chứng:** Viết dài nhưng rỗng, lặp ý, câu filler không mang thông tin mới, cắt đi không mất gì.

**Nguyên nhân:** AI train để viết dài → không có constraint thì thêm từ cho đủ.

**Thuốc:** KT2 Chain of Density — nén trước rồi nở. Sau mỗi lần nở: *"Câu này phục vụ hạt nhân cảm xúc không?"* Nếu không → cắt.

**Prompt sửa:**
```
Đọc lại đoạn này. Cắt mọi câu mà nếu bỏ đi, người đọc không mất
thông tin hay cảm xúc nào. Mục tiêu: giảm 30% số từ, giữ nguyên impact.
```

---

### 2. Giọng Phèn

**Triệu chứng:** Bóng bẩy nhưng rỗng, "mùi AI", nhiều tính từ kép, ẩn dụ hoa mỹ rỗng.

**Nguyên nhân:** AI mặc định viết "hay" bề mặt — nhiều trang sức, thiếu cốt.

**Thuốc:** KT4 DNA Sample — 500 từ prose mẫu cụ thể kèm tag giải thích.

**Prompt sửa:**
```
[PASTE DNA 300 TỪ MẪU]
Viết lại đoạn dưới đây giữ đúng tần số DNA trên.
Cắt mọi tính từ kép. Cắt mọi ẩn dụ không có xương sống.
[PASTE ĐOẠN CẦN SỬA]
```

---

### 3. Tell Don't Show

**Triệu chứng:** "Anh ta rất buồn", "Cô ấy sợ hãi" — giải thích cảm xúc trực tiếp.

**Nguyên nhân:** Tell dễ hơn Show. AI chọn đường ngắn nhất.

**Thuốc:** KT7 Constraint — CẤM từ chỉ cảm xúc trực tiếp. Buộc AI tả qua hành vi, chi tiết cơ thể, đồ vật.

**Prompt sửa:**
```
Chỉ ra 7 câu TELL trong đoạn dưới. Thay mỗi câu bằng
hành vi/chi tiết cơ thể/đồ vật cho thấy cùng cảm xúc.
CẤM: buồn, vui, giận, sợ, yêu, ghét, lo lắng, hạnh phúc.
[PASTE ĐOẠN]
```

---

### 4. Giọng Trôi

**Triệu chứng:** Chương 5 giọng khác chương 1. Mỗi phiên mới, AI "quên" tần số.

**Nguyên nhân:** AI không nhớ xuyên phiên.

**Thuốc:** Voice Kit — paste DNA mẫu đầu MỖI phiên viết mới.

---

### 5. Flat Emotion

**Triệu chứng:** Cường độ đều từ đầu đến cuối, không đỉnh/thung lũng, người đọc tê liệt.

**Nguyên nhân:** AI không biết vị trí → viết mọi chương cùng cường độ.

**Thuốc:** KT6 Emotional Mapping — vẽ đường cong trước khi viết. Đảm bảo moment of stillness giữa các đỉnh.

---

### 6. Cliché Tràn Lan

**Triệu chứng:** Ẩn dụ quen (biển, trời, vực), cấu trúc đoán được, twist không twist.

**Nguyên nhân:** AI dùng pattern phổ biến nhất trong training data.

**Thuốc:** KT7 Constraint — CẤM ẩn dụ quen cụ thể. Lệnh `REVERSE`. Đổi hệ ẩn dụ: cơ khí, y khoa, côn trùng, kiến trúc.

---

### 7. Nhân Vật Phẳng

**Triệu chứng:** Một chiều, không mâu thuẫn, pure good/evil, đoán trước được.

**Nguyên nhân:** AI tạo nhân vật "sạch" nếu không yêu cầu phức tạp.

**Thuốc:** `DEEPER` — mỗi nhân vật: 1 vết thương, 1 khao khát ẩn, 1 bí mật, 1 mâu thuẫn nội tại.

---

### 8. Lore Dump

**Triệu chứng:** Đoạn dài giải thích worldbuilding, info dump, "như bạn biết..." exposition.

**Nguyên nhân:** AI giải thích thay vì cho thấy.

**Thuốc:** Mọi lore qua hành động/đối thoại. Giải thích > 2 câu liên tiếp = dump. CẤM.

---

### 9. Nhịp Đều

**Triệu chứng:** Mọi đoạn cùng nhịp, cùng độ dài câu, đọc như báo cáo.

**Nguyên nhân:** AI mặc định viết 1 register nhất quán.

**Thuốc:** KT11 Tempo Scripting — bản nhịp TRƯỚC khi viết prose.

---

### 10. Mâu Thuẫn Logic

**Triệu chứng:** Chi tiết chương sau trái trước, nhân vật hành xử không nhất quán, timeline sai.

**Nguyên nhân:** AI không nhớ nội dung chương trước trong phiên mới.

**Thuốc:** FORGE+C bước C (Cross-check) + `COUNCIL`.

---

## Bệnh Nâng Cao

### GHOST VOICE (Giọng Ma AI)

**Triệu chứng:** Giọng nịnh — ca ngợi quá mức. *"Brilliant"*, *"stunning"*. Văn sạch nhưng vô hồn.

**Thuốc:** Humanize Pass trong bước G. Quét từ vựng AI + thêm personality, opinion, specific detail.

---

### MIRROR CHARACTER (Nhân Vật Gương)

**Triệu chứng:** Nhân vật phụ clone tính cách nhân vật chính. Thoại giống nhau.

**Thuốc:** Character Sheet riêng cho mỗi nhân vật. 3 câu thoại mẫu phải KHÁC BIỆT. Che tên → test phân biệt.

---

### SYMBOLISM PHỒNG

**Triệu chứng:** Ẩn dụ quá rõ ràng. AI giải thích ý nghĩa biểu tượng thay vì gợi.

**Thuốc:** CẤM giải thích ẩn dụ. Để người đọc tự tìm. *"Đặt biểu tượng — ĐỪNG giải thích nó."*

---

### EM DASH SPAM

**Triệu chứng:** Quá nhiều dấu — trong 1 đoạn. Mỗi câu đều có em-dash.

**Thuốc:** Giới hạn tối đa 2 em-dash / đoạn. Thay bằng dấu phẩy, chấm, hoặc câu mới.

---

### STRUCTURE LOOP

**Triệu chứng:** Mở đầu nhiều đoạn giống nhau. Cùng pattern: [Nhân vật] + [hành động] + [cảm xúc].

**Thuốc:** Vary câu mở: câu dài → cụt → hình ảnh → thoại → khoảng lặng.

---

### OVER-EXPLAINING

**Triệu chứng:** Giải thích cái người đọc đã hiểu. Nhắc lại context không cần thiết.

**Thuốc:** Cắt mọi giải thích thừa. Tin người đọc thông minh hơn bạn nghĩ. *"Nếu người đọc đã biết — đừng nói."*

---

## Bảng Tra Nhanh Tổng Hợp

| Bệnh | Thuốc nhanh | Lệnh tắt |
|------|-------------|-----------|
| Padding | Chain of Density | — |
| Giọng phèn | DNA Sample 500 từ | `VIẾT` |
| Tell don't Show | CẤM từ cảm xúc | `SENSORY` |
| Giọng trôi | Voice Kit đầu phiên | — |
| Flat emotion | Emotional Map | `EMOTION` |
| Cliché | CẤM ẩn dụ quen | `REVERSE` |
| Nhân vật phẳng | Wound + secret | `DEEPER` |
| Lore dump | Lore qua action/thoại | — |
| Nhịp đều | Tempo Script | — |
| Mâu thuẫn | Cross-check + Council | `COUNCIL` |
| Ghost Voice | Humanize Pass | — |
| Mirror Character | Character Sheet riêng | `DIALOGUE` |
| Symbolism phồng | CẤM giải thích symbol | — |
| Em dash spam | Max 2/đoạn | — |
| Structure loop | Vary câu mở | — |
| Over-explaining | Cắt giải thích thừa | — |

---

*Quay lại: [SKILL.md](../SKILL.md) · Xem thêm: [techniques.md](techniques.md)*
