# CS360 Strapi Project

## วัตถุประสงค์ของเว็บแอปพลิเคชัน Strapi

**Strapi** เป็นระบบจัดการเนื้อหาแบบ Headless (Headless CMS)* ที่พัฒนาด้วย Node.js และเป็นโอเพนซอร์ส โดยมีวัตถุประสงค์หลักในการให้นักพัฒนาสามารถสร้างและจัดการ API ได้อย่างรวดเร็วและยืดหยุ่น ในขณะเดียวกันก็มีหน้าหน้า dashboard ที่ใช้งานสะดวกและง่ายดาย รองรับการทำงานร่วมกับเทคโนโลยีต่างๆ ได้หลากหลาย เช่น React, Vue, Angular ทำให้นักพัฒนามีอิสระในการเลือกเทคโนโลยีฝั่ง frontend ที่เหมาะสมกับโปรเจค นอกจากนี้ Strapi ยังสามารถให้ผู้ใช้สามารถกำหนดโครงสร้างข้อมูล สร้าง API endpoints และจัดการสิทธิ์การเข้าถึงได้อย่างละเอียด

*ระบบการจัดการเนื้อหาแบบ headless คือ แนวคิดในการพัฒนาเว็บและแอปพลิเคชันที่แยกส่วนการจัดการเนื้อหา (Backend) ออกจากส่วนการแสดงผล (Frontend) อย่างชัดเจน โดย CMS ทำหน้าที่เพียงจัดการเนื้อหาและให้บริการผ่าน API เท่านั้น ไม่มีส่วนแสดงผลที่กำหนดตายตัว ทำให้ะสามารถเลือกเทคโนโลยี Frontend ได้อย่างอิสระ

---

## กรณีการใช้งาน

### 1. การจัดการเนื้อหาข้ามแพลตฟอร์ม (Cross-Platform Content Management)
- **รายละเอียด:** Strapi ช่วยให้จัดการเนื้อหาในที่เดียว และนำเนื้อหานั้นไปใช้ในหลายแพลตฟอร์มได้อย่างง่ายดาย เช่น เว็บไซต์ แอปพลิเคชันมือถือ และอุปกรณ์ IoT โดยเนื้อหาสามารถถูกส่งผ่าน API ไปยัง Frontend ของแพลตฟอร์มต่าง ๆ ทำให้มั่นใจได้ว่าข้อมูลจะถูกอัปเดตอย่างสม่ำเสมอ
- **ตัวอย่าง:**
  - บริษัทสื่อที่มีการเผยแพร่ข่าวสารหรือบทความที่ต้องการนำเสนอในเว็บไซต์ แอปมือถือ และช่องทางอื่น ๆ เช่น อีเมล หรือการแจ้งเตือน
  - องค์กรที่มีเนื้อหาภายในสำหรับพนักงาน ซึ่งต้องการแสดงผลผ่านพอร์ทัลเว็บภายในและแอปพลิเคชันมือถือในเวลาเดียวกัน

### 2. การพัฒนา Custom API
- **รายละเอียด:** Strapi สามารถสร้างและปรับแต่ง API ที่สามารถใช้งานได้ตามความต้องการของโปรเจกต์ ไม่ว่าจะเป็น RESTful API หรือ GraphQL API ช่วยให้คุณมีความยืดหยุ่นในการเลือกและจัดการข้อมูล และส่งข้อมูลนั้นไปยังแพลตฟอร์มหรือระบบอื่น ๆ ตามที่ต้องการ
- **ตัวอย่าง:**
  - การพัฒนาแพลตฟอร์มอีคอมเมิร์ซที่ซับซ้อนซึ่งต้องการ API เฉพาะสำหรับการจัดการคำสั่งซื้อ สินค้า และการชำระเงิน
  - การสร้างแอปพลิเคชันที่ต้องการการดึงข้อมูลแบบเฉพาะเจาะจง เช่น แอปพลิเคชันการท่องเที่ยวที่ดึงข้อมูลจากฐานข้อมูลหลาย ๆ แหล่งมาแสดงผลให้กับผู้ใช้

### 3. การจัดการข้อมูลผู้ใช้และการรับรองสิทธิ์การเข้าถึง (User Management and Access Control)
- **รายละเอียด:** Strapi มีระบบจัดการผู้ใช้และการรับรองสิทธิ์การเข้าถึงที่สามารถปรับแต่งได้ ทำให้สามารถกำหนดบทบาทและสิทธิ์การเข้าถึงที่แตกต่างกันสำหรับผู้ใช้ประเภทต่าง ๆ ได้อย่างง่ายดาย เหมาะสำหรับโปรเจกต์ที่ต้องการควบคุมการเข้าถึงข้อมูลในระดับที่ละเอียด เช่น ระบบที่มีข้อมูลที่ต้องรักษาความปลอดภัยสูง หรือแอปพลิเคชันที่มีผู้ใช้หลายกลุ่มที่มีสิทธิ์การเข้าถึงที่ต่างกัน
- **ตัวอย่าง:**
  - ระบบจัดการเอกสารภายในองค์กรที่ต้องการให้เฉพาะพนักงานบางกลุ่มเข้าถึงเอกสารบางประเภทได้
  - แพลตฟอร์มการศึกษาที่ให้ผู้สอนมีสิทธิ์ในการจัดการเนื้อหา และนักเรียนมีสิทธิ์เฉพาะการเข้าถึงบทเรียนเท่านั้น

