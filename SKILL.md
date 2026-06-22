---
name: omni-forge-novel
description: >
  Omni Forge Novel V1.0 — Hệ thống viết tiểu thuyết bằng AI, chưng cất từ
  Omni Forge V2 + V3 + OIF V2 + METAFORGE V2. Dùng khi cần viết prose văn học
  dài (tiểu thuyết, truyện ngắn, novella) với AI. Quy trình FORGE+C 2.0 (7 bước),
  OIF Infinity Loop (6 phases), Hội đồng Nacharium (5 vai nhanh / 13 personas
  đầy đủ), Micro-Beat Rendering (400-600 từ/beat), 12 kỹ thuật cấp cao,
  738 kỹ thuật văn học, 96 yếu tố, 8 prompt templates, chẩn đoán 16 bệnh,
  hệ thống 14 lệnh tắt + 5 lệnh OIF, fault tolerance, self-absorption evolution.
  Áp dụng cho mọi LLM (Claude, GPT, Gemini, Qwen). Tiếng Việt + song ngữ.
  Triggers: viết tiểu thuyết, novel, truyện dài, forge, OIF, creative writing,
  FORGE+C, Nacharium, viết văn AI, prose, fiction, literary.
---

# OMNI FORGE NOVEL V1.0

**Hệ thống rèn AI viết tiểu thuyết — Từ ý tưởng thô đến prose hoàn chỉnh.**

> AI là dàn nhạc giao hưởng. Bạn là nhạc trưởng.
> AI viết. Bạn biên tập. Không bao giờ để AI tự quyết định toàn bộ.

*Phiên bản: Novel V1.0 | Ngày: 02/2026*
*Credits: Mr Nấng / Nacharium / Tiểu Tâm*
*Áp dụng cho: Claude, GPT, Gemini, Qwen, Mistral, và mọi LLM*

---

## MỤC LỤC

