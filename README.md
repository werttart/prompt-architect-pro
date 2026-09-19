# ⚡ Prompt Architect Pro

ระบบสร้าง Master Prompt อัจฉริยะ — คิด → วิเคราะห์ → วางแผน ก่อนสังเคราะห์ Master Prompt เพื่อสั่งงาน AI สร้างระบบ Google Apps Script 3 ไฟล์

> ไฟล์เดียว `index.html` — รันบนเบราว์เซอร์ เรียก Gemini API โดยตรง ไม่ต้องมี backend

## ✨ Features
- 3-Phase Pipeline: วิเคราะห์ความต้องการ → ออกแบบสถาปัตยกรรม → สังเคราะห์ Master Prompt
- รองรับ Gemini 2.5 Pro / Flash
- ส่งมอบ 3 ไฟล์ตามลำดับ: `Code.gs` → `Index.html` → `mockdata.gs` ด้วยคำสั่ง "ต่อไป"
- คัดลอก / ดาวน์โหลด Master Prompt ได้ทันที

## 🚀 วิธีใช้
1. เปิด `index.html` ด้วยเบราว์เซอร์ (ดับเบิลคลิกได้เลย)
2. กรอก ชื่อระบบ / กลุ่มผู้ใช้ / คำอธิบายระบบ
3. ใส่ Gemini API Key (ขอที่ https://aistudio.google.com/app/apikey)
4. กด **เริ่มกระบวนการสร้าง Master Prompt**
5. คัดลอกผลลัพธ์ไปวางใน Gemini / ChatGPT / Claude

## 🔐 ความปลอดภัย API Key
- Key ถูกใช้จากเบราว์เซอร์โดยตรง ไม่ส่งไปเซิร์ฟเวอร์อื่น
- ห้าม commit Key ลง Git — ไฟล์นี้ไม่มี hardcoded key
- ถ้าเคยโพสต์ Key ที่ไหน ให้ไป revoke ทันทีที่ https://aistudio.google.com/app/apikey

## 📂 โครงสร้าง
```
prompt-architect-pro/
├── index.html              # ไฟล์หลัก (HTML/CSS/JS จบในไฟล์เดียว)
├── prompt-architect.html   # สำเนาเดียวกัน
├── README.md
└── .gitignore
```

## 📄 License
MIT — ใช้เพื่อการเรียนการสอนได้อิสระ