### 4. การสร้างและจัดการบล็อกหรือเว็บไซต์เนื้อหาที่ต้องการการอัปเดตบ่อย ๆ (Blogs and Frequently Updated Content Sites)
- **รายละเอียด:** Strapi สามารถในการจัดการเนื้อหาและการผสานรวมกับเครื่องมือที่หลากหลาย สามารถจัดการบทความ, รูปภาพ, วิดีโอ, และอื่น ๆ ได้ในที่เดียว และมั่นใจได้ว่าเนื้อหาจะถูกอัปเดตบนเว็บไซต์ได้อย่างรวดเร็ว
- **ตัวอย่าง:**
  - บล็อกส่วนตัวหรือเว็บไซต์ของนักข่าวที่ต้องการเผยแพร่เนื้อหาใหม่ ๆ ทุกวันหรือทุกสัปดาห์
  - เว็บไซต์ข่าวที่มีเนื้อหาที่หลากหลายและต้องการการอัปเดตแบบเรียลไทม์

### 5. แอปพลิเคชัน e-commerce
- **รายละเอียด:** Strapi ช่วยให้สามารถจัดการข้อมูลผลิตภัณฑ์, คำสั่งซื้อ, ลูกค้า และข้อมูลอื่น ๆ ที่เกี่ยวข้องกับอีคอมเมิร์ซได้อย่างมีประสิทธิภาพ ระบบสามารถรวมเข้ากับแพลตฟอร์มการชำระเงินและการจัดส่ง นอกจากนี้ยังสามารถรองรับการปรับแต่งตามความต้องการของธุรกิจได้อย่างยืดหยุ่น
- **ตัวอย่าง:** ร้านค้าออนไลน์ที่ต้องการระบบจัดการผลิตภัณฑ์ที่สามารถอัปเดตราคาและสต็อกสินค้าได้ง่าย ๆ

---

## องค์ประกอบ

(รอแก้ไข)

---

## วิธีการติดตั้งแอปพลิเคชัน Strapi Application ด้วย CLI