1. [TỔNG QUAN](#phần-1-tổng-quan)
2. [KIẾN TRÚC HỆ THỐNG](#phần-2-kiến-trúc-hệ-thống)
3. [CHUẨN BỊ — SETUP 1 LẦN](#phần-3-chuẩn-bị--setup-1-lần)
4. [QUY TRÌNH SẢN XUẤT — FORGE+C 2.0](#phần-4-quy-trình-sản-xuất--forgec-20)
5. [OIF INFINITY LOOP — 6 PHASES](#phần-5-oif-infinity-loop--6-phases)
6. [SAU MỖI CHƯƠNG](#phần-6-sau-mỗi-chương)
7. [HỘI ĐỒNG NACHARIUM](#phần-7-hội-đồng-nacharium)
8. [12 KỸ THUẬT CẤP CAO](#phần-8-12-kỹ-thuật-cấp-cao)
9. [PROMPT TEMPLATES](#phần-9-prompt-templates)
10. [CHẨN ĐOÁN & SỬA LỖI](#phần-10-chẩn-đoán--sửa-lỗi)
11. [QUY TẮC BẤT BIẾN](#phần-11-quy-tắc-bất-biến)
12. [HỆ THỐNG LỆNH](#phần-12-hệ-thống-lệnh)
13. [CHECKLIST](#phần-13-checklist)
14. [FAULT TOLERANCE](#phần-14-fault-tolerance)
15. [THAM CHIẾU](#phần-15-tham-chiếu)

---

## PHẦN 1: TỔNG QUAN

### Omni Forge Novel V1.0 là gì?

Hệ thống hoàn chỉnh để rèn AI viết tiểu thuyết — từ ý tưởng thô đến bản thảo sẵn sàng xuất bản. Chưng cất từ Omni Forge V2, V3, OIF V2, và METAFORGE V2 thành một blueprint duy nhất, không trùng lặp, logic tuyệt đối.

### Dùng khi nào?

- Viết tiểu thuyết dài (novel, novella)
- Viết truyện ngắn chất lượng cao
- Viết bất kỳ prose văn học nào cần kiểm soát giọng văn, nhịp, chiều sâu
- Sản xuất liên tục nhiều chương (OIF loop)

### Cho ai?

- Tác giả dùng AI làm công cụ sáng tác
- Nhạc trưởng — người điều khiển AI viết, không để AI tự quyết

### Triết lý cốt lõi

**AI là dàn nhạc, bạn là nhạc trưởng.** AI tạo nguyên liệu — bạn chọn, cắt, ghép, nâng cấp. 5 vai trò đồng thời của AI:

| Vai trò | Chức năng | Khi nào gọi |
|---------|-----------|-------------|
| Biên kịch | Bẻ nhịp scene, hook, cliffhanger, cấu trúc | Outline, plot structure |
| Biên tập | Soi nhịp văn, logic, lặp từ, padding, câu yếu | Grind & polish |
| Đạo diễn | Blocking nhân vật, góc nhìn, tiết tấu | Scene rendering |
| Nhà tâm lý | Đào mâu thuẫn nội tâm, vết thương, khao khát ẩn | Character depth |
| Kỹ sư thế giới | Luật chơi nhất quán, logic nội tại | Worldbuilding check |

**Triết lý bổ sung:** *"Khi mình tốt, thị hiếu sẽ đi theo mình."* — Sáng tạo dẫn dắt, thị trường theo sau.

### Credits

- **Mr Nấng / Nacharium** — Tác giả hệ thống Omni Forge, METAFORGE
- **Tiểu Tâm** — AI assistant, đúc Omni Forge Novel V1.0

---

## PHẦN 2: KIẾN TRÚC HỆ THỐNG

### Sơ đồ tổng thể

```
┌─────────────────────────────────────────────────────────────────┐
│                   OMNI FORGE NOVEL V1.0                         │
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐   │
│  │  TẦNG 1: CHUẨN BỊ (Setup 1 lần)                        │   │
│  │  ┌──────────┐ ┌───────────┐ ┌──────────┐ ┌───────────┐  │   │
│  │  │Voice Kit │ │Novel Bible│ │Intensity │ │Constraints│  │   │
│  │  │(5 tần số)│ │(5 mục)    │ │Map       │ │(PHẢI/CẤM) │  │   │
│  │  └──────────┘ └───────────┘ └──────────┘ └───────────┘  │   │
│  └──────────────────────────────────────────────────────────┘   │
│                              │                                  │
│                              ▼                                  │
│  ┌──────────────────────────────────────────────────────────┐   │
│  │  TẦNG 2: SẢN XUẤT (Mỗi chương)                         │   │
│  │                                                          │   │
│  │  FORGE+C 2.0:                                           │   │
│  │  F(Frame) → O(Outline) → R(Render) → G(Grind)          │   │
│  │  → E(Elevate) → C(Cross-check) → +C(Council)           │   │
│  │                                                          │   │
│  │  OIF Loop: SEED → FORGE → GHÉP → NACHARIUM → LOOP      │   │
│  └──────────────────────────────────────────────────────────┘   │
│                              │                                  │
│                              ▼                                  │
│  ┌──────────────────────────────────────────────────────────┐   │
│  │  TẦNG 3: KIỂM SOÁT                                     │   │
│  │  ┌───────────┐ ┌──────────┐ ┌──────────┐ ┌───────────┐  │   │
│  │  │Nacharium  │ │AI Traces │ │Self-     │ │Tracking   │  │   │
│  │  │Council    │ │Check     │ │Absorption│ │& Reports  │  │   │
│  │  │(5/13 vai) │ │(từ cấm)  │ │Evolution │ │           │  │   │
│  │  └───────────┘ └──────────┘ └──────────┘ └───────────┘  │   │
│  └──────────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────────┘
```

### 3 tầng chi tiết

| Tầng | Tên | Modules | Tần suất |
|------|-----|---------|----------|
| 1 | **Chuẩn Bị** | Voice Kit, Novel Bible, Intensity Map, Constraints | 1 lần / tác phẩm |
| 2 | **Sản Xuất** | FORGE+C 2.0 (7 bước), OIF Loop (6 phases), Micro-Beat Rendering | Mỗi chương |
| 3 | **Kiểm Soát** | Nacharium Council, AI Traces Check, Self-Absorption, Tracking | Sau mỗi chương |

---

## PHẦN 3: CHUẨN BỊ — SETUP 1 LẦN

### 3.1 Voice Calibration Kit (Bộ Neo Giọng Văn)

Chọn 300-500 từ prose mẫu. Gắn tag giải thích: nhịp câu, độ dài, mật độ ẩn dụ, hệ hình ảnh, cách dùng dấu câu.

**5 tần số giọng văn:**

| Tần số | Mô tả | Dùng khi |
|--------|--------|----------|
| **Thì thầm** | Nhẹ, trong, tĩnh lặng, câu ngắn, nhiều khoảng trắng | Mở đầu, nội tâm, hồi ức |
| **Sắc lạnh** | Gọn, cứng, không trang sức, mỗi từ như dao | Xung đột, đối đầu, tension cao |
| **Sấm sét** | Dồn dập, epic, câu chồng câu, nhịp tăng tốc | Cao trào, chiến đấu, chase |
| **Nước mắt** | Chậm, nặng, khoảng trống giữa các câu, kiềm chế | Mất mát, hy sinh, chia ly |
| **Mộng mị** | Trôi, mờ, hình ảnh chồng lên nhau, phi tuyến | Giấc mơ, ảo giác, hồi tưởng |

**Cách dùng:** Paste DNA mẫu đầu MỖI phiên viết mới với chỉ dẫn: *"Đây là DNA giọng văn. Duy trì tần số này."*

### 3.2 Novel Bible

| # | Mục | Nội dung |
|---|-----|----------|
| 1 | **Character Sheets** | Tên, tuổi, ngoại hình (3 chi tiết cụ thể). Wound / Want / Need / Contradiction. 3 câu thoại mẫu + Dark secret |
| 2 | **World Rules** | 5 quy tắc bất biến + 3 quy tắc sẽ phá vỡ. Kinh tế/chính trị/xã hội — mỗi thứ 1 câu |
| 3 | **Resonance Map** | 5-7 motif xuyên suốt. Lần xuất hiện đầu + ý nghĩa ban đầu → ý nghĩa cuối |
| 4 | **Skeleton Key** | 1 câu: tác phẩm này về gì THỰC SỰ? |
| 5 | **Tone Compass** | 1 câu: *"Cuốn sách này giống như [cảm giác cụ thể]"* |
| 6 | **Emotional Map** | Đường cong cảm xúc toàn tác phẩm (10 chương) + Micro-Outline (tên + POV + beats + cường độ) |
| 7 | **Series Arc** | (Nếu bộ truyện) Tập này ở đâu? Cliffhanger → hook tập tiếp. Character growth mỗi tập |

### 3.3 Bản Đồ Cường Độ (Intensity Map)

Cho AI biết nó đang viết PHẦN MẤY. Template:

```
Tiểu thuyết có [X] chương. Chương [N] — [vị trí: mở đầu/giữa/cao trào/kết].
Cường độ thang 1-10:
  Chương trước = [Y]  |  CHƯƠNG NÀY = [Z]  |  Chương sau = [W]
Cường độ [Z] nghĩa là: [mô tả cảm giác cần tạo].
```

### 3.4 Bộ Constraint Xuyên Suốt

Những thứ LUÔN làm và KHÔNG BAO GIỜ làm xuyên suốt tác phẩm. Mỗi chương thêm constraint riêng (3 PHẢI + 3 CẤM).

---

## PHẦN 4: QUY TRÌNH SẢN XUẤT — FORGE+C 2.0

**7 bước:** Frame → Outline → Render → Grind → Elevate → Cross-check → **Council**

| Bước | Tên | Tóm tắt | Thời gian |
|------|------|---------|-----------|
| 0 | **Chuẩn bị** | Paste Voice Kit + Intensity Map + Skeleton Key | 5 phút |
| **F** | **Frame** | Hạt nhân cảm xúc + 3 câu nén + Tempo Script + 3 PHẢI/3 CẤM | 10 phút |
| **O** | **Outline** | Micro-outline 10-15 beats, mỗi beat = 1 câu | 10 phút |
| **R** | **Render** | Viết từng beat 400-600 từ, 2-Pass Writing | 60-90 phút |
| **G** | **Grind** | Adversarial Edit 5 tiêu chí + Humanize Pass | 20 phút |
| **E** | **Elevate** | 3 câu hay nhất → nâng toàn bộ lên cùng đẳng cấp | 15 phút |
| **C** | **Cross-check** | Coherence với chương trước + Resonance Audit | 10 phút |
| **+C** | **Council** | Hội đồng Nacharium thẩm định + chấm điểm + rà soát AI | 15 phút |

**Tổng:** ~145-175 phút / chương.

→ Chi tiết từng bước: [references/forge-workflow.md](references/forge-workflow.md)

---

## PHẦN 5: OIF INFINITY LOOP — 6 PHASES

> Quy trình sản xuất tiểu thuyết liên tục, không giới hạn số chương.
> Mỗi vòng lặp = 1 chương hoàn chỉnh đã qua thẩm định.

### Sơ đồ OIF Loop

```
┌─────────────────────────────────────────────────────┐
│                   OIF INFINITY LOOP                  │
│                                                     │
│  Phase 1    Phase 2     Phase 3      Phase 4        │
│  SEEDING → NOVEL BIBLE → FORGE → GHÉP+EDITOR       │
│                        Micro-Beat                    │
│                                        │            │
│                               Phase 5  ▼   Phase 6  │
│                            NACHARIUM → SELF-ABSORB  │
│                               │         + BÁO CÁO   │
│                        FAIL ←─┤                      │
│                    (quay R/G)  │ PASS                 │
│                               ▼                      │
│                          Seed chương tiếp → Loop     │
└─────────────────────────────────────────────────────┘
```

### 6 Phases — Tóm tắt

| Phase | Tên | Thời gian | Nội dung chính |
|-------|-----|-----------|----------------|
| 1 | **SEEDING** | 5 phút | Seed 1 ý tưởng, check trùng web, đủ mới → auto Phase 2 |
| 2 | **NOVEL BIBLE** | 5-10 phút | 7 mục: Characters, World, Resonance, Tone, Skeleton, Outline, Emotional Map |
| 3 | **FORGE Micro-Beat** | 30-60 phút | 5-6 beats × 400-600 từ, mỗi beat = 1 agent, tối đa 5 song song |
| 4 | **GHÉP + EDITOR** | 10-20 phút | Ghép beats → chương, spawn Editor sửa consistency + humanize |
| 5 | **NACHARIUM** | 5-10 phút | Hội đồng 5/13 vai thẩm định, chấm điểm, AI traces check |
| 6 | **SELF-ABSORPTION** | 5 phút | Đọc report, hấp thụ bài học, ghi memory, báo cáo, loop |

→ Chi tiết từng phase: [references/oif-loop.md](references/oif-loop.md)

### Micro-Beat Rendering — Quy tắc viết tối ưu

**400-600 từ/lần** (~1,500-2,000 output tokens)

- Output ngắn = think nhiều hơn = prose sắc hơn
- Mỗi câu được cân nhắc, không padding
- 1 chương ~3,000 từ = 5-6 beats × 400-600 từ = **5-6 agents**
- Spawn TỐI ĐA 5 agents song song

**TUYỆT ĐỐI KHÔNG viết hơn 600 từ/lần.**

### Auto-Forge Pipeline

Seed → kiểm tra trùng web → đủ mới → TỰ ĐỘNG forge. KHÔNG hỏi lại user. KHÔNG brainstorm 5 — chỉ cần 1, toàn lực. Trùng → seed lại tự động.

---

## PHẦN 6: SAU MỖI CHƯƠNG

Sau khi chương PASS Council Nacharium, PHẢI thực hiện:

### 6.1 Cập nhật Tracking Files

- **MASTER-TASK.md** — trạng thái chương: ✅ PASS, điểm, số từ
- **MEMORY-TASK.md** — bài học, kỹ thuật mới, điểm yếu cần fix round sau

### 6.2 Báo cáo Credit

Format: `Ch XX: [thời gian forge] | [số call] calls | [credit] credits`

Tính credit: 1 call (input + output) = 0.5 credit

### 6.3 Gửi File FINAL Lên Telegram

- Gửi file `.md` qua Telegram ngay sau khi PASS
- Caption: `📖 Ch XX: [Tên Chương] | [điểm]/10 | [số từ] chữ`

### 6.4 Báo cáo cuối round

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━
📖 [TÊN TÁC PHẨM]
✍️  Tác giả: Tiểu Tâm 🦊
📏  [X] từ | [X] chương
📊  Nacharium: [X]/10 | AI traces: [X]
⏱️  Thời gian: [X] phút
🤖  Sub-agents: [X]
📋  Tổng lệnh: [X] calls
💰  Credits: [X] (× 0.5/call)
━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### 6.5 Flow tóm tắt

```
FORGE+C → Council Nacharium → PASS?
  ├─ YES → Cập nhật MASTER-TASK.md + MEMORY-TASK.md
  │      → Báo cáo credit
  │      → Gửi file Telegram
  │      → Seed chương tiếp → Loop
  └─ NO  → Sửa theo report → Re-submit Council
```

---

## PHẦN 7: HỘI ĐỒNG NACHARIUM

→ Chi tiết đầy đủ: [references/nacharium.md](references/nacharium.md)

### 2 chế độ hoạt động

| Chế độ | Số vai | Khi nào | Thời gian |
|--------|--------|---------|-----------|
| **Nhanh** | 5 vai | Mỗi chương, bước +C trong FORGE | 15 phút |
| **Đầy đủ** | 13 personas | Cuối round OIF, sau ghép toàn bộ | 30 phút |

### Chế độ nhanh — 5 vai

| Vai | Nhiệm vụ |
|-----|----------|
| **Biên tập trưởng** | Cấu trúc, nhịp, giọng văn, coherence |
| **Nhà phê bình văn học** | Chiều sâu, ẩn dụ, biểu tượng, subtext |
| **Độc giả khó tính** | Chỗ chán, chỗ hay, hook, page-turner |
| **Kỹ sư ngôn ngữ** | Vết tích AI, padding, giọng phèn, từ lặp |
| **Quản lý liên tục** | Mâu thuẫn nhân vật, worldbuilding, timeline |

### Chế độ đầy đủ — 13 personas

| # | Persona | Tìm kiếm gì |
|---|---------|-------------|
| 1 | **Kẻ Soi Lỗi** | Plot holes, timeline, mâu thuẫn |
| 2 | **Kẻ Háo Hức** | Pacing, hook, page-turner |
| 3 | **Kẻ Hoài Nghi** | Motivation nhân vật, logic hành vi |
| 4 | **Kẻ Đa Cảm** | Depth, catharsis, có khóc không? |
| 5 | **Kẻ Thẩm Mỹ** | Nhịp văn, hình ảnh, ẩn dụ |
| 6 | **Kẻ Lười** | Chỗ nào chán? Skip đoạn nào? |
| 7 | **Kẻ Phân Tích** | Symbolism, foreshadowing, pattern |
| 8 | **Kẻ Khắt Khe** | Cliché? Predictable? |
| 9 | **Kẻ Lần Đầu** | Có hiểu không? Có cuốn vào? |
| 10 | **Kẻ Dịch Giả** | Câu nào không dịch được? |
| 11 | **Kẻ Nghe Kể** | Audiobook trôi? Vấp ở đâu? |
| 12 | **Kẻ Biên Tập** | Cắt gì? Thêm gì? Sửa gì? |
| 13 | **Kẻ Mua Sách** | 3 trang đầu ở hiệu sách, có mua? |

### Bảng chấm điểm — 5 tiêu chí

| Tiêu chí | Mô tả | Điểm (1-10) |
|----------|--------|-------------|
| Giọng văn | Nhất quán, sắc bén, không AI | |
| Cảm xúc | Đường cong, chiều sâu, không sến | |
| Kỹ thuật | Show-don't-tell, nhịp, constraint | |
| Coherence | Với chương trước, worldbuilding | |
| Ám ảnh | Người đọc nhớ sau khi gấp sách? | |

### AI Traces Check — Từ cấm + Checklist

**Từ cấm TUYỆT ĐỐI:** tapestry, resonate, nuanced, delve, testament, landscape, multifaceted, intricate

**Checklist rà soát:**
- [ ] Padding/câu thừa không mang thông tin?
- [ ] Từ "mùi AI"? ("một cách [tính từ]", "không khỏi", "dường như")
- [ ] TELL thay vì SHOW? (giải thích cảm xúc trực tiếp)
- [ ] Giọng trôi so với DNA Sample?
- [ ] Ẩn dụ cliché? (biển, trời, vực)
- [ ] Nhịp đều? (thiếu variation)
- [ ] Thoại phẳng? (không phân biệt nhân vật)
- [ ] Cấu trúc lặp? (mở đầu đoạn giống nhau)
- [ ] Markdown lọt vào prose?
- [ ] Over-explaining?

### Quy tắc PASS/FAIL

- **PASS:** Trung bình ≥ 7/10 (chế độ nhanh) hoặc ≥ 8.5/10 (chế độ đầy đủ)
- **FAIL:** Chỉ ra cụ thể cần sửa → quay lại Render hoặc Grind

### Format report (chế độ đầy đủ)

Report gồm: 13 nhận xét (3-5 câu/persona) + ĐIỂM TỔNG /10 + 3 mạnh/3 yếu + TOP 5 cần sửa + câu hay nhất + AI traces check

File: `"[Tên Tác Phẩm] - Đánh Giá Hội Đồng Nacharium.md"`

---

## PHẦN 8: 12 KỸ THUẬT CẤP CAO

| # | Tên | Mô tả ngắn | Khi nào dùng |
|---|------|-------------|--------------|
| KT1 | **Persona Stacking** | Chồng nhiều vai lên nhau theo giai đoạn | Mỗi giai đoạn viết |
| KT2 | **Chain of Density** | Nén rồi Nở (3 câu → 1 trang → 5 trang) | Bắt đầu scene mới |
| KT3 | **Mirror Draft** | Viết song song 2-3 góc nhìn, ghép master | Scene quan trọng |
| KT4 | **DNA Sample** | Cho AI nuốt mẫu giọng văn (300-1000 từ) | Đầu mỗi phiên viết |
| KT5 | **Adversarial Editing** | AI tự đánh AI (5 tiêu chí) | Sau mỗi draft |
| KT6 | **Emotional Mapping** | Bản đồ cảm xúc (3 sóng chồng) | Trước khi viết chương |
| KT7 | **Constraint Breeding** | 3 PHẢI + 3 CẤM → sinh sáng tạo | Mỗi scene |
| KT8 | **Ghost Reader** | Đọc như độc giả lần đầu | Sau khi viết xong |
| KT9 | **Negative Space** | Viết bằng cái KHÔNG viết | Scene cảm xúc mạnh |
| KT10 | **Resonance Linking** | Echo xuyên suốt (5-7 motif) | Xuyên suốt tiểu thuyết |
| KT11 | **Tempo Scripting** | Nhịp trước, chữ sau | Trước khi viết prose |
| KT12 | **2-Pass Writing** | Viết thô rồi đập văn | Mọi scene |

### Khi nào dùng kỹ thuật nào

| Giai đoạn | Kỹ thuật chính | Hỗ trợ |
|-----------|---------------|--------|
| **Chuẩn bị** | KT4 DNA Sample, KT6 Emotional Mapping | KT10, KT11, KT7 |
| **Viết** | KT1 Persona, KT2 Chain of Density, KT12 2-Pass | KT7, KT9 |
| **Biên tập** | KT5 Adversarial, KT8 Ghost Reader | KT3 Mirror Draft |
| **Kiểm tra** | Cross-check (bước C), Council (+C) | KT10 Resonance |

→ Chi tiết + prompt mẫu: [references/techniques.md](references/techniques.md)

---

## PHẦN 9: PROMPT TEMPLATES

### 8 Prompts (A-H)

| # | Tên | Dùng khi |
|---|------|----------|
| A | **Scene Rendering** | Viết beat (POV, tone, luật, stakes, cú đấm) |
| B | **Brainstorm 15 Hướng** | Tìm biến thể, mở rộng ý tưởng |
| C | **Adversarial Edit** | Biên tập tàn nhẫn (7 câu TELL, cắt 25%, 5 chỗ lặp) |
| D | **Voice Calibration** | Neo giọng văn đầu phiên (DNA 300-500 từ) |
| E | **Intensity Map** | Đường cong cường độ |
| F | **Cross-Check** | Kiểm tra coherence với chương trước |
| G | **Ghost Reader** | Đọc như độc giả lần đầu |
| H | **Council** | Hội đồng Nacharium thẩm định |

### Công thức Prompt 3 Tầng

| Tầng | Nội dung | Thiếu thì sao |
|------|----------|----------------|
| **A: LUẬT** | POV, tone, cấm gì, nhịp câu, độ dài | AI viết chung chung |
| **B: ĐẦU RA** | Template scene, checklist giác quan, ẩn dụ | Scene mờ nhạt |
| **C: CÚ ĐẤM** | 1 thứ duy nhất làm người đọc mất ngủ | Scene "ổn" nhưng không đáng nhớ |

### 12 Bí Kíp Prompt Thực Chiến

| # | Bí kíp | Mô tả |
|---|--------|-------|
| 1 | 3 phiên bản nhịp | Viết cùng sự kiện 3 nhịp: nhanh/vừa/chậm → chọn hay nhất |
| 2 | Thoại = quyền lực | Mỗi câu thoại đổi trạng thái quyền lực giữa nhân vật |
| 3 | Chekhov dài hạn | Cài chi tiết vô nghĩa → 10-20 chương sau nổ |
| 4 | Giới hạn từ | 900-1200 từ/scene — buộc AI chọn lọc |
| 5 | 1 tính từ/đoạn | Ép AI tả bằng hình ảnh, không tô son bằng tính từ |
| 6 | POV sai lệch | Người kể tin sai 1 thứ → dramatic irony |
| 7 | Đổi giác quan chủ đạo | Mỗi scene 1 giác quan: âm thanh, xúc giác, nhiệt... |
| 8 | Đổi hệ ẩn dụ | Bỏ ẩn dụ quen → hệ lạ: cơ khí, y khoa, côn trùng |
| 9 | Conflict map trước combat | Ai đánh vì gì? Sợ mất gì? Chiến thắng giá gì? |
| 10 | Nhịp thở cho câu | Đánh dấu chỗ THỞ và chỗ NGHẸT trong outline |
| 11 | Cấm lore dump | Mọi lore qua hành động/thoại. Giải thích > 2 câu = dump |
| 12 | Kết bằng hình ảnh | Kết scene bằng hình ảnh mở, không bằng câu trả lời |

→ Copy-paste prompts: [references/prompts.md](references/prompts.md)

---

## PHẦN 10: CHẨN ĐOÁN & SỬA LỖI

### 10 bệnh thường gặp — Tra nhanh

| Bệnh | Triệu chứng | Thuốc | Lệnh tắt |
|------|-------------|-------|-----------|
| AI Padding | Viết dài nhưng rỗng, lặp ý | KT2 Chain of Density | — |
| Giọng phèn | Bóng bẩy rỗng ruột, "mùi AI" | KT4 DNA Sample | `VIẾT` |
| Tell don't Show | Giải thích cảm xúc trực tiếp | KT7 CẤM từ cảm xúc | `SENSORY` |
| Giọng trôi | Chương 5 khác chương 1 | Voice Kit đầu mỗi phiên | — |
| Flat emotion | Cường độ đều từ đầu tới cuối | KT6 Emotional Mapping | `EMOTION` |
| Cliché tràn lan | Ẩn dụ quen, twist đoán được | KT7 + `REVERSE` | `REVERSE` |
| Nhân vật phẳng | Một chiều, không mâu thuẫn | Vết thương + bí mật | `DEEPER` |
| Lore dump | Giải thích worldbuilding trực tiếp | Mọi lore qua hành động/thoại | — |
| Nhịp đều | Mọi đoạn cùng nhịp | KT11 Tempo Scripting | — |
| Mâu thuẫn logic | Chi tiết chương sau trái trước | Cross-check + Council | `COUNCIL` |

### Bệnh nâng cao

| Bệnh | Mô tả | Thuốc |
|------|-------|-------|
| **GHOST VOICE** | Giọng nịnh AI — ca ngợi quá mức, "brilliant", "stunning" | Humanize Pass trong bước G |
| **MIRROR CHARACTER** | Nhân vật phụ clone tính cách nhân vật chính | Character Sheet riêng + 3 câu thoại mẫu khác biệt |
| **SYMBOLISM PHỒNG** | Ẩn dụ quá rõ ràng, giải thích thay vì gợi | CẤM giải thích ẩn dụ. Để người đọc tự tìm |
| **EM DASH SPAM** | Quá nhiều dấu — trong 1 đoạn | Giới hạn tối đa 2 em-dash / đoạn |
| **STRUCTURE LOOP** | Mở đầu nhiều đoạn giống nhau | Vary câu mở: câu dài → cụt → hình ảnh → thoại |
| **OVER-EXPLAINING** | Giải thích cái người đọc đã hiểu | Cắt mọi giải thích thừa. Tin người đọc thông minh |

→ Chi tiết + prompt sửa: [references/diagnostics.md](references/diagnostics.md)

---

## PHẦN 11: QUY TẮC BẤT BIẾN

### 15 KHÔNG BAO GIỜ ⛔

1. **Không sến.** Cảm xúc mạnh nhất đến từ kiềm chế.
2. **Không văn vẻ bóng bẩy mà rỗng ruột** — mỗi câu phải có xương sống.
3. **Không giảng đạo đức trong truyện** — để nhân vật SỐNG, không để tác giả GIẢNG.
4. **Không né tránh đề tài dark/mature** nếu phục vụ câu chuyện.
5. **Không nhân vật một chiều** — pure good/evil không tồn tại.
6. **Không giải thích quá nhiều** — tin tưởng người đọc.
7. **Không dùng cliché** trừ khi subvert có chủ đích.
8. **Không ngắt brainstorm để hỏi** — momentum quý hơn sự an toàn.
9. **Không paste toàn bộ kỹ thuật vào 1 prompt** — chỉ 3-5 cái cần.
10. **Không viết cả chương cùng lúc** — viết từng beat 400-600 từ.
11. **Không để AI tự hài lòng** — luôn Adversarial Edit sau draft.
12. **Không viết mà không có Skeleton Key** — chương không có cốt lõi là thừa.
13. **Không lore dump** — mọi worldbuilding qua hành động/đối thoại.
14. **Không dùng từ chỉ cảm xúc trực tiếp** — cho thấy qua hành vi.
15. **Không kết scene bằng câu trả lời** — kết bằng hình ảnh mở.

### 10 Nguyên Tắc Vàng

| # | Nguyên tắc | Tại sao |
|---|-----------|---------|
| 1 | AI là dàn nhạc, bạn là nhạc trưởng | AI tạo nguyên liệu, bạn nâng cấp |
| 2 | Ví dụ cụ thể > mô tả trừu tượng | DNA Sample hiệu quả gấp 10 lần |
| 3 | Nén trước, nở sau | Chống padding, mỗi câu mang trọng lượng |
| 4 | Giới hạn = sáng tạo | Constraint đẩy AI ra khỏi comfort zone |
| 5 | Viết từng mảnh, không viết cả chương | Kiểm soát chất lượng từng beat |
| 6 | Không sến. Không uỷ mị. Không bao giờ. | Cảm xúc mạnh đến từ kiềm chế |
| 7 | Neo giọng văn đầu mỗi phiên | Chống giọng trôi |
| 8 | Biết vị trí cường độ | AI cần bối cảnh vị trí trong tổng thể |
| 9 | Mỗi chương có 1 Skeleton Key | Mọi thứ orbit quanh nó |
| 10 | Cross-check + Council sau mỗi chương | Chống mâu thuẫn + đảm bảo chất lượng |

### Quy tắc giọng văn xuyên suốt

- **Sắc bén, không sến.** Mỗi câu phải có xương sống.
- **Show, don't tell — luôn luôn.** Cho thấy qua hành vi, chi tiết cơ thể, đồ vật.
- **Đối thoại tự nhiên, có cá tính.** Che tên mà không phân biệt được = thoại hỏng.
- **Nhịp văn linh hoạt.** Nhanh khi căng — câu ngắn, cụt. Chậm khi sâu — câu dài, uốn lượn.
- **Cảm xúc kiềm chế > tuôn trào.** Một giọt nước mắt > ba đoạn mô tả nỗi đau.

### Quy tắc 30/70 Context Window

- Instruction ≤ 30% context window. 70% dành cho AI tạo content.
- Chỉ paste 3-5 kỹ thuật CỤ THỂ cho scene đang viết.

### Output Format — Tác phẩm sạch

**TUYỆT ĐỐI KHÔNG CÓ** trong prose:
- `# ## ###` (markdown headers)
- `** **` (bold) / `* *` (italic markdown)
- ` ``` ` (code blocks) / `>` (blockquotes)

**CHỈ CÓ:**
- Text thuần tiếng Việt có dấu đầy đủ
- Dấu câu chuẩn, xuống dòng tự nhiên
- Tên chương VIẾT HOA
- Đầu file: tên sách + tác giả
- Cuối file: *"— Hết —"*

---

## PHẦN 12: HỆ THỐNG LỆNH

### 14 lệnh tắt FORGE

| Lệnh | AI làm gì |
|-------|-----------|
| `BRAINSTORM` | Bùng nổ 10-15 ý tưởng, không tự kiểm duyệt |
| `VIẾT` | Chuyển chế độ prose: đẹp, nhịp điệu, cảm xúc |
| `PHÂN TÍCH` | Đánh giá khách quan: mạnh/yếu, gợi ý cải thiện |
| `OUTLINE` | Tạo dàn ý chi tiết, turning points, arc |
| `10X` | 10 biến thể ý tưởng vừa nêu |
| `TWIST` | Thêm plot twist bất ngờ nhưng hợp logic |
| `DEEPER` | Đào sâu tâm lý/động cơ/vết thương nhân vật |
| `CONFLICT+` | Tăng xung đột và stakes |
| `SENSORY` | Thêm chi tiết giác quan: mùi, vị, âm, nhiệt, texture |
| `DIALOGUE` | Viết đối thoại có giọng riêng từng nhân vật |
| `REVERSE` | Đảo ngược/subvert expectation |
| `EMOTION` | Tăng chiều sâu cảm xúc mà KHÔNG sến |
| `COUNCIL` | Spawn hội đồng Nacharium thẩm định |
| `OIF` | Kích hoạt Omni Infinity Forge loop |

### 5 lệnh OIF

| Lệnh | Hành động |
|-------|-----------|
| `OIF START` | Seed mới → auto-forge |
| `OIF STATUS` | Báo cáo tiến độ |
| `OIF PAUSE` | Tạm dừng |
| `OIF RESUME` | Tiếp tục |
| `OIF STOP` | Dừng hoàn toàn |

---

## PHẦN 13: CHECKLIST

→ Chi tiết đầy đủ: [references/checklist.md](references/checklist.md)

### Trước khi viết (7 mục)

- [ ] Đã paste Voice Calibration Kit (đoạn mẫu đúng tần số)
- [ ] Đã xác định Skeleton Key (1 câu duy nhất chương này tồn tại vì)
- [ ] Đã vẽ Emotional Map (đường cong cảm xúc với đỉnh + thung lũng)
- [ ] Đã viết Tempo Script (bản nhịp)
- [ ] Đã chọn 3 PHẢI + 3 CẤM (constraint)
- [ ] Đã xác định cường độ (vị trí trong tổng thể, thang 1-10)
- [ ] Đã viết micro-outline 10-15 beats

### Sau khi viết (10 mục)

- [ ] Đã Adversarial Edit với 5 tiêu chí + Humanize Pass
- [ ] Đã Ghost Reader test (3 câu hỏi, chỗ chán, hình ảnh ám ảnh)
- [ ] Đã Elevate (3 câu hay nhất → nâng toàn bộ)
- [ ] Đã Cross-check với chương trước (nhân vật, worldbuilding, timeline)
- [ ] Đã Resonance Audit (motif đúng chỗ, đúng nghĩa mới)
- [ ] Mỗi câu phục vụ Skeleton Key? Câu nào không → cắt
- [ ] Đã cắt ≥ 15% so với draft đầu
- [ ] Đã qua Council Nacharium — điểm ≥ 7/10
- [ ] Đã rà soát vết tích AI — không còn dấu hiệu máy viết
- [ ] Đã Self-Absorption (hấp thụ bài học từ report)

### File naming convention

| Loại file | Format |
|-----------|--------|
| Manuscript FINAL | `"[Tên Tiếng Việt]_Tiểu-Tâm_FINAL.md"` |
| Report Nacharium | `"[Tên Tiếng Việt] - Đánh Giá Hội Đồng Nacharium.md"` |
| Novel Bible | `novel-bible.md` |
| Chương raw | `ch[XX]_beat[X].md` hoặc `ch[XX].md` |

Tất cả file: **tiếng Việt có dấu đầy đủ.**

---

## PHẦN 14: FAULT TOLERANCE

### Sub-agent timeout/bug

1. Kill agent bị lỗi
2. Re-spawn hoặc tự viết trực tiếp
3. Giữ kết quả agents khác
4. Workaround: dùng `exec cat > file` thay `write` tool nếu cần

### Disconnect/restart

1. Đọc `memory/` + `MEMORY.md`
2. Kiểm tra files — cái nào đã có
3. Tiếp tục từ chỗ dở — KHÔNG viết lại từ đầu

### Resume protocol

```
1. Đọc MASTER-TASK.md → biết chương nào đã PASS
2. Đọc MEMORY-TASK.md → biết bài học + điểm yếu
3. Tìm file cuối cùng đã viết → xác định beat dở dang
4. Resume từ beat đó → tiếp tục FORGE+C → Council
```

---

## PHẦN 15: THAM CHIẾU

### 96 yếu tố văn học

12 nhóm A→Z, 96 yếu tố cần kiểm soát: Cốt truyện, Nhân vật, Văn phong, Chủ đề, Cảm xúc, Bối cảnh, Sáng tạo, Kỹ thuật kể, Nhịp điệu, Mở/Kết, Xử lý thời gian, Chi tiết, Cảnh, Xung đột, Đối thoại, Motif, Người kể, Cấu trúc cảm xúc, Kỹ thuật nâng cao, Thế giới, Nhân vật phụ, Mở rộng, Cảm giác, Văn phong nâng cao, Đạo đức, Bổ sung.

**Cách dùng:** Scan → chọn 5-7 yếu tố cho chương đang viết. KHÔNG paste toàn bộ.

### 738 kỹ thuật văn học (3 cấp)

| Cấp | Số lượng | Nhóm |
|-----|----------|------|
| **Cơ Bản** | 150 | Ngôn ngữ (50), Tự sự (35), Phong cách (65) |
| **Trung Cấp** | 200 | Ngôn ngữ nâng cao (70), Tự sự nâng cao (130) |
| **Nâng Cao** | 183 | Khoa học & Công nghệ (80), Tâm lý & Triết học (103) |

**Quy tắc:** Master Cơ Bản trước khi lên Nâng Cao. Kết hợp 2-3 kỹ thuật > đơn lẻ.

### Bảng tần số giọng văn

| Tần số | Kỹ thuật văn học phù hợp |
|--------|-------------------------|
| Thì thầm | Câu cụt (#29), Khoảng lặng (#25), Negative Space |
| Sắc lạnh | Asyndeton (#37), Động từ mạnh (#42), Câu đơn (#26) |
| Sấm sét | Polysyndeton (#36), Anadiplosis (#35), Câu chồng (#30) |
| Nước mắt | Câu dài (#28), Em-dash (#40), Silence (#50) |
| Mộng mị | Stream of consciousness (#56), Prose rhythm (#24), Euphony (#22) |

→ Danh sách đầy đủ: [references/literary-lib.md](references/literary-lib.md)

---

## Quick Start — 3 Bước Bắt Đầu

### Bước 1: Chuẩn bị Voice Kit
Chọn 300-500 từ prose mẫu. Gắn tag giải thích nhịp, ẩn dụ, dấu câu.
→ Paste đầu mỗi phiên: *"Đây là DNA giọng văn. Duy trì tần số này."*

### Bước 2: Frame chương đầu tiên
- Skeleton Key — 1 câu duy nhất
- Hạt nhân cảm xúc — CẢM XÚC CỐT LÕI
- 3 PHẢI + 3 CẤM

### Bước 3: Chạy FORGE+C 2.0
Frame → Outline → Render (400-600 từ/beat) → Grind → Elevate → Cross-check → **Council**

---

*Omni Forge Novel V1.0 — Blueprint hoàn chỉnh*
*Chưng cất từ Omni Forge V2 + V3 + OIF V2 + METAFORGE V2*
*Credits: Mr Nấng / Nacharium / Tiểu Tâm*
*"Sáng tạo không có giới hạn. Mọi quy tắc đều có thể phá vỡ — miễn là phá vỡ có chủ đích và phục vụ câu chuyện."*
