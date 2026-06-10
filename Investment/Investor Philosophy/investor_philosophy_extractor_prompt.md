# Investor Philosophy Extractor — Ready-to-Use Prompt

**วิธีใช้**: Copy prompt ด้านล่างทั้งหมด → แนบไฟล์ transcript → วางใน Claude แล้วส่งได้เลย  
**Output**: ไฟล์ Markdown 1 ไฟล์ต่อนักลงทุน 1 คน พร้อมใช้เป็น AI knowledge base

---

## ✅ PROMPT (Copy ทั้งหมดด้านล่างนี้)

---

You are an expert at extracting the deep investment philosophy from interviews, lectures, and transcripts of master investors.

Your job is NOT to create a generic checklist. Your job is to faithfully reconstruct HOW THIS SPECIFIC PERSON THINKS about investing — their mental models, their first principles, their hard-won beliefs — as if you were creating a "mind clone" of this investor for future AI use.

The output must be a single, clean Markdown file that another AI can use as a reference knowledge base when answering investment questions in the style of this investor.

---

## TRANSCRIPT QUALITY NOTE

The attached transcript may be auto-generated (e.g. YouTube auto-subtitles). Apply these rules before processing:

- Spelling of financial terms may be corrupted — use context to infer correct meaning
  - e.g. "แช Cycle" → "Cash Cycle", "war and Buffet" → "Warren Buffett", "roic" → "ROIC"
- Sentences may be fragmented or cut mid-thought — reconstruct meaning from surrounding context
- Do NOT quote corrupted text verbatim in the output
- If a term is ambiguous, note your interpretation briefly in parentheses

---

## INVESTOR CONTEXT

Fill in before sending (leave blank if unknown — AI will infer from transcript):

- **Name**: {ชื่อนักลงทุน}
- **Source**: {ชื่อรายการ / ช่อง / งาน}
- **Date**: {ปี หรือช่วงเวลา}
- **Market environment at the time**: {สภาพตลาด เช่น ขาลง / ดอกเบี้ยสูง / post-crisis}
- **Investor background**: {สไตล์ เช่น VI / Growth / ประสบการณ์กี่ปี}

---

## CRITICAL RULES

1. Every insight must be grounded in something the investor ACTUALLY SAID — no fabrication, no generic advice padded in
2. Capture their exact language and metaphors where possible — these reveal how they truly think
3. Distinguish between "rules they always apply" vs "principles they apply situationally"
4. If the investor contradicts conventional wisdom, highlight this explicitly — it is often the most valuable insight
5. Prioritize PHILOSOPHY over mechanics — why they think this way matters more than what ratio they use
6. Output language: ใช้ภาษาไทยสำหรับคำอธิบายทั้งหมด คงคำศัพท์การเงินเป็นภาษาอังกฤษตามเดิม (ROE, Cash Cycle, ROIC ฯลฯ)

---

## OUTPUT FORMAT

Produce exactly the following Markdown structure. Save as: `[investor-name]_philosophy.md`

---

# [Investor Name] — Investment Philosophy Profile
**Source**: [รายการ / งาน]
**Date**: [ปี]
**Compiled for AI use**: Yes — use this file as a knowledge base to reason in this investor's style

---

## 1. Core Philosophy (แก่นแท้ปรัชญา)

เขียน 1 ย่อหน้า (3–5 ประโยค) ที่สะท้อนความเชื่อลึกที่สุดของนักลงทุนคนนี้ ไม่ใช่รายการข้อ ไม่ใช่สรุปทั่วไป — แต่เป็น worldview ที่เขาใช้ตัดสินใจทุกอย่าง เขียนในเสียงของเขาเอง (first person)

> *"[เขียนราวกับนักลงทุนคนนี้กำลังพูด worldview ของตัวเองใน 3–5 ประโยค]"*

---

## 2. First Principles (หลักการที่ไม่เคยละทิ้ง)

หลักการที่นักลงทุนคนนี้ยึดถือโดยไม่มีข้อยกเว้น ไม่ว่าตลาดจะเป็นอย่างไร

### Principle [N]: [ชื่อหลักการ]
- **ความเชื่อ**: [หลักการนั้นคืออะไร ในภาษาเข้าใจง่าย]
- **เหตุผลเบื้องหลัง**: [ทำไมเขาถึงเชื่อเช่นนี้ — มาจากประสบการณ์หรือเหตุผลอะไรใน transcript]
- **แสดงออกในทางปฏิบัติอย่างไร**: [พฤติกรรมหรือการตัดสินใจที่เห็นได้ชัดจากหลักการนี้]
- **คำพูดของเขาเอง**: [ประโยคหรือวลีจาก transcript ที่สะท้อนหลักการนี้ได้ดีที่สุด — ภาษาเดิม]
- **Contrarian note** *(ถ้ามี)*: [ถ้าหลักการนี้ขัดกับ conventional wisdom ให้ระบุว่าขัดอย่างไร]

---

## 3. Mental Models (กรอบความคิดที่ใช้มองธุรกิจ)

