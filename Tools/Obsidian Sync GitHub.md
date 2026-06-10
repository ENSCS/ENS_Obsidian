
## การ Sync ทุกครั้ง (3 คำสั่ง)

### Step 1 — เข้าโฟลเดอร์ vault

```bash
cd "/Users/xxx/ENS_Obsidian"
```

### Step 2 — ดึงการเปลี่ยนแปลงจาก GitHub ก่อน (ป้องกัน conflict)

```bash
git pull origin main
```

### Step 3 — Push ไฟล์ที่แก้ไขขึ้น GitHub

```bash
git add .
git commit -m "update notes"
git push origin main
```

---

## Commit Message แนะนำ

| สถานการณ์         | ข้อความ                               |
| ----------------- | ------------------------------------- |
| อัปเดตทั่วไป      | `git commit -m "update notes"`        |
| เพิ่ม oppday ใหม่ | `git commit -m "add PTTEP Q2 oppday"` |
| แก้ไขไฟล์เฉพาะ    | `git commit -m "edit MEGA watchlist"` |