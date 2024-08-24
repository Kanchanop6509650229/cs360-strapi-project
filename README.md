# cs360-strapi-project


## วัตถุประสงค์ของเว็บแอปพลิเคชัน Strapi
Strapi เป็นระบบจัดการเนื้อหาแบบ Headless (Headless CMS)* ที่พัฒนาด้วย Node.js และเป็นโอเพนซอร์ส โดยมีวัตถุประสงค์หลักในการให้นักพัฒนาสามารถสร้างและจัดการ API ได้อย่างรวดเร็วและยืดหยุ่น ในขณะเดียวกันก็มีหน้าหน้า dashboard ที่ใช้งานสะดวกและง่ายดาย รองรับการทำงานร่วมกับเทคโนโลยีต่างๆ ได้หลากหลาย เช่น React, Vue, Angular ทำให้นักพัฒนามีอิสระในการเลือกเทคโนโลยีฝั่ง frontend ที่เหมาะสมกับโปรเจค นอกจากนี้ Strapi ยังสามารถให้ผู้ใช้สามารถกำหนดโครงสร้างข้อมูล สร้าง API endpoints และจัดการสิทธิ์การเข้าถึงได้อย่างละเอียด

*ระบบการจัดการเนื้อหาแบบ headless คือ แนวคิดในการพัฒนาเว็บและแอปพลิเคชันที่แยกส่วนการจัดการเนื้อหา (Backend) ออกจากส่วนการแสดงผล (Frontend) อย่างชัดเจน โดย CMS ทำหน้าที่เพียงจัดการเนื้อหาและให้บริการผ่าน API เท่านั้น ไม่มีส่วนแสดงผลที่กำหนดตายตัว ทำให้ะสามารถเลือกเทคโนโลยี Frontend ได้อย่างอิสระ


## กรณีการใช้งาน
### 1. **การจัดการเนื้อหาข้ามแพลตฟอร์ม (Cross-Platform Content Management)**
   Strapi ช่วยให้จัดการเนื้อหาในที่เดียว และนำเนื้อหานั้นไปใช้ในหลายแพลตฟอร์มได้อย่างง่ายดาย เช่น เว็บไซต์ แอปพลิเคชันมือถือ และอุปกรณ์ IoT โดยเนื้อหาสามารถถูกส่งผ่าน API ไปยัง Frontend ของแพลตฟอร์มต่าง ๆ ทำให้มั่นใจได้ว่าข้อมูลจะถูกอัปเดตอย่างสม่ำเสมอ

   **ตัวอย่าง**: 
   - บริษัทสื่อที่มีการเผยแพร่ข่าวสารหรือบทความที่ต้องการนำเสนอในเว็บไซต์ แอปมือถือ และช่องทางอื่น ๆ เช่น อีเมล หรือการแจ้งเตือน
   - องค์กรที่มีเนื้อหาภายในสำหรับพนักงาน ซึ่งต้องการแสดงผลผ่านพอร์ทัลเว็บภายในและแอปพลิเคชันมือถือในเวลาเดียวกัน

### 2. **การพัฒนา Custom API**
   Strapi สามารถสร้างและปรับแต่ง API ที่สามารถใช้งานได้ตามความต้องการของโปรเจกต์ ไม่ว่าจะเป็น RESTful API หรือ GraphQL API ช่วยให้คุณมีความยืดหยุ่นในการเลือกและจัดการข้อมูล และส่งข้อมูลนั้นไปยังแพลตฟอร์มหรือระบบอื่น ๆ ตามที่ต้องการ

   **ตัวอย่าง**: 
   - การพัฒนาแพลตฟอร์มอีคอมเมิร์ซที่ซับซ้อนซึ่งต้องการ API เฉพาะสำหรับการจัดการคำสั่งซื้อ สินค้า และการชำระเงิน
   - การสร้างแอปพลิเคชันที่ต้องการการดึงข้อมูลแบบเฉพาะเจาะจง เช่น แอปพลิเคชันการท่องเที่ยวที่ดึงข้อมูลจากฐานข้อมูลหลาย ๆ แหล่งมาแสดงผลให้กับผู้ใช้

### 3. **การจัดการข้อมูลผู้ใช้และการรับรองสิทธิ์การเข้าถึง (User Management and Access Control)**
   Strapi มีระบบจัดการผู้ใช้และการรับรองสิทธิ์การเข้าถึงที่สามารถปรับแต่งได้ ทำให้สามารถกำหนดบทบาทและสิทธิ์การเข้าถึงที่แตกต่างกันสำหรับผู้ใช้ประเภทต่าง ๆ ได้อย่างง่ายดาย เหมาะสำหรับโปรเจกต์ที่ต้องการควบคุมการเข้าถึงข้อมูลในระดับที่ละเอียด เช่น ระบบที่มีข้อมูลที่ต้องรักษาความปลอดภัยสูง หรือแอปพลิเคชันที่มีผู้ใช้หลายกลุ่มที่มีสิทธิ์การเข้าถึงที่ต่างกัน

   **ตัวอย่าง**: 
   - ระบบจัดการเอกสารภายในองค์กรที่ต้องการให้เฉพาะพนักงานบางกลุ่มเข้าถึงเอกสารบางประเภทได้
   - แพลตฟอร์มการศึกษาที่ให้ผู้สอนมีสิทธิ์ในการจัดการเนื้อหา และนักเรียนมีสิทธิ์เฉพาะการเข้าถึงบทเรียนเท่านั้น