เครื่องมือคิดและ analogy ที่นักลงทุนคนนี้ใช้ประเมินธุรกิจ — ไม่ใช่ตัวเลข แต่เป็น "วิธีมอง"

### Model [N]: [ชื่อ Model]
- **Model นี้คืออะไร**: [อธิบาย]
- **ใช้เมื่อไหร่และอย่างไร**: [บริบทที่เขานำมาใช้]
- **ตัวอย่างจาก transcript**: [case study หรือตัวอย่างที่เขายกมา]

---

## 4. Decision Framework (ลำดับการตัดสินใจ)

ลำดับคำถามที่นักลงทุนคนนี้ถามเมื่อประเมินการลงทุน — **ลำดับสำคัญมาก** อะไรดูก่อน อะไรดูทีหลัง

```
Step 1: [ดูอะไรก่อน — และทำไมถึงดูสิ่งนี้ก่อน]
Step 2: [ดูอะไรต่อ]
...
Step N: [ดูอะไรสุดท้าย — มักเป็น valuation / ราคา]

ผ่านทุก Step แล้ว → ค่อยพิจารณา position size และจังหวะเข้า
```

ระบุ "เงื่อนไขที่ทำให้ไม่ลงทุน" ที่นักลงทุนคนนี้พูดถึงโดยตรงด้วย

---

## 5. What This Investor Truly Fears (สิ่งที่กังวลที่สุด)

ความเสี่ยงที่นักลงทุนคนนี้กังวลจริงๆ — ไม่ใช่ความเสี่ยงทั่วไป แต่เป็น failure mode เฉพาะตัวที่เขาพูดถึงหรือสะท้อนออกมาใน transcript

- **[ชื่อความกังวล]**: [มันคืออะไร ทำไมเขาถึงกลัวสิ่งนี้มากกว่าสิ่งอื่น]

---

## 6. Signature Insights (ข้อคิดที่หาจากที่อื่นไม่ได้)

3–5 insight จากนักลงทุนคนนี้โดยเฉพาะ — ที่ไม่มีในหนังสือการลงทุนทั่วไป ควรรู้สึก "แปลกใหม่" หรือ "เฉพาะตัวมาก"

- **[ชื่อ insight]**: [insight นั้นคืออะไร + ทำไมมันสำคัญ + คำพูดต้นฉบับถ้ามี]

---

## 7. What This Investor Would Say About... (การประยุกต์ใช้)

อนุมานจาก transcript ว่านักลงทุนคนนี้จะตอบสถานการณ์เหล่านี้อย่างไร

| สถานการณ์ | มุมมองที่น่าจะเป็น | อ้างอิงจาก transcript |
|----------|-----------------|----------------------|
| หุ้น ROE ดีแต่ราคาแพงกว่า fair value | | |
| ธุรกิจที่ตัวเองไม่มีความรู้เลย | | |
| ตลาดขาลงหนัก ทุกหุ้นร่วง | | |
| หุ้นที่ถืออยู่ราคาถึง target price แล้ว | | |
| บริษัทดีแต่ management ไม่น่าเชื่อถือ | | |
| หุ้นที่ตัวเองถืออยู่มีข่าวร้ายออกมา | | |

---

## 8. Applicability to Thai Market — SET/mai (การนำไปใช้จริง)

ประเมินว่าแต่ละ First Principle ใช้ได้กับหุ้นไทยโดยตรงแค่ไหน

| หลักการ | ใช้ได้กับ SET/mai | หมายเหตุ / สิ่งที่ต้องปรับ |
|--------|-----------------|--------------------------|
| [Principle 1] | ⭐⭐⭐ ใช้ได้ทันที / ⭐⭐ ต้องปรับบริบท / ⭐ เป็น concept เท่านั้น | |

---

## 9. AI Usage Instructions (วิธีให้ AI ใช้ไฟล์นี้)

> *Section นี้สำหรับ AI ที่รับไฟล์นี้เป็น context — ไม่ใช่สำหรับนักลงทุนที่อ่าน*

เมื่อใช้ไฟล์นี้เป็น knowledge base:
- ใช้ **Section 1 (Core Philosophy)** เป็นฐานของทุกคำตอบ — ถ้าขัดกับ Core Philosophy ต้องระบุ
- ใช้ **Section 4 (Decision Framework)** ตามลำดับ Step เสมอ — ห้ามข้ามขั้นตอน
- **Section 2 และ 3** คือ "เหตุผล" เบื้องหลัง — อธิบาย why เสมอ ไม่ใช่แค่ what
- ถ้าถามเรื่องที่ไม่มีใน transcript → extrapolate จาก Section 7 patterns และระบุว่าเป็นการอนุมาน
- มุมมองใน transcript นี้ถ่ายไว้ ณ **[DATE]** — ถ้าบริบทตลาดเปลี่ยนแล้ว ให้ flag ก่อนตอบ
- ห้ามผสมมุมมองของนักลงทุนคนนี้กับนักลงทุนคนอื่น ยกเว้นถูกขอให้เปรียบเทียบโดยตรง

---

*Generated from transcript. All insights are attributed to the investor named above.*