### การเตรียมการก่อนเริ่มการติดตั้ง
- **[NodeJS](https://nodejs.org/en)** (เฉพาะ v18 หรือ v20 เท่านั้น)
- **Node.js package manager** (yarn หรือ npm) : [yarn](https://yarnpkg.com/getting-started/install) 
- **[Python](https://www.python.org/downloads/)** (หากใช้ Database เป็น SQLite)

### เริ่มต้นการสร้างโปรเจกต์

1. เปิด command prompt แล้วไปที่ Directory ที่ต้องการจะสร้างโปรเจกต์
   ```bash
   cd Pathไปยังโฟลเดอร์
   ```
2. พิมพ์คำสั่งในการติดตั้ง
   ```bash
   yarn create-strapi-app@latest ชื่อโปรเจกต์
   ```
   หรือสามารถติดตั้งตามค่า default ได้ด้วยคำสั่ง
   ```bash
   yarn create-strapi-app@latest ชื่อโปรเจกต์ --quickstart
   ```

---

## วิธีการรันแอปพลิเคชัน Strapi Application ด้วย CLI

1. เปิด command prompt แล้วไปที่ Directory ของโปรเจกต์ที่ได้สร้างไว้
   ```bash
   cd Pathไปยังโฟลเดอร์
   ```
2. พิมพ์คำสั่ง
   ```bash
   yarn run develop
   ```

---

## การ Deploy ลง AWS

### 1. สร้าง AWS EC2 Instance

### 2. ติดตั้ง NodeJS ลงบน EC2
   ```bash
   cd ~
   sudo yum update
   ...
   sudo yum install -y ca-certificates curl gnupg
   ...
   sudo yum install nodejs -y
   ...
   node -v && npm -v
   ```

### 3. สร้างและเปลี่ยน npm default directory
   ```bash
   cd ~
   mkdir ~/.npm-global
   npm config set prefix '~/.npm-global'
   ...
   # แก้ไขไฟล์ .profile
   sudo nano ~/.profile

   # ใส่คำสั่งต่อไปนี้ไว้ล่างสุดของไฟล์
   export PATH=~/.npm-global/bin:$PATH
   ...
   # อัพเดตข้อมูล
   source ~/.profile
   ```

### 4. ติดตั้ง package ลงโปรเจกต์ในเครื่องของเรา
```bash
cd ที่อยู่โปรเจกต์ในEC2
yarn install pg
yarn install @strapi/provider-upload-aws-s3
```

### 5. แก้ไข config โปรเจกต์ที่ ./config/plugins.js ในเครื่องของเรา
```bash
module.exports = ({ env }) => ({
      upload: {
        config: {
          provider: 'aws-s3',
          providerOptions: {
            s3Options: {
              accessKeyId: env('AWS_ACCESS_KEY_ID'),
              secretAccessKey: env('AWS_ACCESS_SECRET'),
              region: env('AWS_REGION'),
              params: {
                Bucket: env('AWS_BUCKET_NAME'),
              },
            }
          },
          // These parameters could solve issues with ACL public-read access — see [this issue](https://github.com/strapi/strapi/issues/5868) for details
          actionOptions: {
            upload: {
              ACL: null
            },
            uploadStream: {
              ACL: null
            },
          }
        },
      }
    });
```

### 6. Push โปรเจกต์บนเครื่องขึ้น github
```bash
git add .
git commit -m 'ข้อความ commit'
git push
```

### 7. ทำการโคลนโปรเจกต์มาไว้ในเครื่อง EC2
```bash
cd ~
git clone https://github.com/ชื่อในgithub/ชื่อrepository.git
```

### 8. ติดตั้ง package ลงโปรเจกต์ในเครื่อง EC2
```bash
cd ที่อยู่โปรเจกต์ในEC2
yarn install
NODE_ENV=production yarn run build
```

### 9. ติดตั้ง PM2 Runtime
   ```bash
   cd ~
   yarn install pm2@latest -g
   ```

### 10. แก้ไข ecosystem.config.js
```javascript
cd ~
pm2 init
sudo nano ecosystem.config.js

# โดยแก้ไขข้อมูลข้างในไฟล์ดังนี้
module.exports = ({ env }) => ({
      upload: {
        config: {
          provider: 'aws-s3',
          providerOptions: {
            s3Options: {
              accessKeyId: env('AWS_ACCESS_KEY_ID'),
              secretAccessKey: env('AWS_ACCESS_SECRET'),
              region: env('AWS_REGION'),
              params: {
                Bucket: env('AWS_BUCKET_NAME'),
              },
            }
          },
          // These parameters could solve issues with ACL public-read access — see [this issue](https://github.com/strapi/strapi/issues/5868) for details
          actionOptions: {
            upload: {
              ACL: null
            },
            uploadStream: {
              ACL: null
            },
          }
        },
      }
    });
```

### 11. ตั้งค่า Security Group ของ EC2 ในส่วน Inbound

- **Type:** SSH, **Protocol:** TCP, **Port Range:** 22, **Source:** ::/0
- **Type:** HTTP, **Protocol:** TCP, **Port Range:** 80, **Source:** 0.0.0.0/0, ::/0
- **Type:** HTTPS, **Protocol:** TCP, **Port Range:** 443, **Source:** 0.0.0.0/0, ::/0
- **Custom TCP Rule, Protocol:** TCP, **Port Range:** 1337, **Source:** 0.0.0.0/0

### 12. Start PM2 ให้เว็ปไซต์ทำงาน โดยจะเข้าถึงเว็ปไซต์ได้ที่ http://public-ipของec2:1337/

```bash
cd ~
pm2 start ecosystem.config.js
```

### 13. ตั้งค่าให้ PM2 ทำงานทันทีเมื่อทำการเปิด EC2
```bash
cd ~
pm2 startup systemd
...
# หลังจากนั้น console จะพิมพ์คำสั่งมาให้ ทำการก็อปวางได้ เช่น
sudo env PATH=$PATH:/usr/bin /usr/lib/node_modules/pm2/bin/pm2 startup systemd -u your-name --hp /home/your-name
...
pm2 save
...
# reboot 1 รอบ
sudo reboot
```

---

## ข้อมูลอ้างอิง

- [Strapi คืออะไร และทำไมถึงได้รับความนิยมในโลกของ Headless CMS](https://morphos.is/th/blog/what-is-strapi-and-how-it-will-dominate-the-world-of-headless-cms)
- [ลองเล่น Strapi — Headless CMS กัน](https://medium.com/i-gear-geek/%E0%B8%A5%E0%B8%AD%E0%B8%87%E0%B9%80%E0%B8%A5%E0%B9%88%E0%B8%99-strapi-headless-cms-%E0%B8%81%E0%B8%B1%E0%B8%99-f26ff53ac069)
- [Installing from CLI](https://docs.strapi.io/dev-docs/installation/cli)
- [Amazon AWS Deployment](https://docs.strapi.io/dev-docs/deployment/amazon-aws)

---
