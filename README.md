---

```markdown
# 🎨 Prompt Studio — Single File

> เครื่องมือสร้างและจัดการ Prompt สำหรับ AI ในไฟล์ HTML เดียว
> ทำงานได้ทั้งบนมือถือ แท็บเล็ต และคอมพิวเตอร์ โดยไม่ต้องติดตั้งอะไรเพิ่ม

[![Single File](https://img.shields.io/badge/single--file-HTML-00e68a?style=flat-square)](./index.html)
[![No Build](https://img.shields.io/badge/build-none-00e68a?style=flat-square)]()
[![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](./LICENSE)
[![Mobile Friendly](https://img.shields.io/badge/mobile-friendly-00e68a?style=flat-square)]()

---

## 🌐 ลิงก์ใช้งานจริง

**[https://aa-ok99.github.io/Prompt-studio/](https://aa-ok99.github.io/Prompt-studio/)**

*(เปิดใช้งานได้หลังตั้งค่า GitHub Pages แล้ว — ดูหัวข้อ "การ Deploy" ด้านล่าง)*

---

## ✨ ฟีเจอร์หลัก

| ฟีเจอร์ | รายละเอียด |
|---|---|
| 📝 **Editor** | เขียนและแก้ไข Prompt พร้อมนับตัวอักษร / คำ / บรรทัด |
| 🧩 **Templates 90+** | คลังเทมเพลตพร้อมใช้ ครอบคลุม 14 หมวด |
| 🎯 **Smart Variables** | ระบบตัวแปรอัจฉริยะ — เลือก/พิมพ์/เติมตัวอย่างอัตโนมัติ |
| ❤️ **Favorites** | บันทึกเทมเพลตโปรดไว้ใช้ซ้ำ |
| 🕓 **History** | บันทึก Prompt อัตโนมัติ (สูงสุด 50 รายการ) ผ่าน `localStorage` |
| 📄 **File Viewer** | อ่านไฟล์โค้ด/text พร้อม Syntax Highlight (Prism.js) |
| 📤 **Import / Export** | สำรองและกู้คืนข้อมูลเป็น JSON |
| 🚀 **AI Test Links** | ลิงก์ทดสอบ Prompt กับ AI ฟรี 6 แพลตฟอร์ม |
| 📱 **Responsive** | ใช้งานได้เต็มรูปแบบบนมือถือ |

---

## 🗂️ หมวดเทมเพลต

`writing` · `code` · `image` · `chat` · `market` · `termux` · `music` · `video` · `business` · `agent` · `3d` · `web` · `automation` · `creative`

---

## 📁 โครงสร้างโปรเจกต์

```

Prompt-studio/
└── index.html      ← ไฟล์เดียวจบ (HTML + CSS + JS)
└── README.md       ← เอกสารที่คุณกำลังอ่านอยู่

```

---

## 🚀 วิธีใช้งาน

### วิธีที่ 1: เปิดออนไลน์ (แนะนำ)
1. เปิด **[GitHub Pages link](https://aa-ok99.github.io/Prompt-studio/)**
2. เริ่มใช้งานได้ทันที

### วิธีที่ 2: รันในเครื่อง
1. ดาวน์โหลด `index.html`
2. ดับเบิลคลิกเพื่อเปิดในเบราว์เซอร์
3. ไม่ต้องติดตั้ง Node.js หรือ build ใดๆ

### วิธีที่ 3: รันบน Termux (Android)
```bash
pkg install git
git clone https://github.com/Aa-ok99/Prompt-studio.git
cd Prompt-studio
# เปิดไฟล์ผ่านเบราว์เซอร์มือถือ
termux-open index.html
```

---

🌐 การ Deploy บน GitHub Pages

1. เข้า Settings ของ repo
2. เลือกเมนู Pages (แถบซ้าย)
3. Source → Deploy from a branch
4. Branch → main และโฟลเดอร์ / (root)
5. กด Save แล้วรอ 1–2 นาที
6. URL จะกลายเป็น: https://aa-ok99.github.io/Prompt-studio/

⚠️ GitHub Pages ใช้ได้กับ repo แบบ Public เท่านั้น

---

🎯 วิธีใช้ Smart Variables

เทมเพลตหลายตัวมีตัวแปรอยู่ในวงเล็บ [ชื่อตัวแปร] เช่น:

```
คุณเป็นนักเขียนบล็อกที่มีประสบการณ์ [จำนวนปี] ปี
จงเขียนบทความเรื่อง "[หัวข้อ]" ...
```

เมื่อคลิกใช้เทมเพลต ระบบจะเปิดหน้าต่างกรอกตัวแปรให้อัตโนมัติ พร้อม:

· ✅ ตรวจนับช่องที่กรอกแล้ว (progress bar)
· ✅ ปุ่ม 🚀 ตัวอย่าง + สร้าง + คัดลอก (เติมค่าตัวอย่างที่เหมาะสม + สร้าง Prompt + คัดลอกทันที)
· ✅ รองรับ checkbox / select / multiselect / color picker / range slider

---

🛠️ เทคโนโลยีที่ใช้

· HTML5 + CSS3 + Vanilla JS — ไม่มี framework
· localStorage — บันทึกประวัติและ favorites
· Prism.js — Syntax highlighting สำหรับ Viewer
· Font Awesome 6 — ไอคอน
· Google Fonts — Space Grotesk + JetBrains Mono

---

💾 การสำรองข้อมูล

ข้อมูลทั้งหมดเก็บใน localStorage ของเบราว์เซอร์ — ไม่ขึ้นกับเซิร์ฟเวอร์

· Export: กดปุ่ม ⬇ Export ที่ header → ได้ไฟล์ .json
· Import: กดปุ่ม ⬆ Import → เลือกไฟล์ .json ที่เคย export ไว้
· คำเตือน: การล้าง cache ของเบราว์เซอร์จะลบข้อมูลทั้งหมด → ควรรัน Export เป็นระยะ

---

🤝 การร่วมพัฒนา

Pull Request ยินดีต้อนรับเสมอ

```bash
git clone https://github.com/Aa-ok99/Prompt-studio.git
cd Prompt-studio
# แก้ไข index.html แล้ว commit
git add .
git commit -m "feat: add new template"
git push origin main
```

---

📄 License

MIT License — ใช้งานได้อย่างอิสระ ทั้งส่วนตัวและเชิงพาณิชย์

---

👤 ผู้พัฒนา

Aa-ok99 · GitHub

---

<p align="center">
  <sub>สร้างด้วย ❤️ และไฟล์ HTML เดียว</sub>
</p>
```

---