### 4. **การสร้างและจัดการบล็อกหรือเว็บไซต์เนื้อหาที่ต้องการการอัปเดตบ่อย ๆ (Blogs and Frequently Updated Content Sites)**
   Strapi สามารถในการจัดการเนื้อหาและการผสานรวมกับเครื่องมือที่หลากหลาย สามารถจัดการบทความ, รูปภาพ, วิดีโอ, และอื่น ๆ ได้ในที่เดียว และมั่นใจได้ว่าเนื้อหาจะถูกอัปเดตบนเว็บไซต์ได้อย่างรวดเร็ว

   **ตัวอย่าง**: 
   - บล็อกส่วนตัวหรือเว็บไซต์ของนักข่าวที่ต้องการเผยแพร่เนื้อหาใหม่ ๆ ทุกวันหรือทุกสัปดาห์
   - เว็บไซต์ข่าวที่มีเนื้อหาที่หลากหลายและต้องการการอัปเดตแบบเรียลไทม์

### 5. **แอปพลิเคชัน e-commerce**
   Strapi ช่วยให้สามารถจัดการข้อมูลผลิตภัณฑ์, คำสั่งซื้อ, ลูกค้า และข้อมูลอื่น ๆ ที่เกี่ยวข้องกับอีคอมเมิร์ซได้อย่างมีประสิทธิภาพ ระบบสามารถรวมเข้ากับแพลตฟอร์มการชำระเงินและการจัดส่ง นอกจากนี้ยังสามารถรองรับการปรับแต่งตามความต้องการของธุรกิจได้อย่างยืดหยุ่น

   **ตัวอย่าง**: 
   - ร้านค้าออนไลน์ที่ต้องการระบบจัดการผลิตภัณฑ์ที่สามารถอัปเดตราคาและสต็อกสินค้าได้ง่าย ๆ


## องค์ประกอบ


## วิธีการติดตั้งแอปพลิเคชัน Strapi Application ด้วย CLI

### การเตรียมการก่อนเริ่มการติดตั้ง
- [NodeJS](https://nodejs.org/en) (เฉพาะ v18 หรือ v20 เท่านั้น)
- Node.js package manager (สามารถเลือกใช้ได้ตามสะดวก) : [npm](https://docs.npmjs.com/cli/v6/commands/npm-install) (v6 หรือใหม่กว่า)
- [Python](https://www.python.org/downloads/) (หากเลือกใช้ Database เป็น SQLite)

### เริ่มต้นการสร้างโปรเจกต์
1. เปิด command prompt แล้วไปที่ Directory ที่ต้องการจะสร้างโปรเจกต์
```bash
cd "Path ไปยังโฟลเดอร์"
```

2. พิมพ์คำสั่งในการติดตั้ง
```bash
npx create-strapi-app@latest ชื่อโปรเจกต์
```
หรือสามารถติดตั้งตามค่า default ได้ด้วยคำสั่ง
```bash
npx create-strapi-app@latest ชื่อโปรเจกต์ --quickstart
```


## วิธีการรันแอปพลิเคชั่น Strapi Application ด้วย CLI
1. เปิด command prompt แล้วไปที่ Directory ของโปรเจกต์ที่ได้สร้างไว้
```bash
cd "Path ไปยังโฟลเดอร์"
```

2. พิมพ์คำสั่ง
```bash
npm run develop
```


## ข้อมูลอ้างอิง
ข้อมูลบางส่วนได้รับการอ้างอิงจากบทความที่เกี่ยวข้อง:  
[Strapi คืออะไร และทำไมถึงได้รับความนิยมในโลกของ Headless CMS](https://morphos.is/th/blog/what-is-strapi-and-how-it-will-dominate-the-world-of-headless-cms)
[ลองเล่น Strapi — Headless CMS กัน](https://medium.com/i-gear-geek/%E0%B8%A5%E0%B8%AD%E0%B8%87%E0%B9%80%E0%B8%A5%E0%B9%88%E0%B8%99-strapi-headless-cms-%E0%B8%81%E0%B8%B1%E0%B8%99-f26ff53ac069)
[Installing from CLI](https://docs.strapi.io/dev-docs/installation/cli)
