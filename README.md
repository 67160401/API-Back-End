## คำอธิบายโครงสร้างโปรเจกต์

```
student-api/
├── node_modules/
├── index.js
├── package.json
├── package-lock.json
├── postman-collection.md
└── README.md
```

- **node_modules/** : เก็บไลบรารีที่ติดตั้ง เช่น Express
- **index.js** : ไฟล์หลักของโปรเจกต์ ใช้สร้าง Express Server, กำหนด Mock Data และ API สำหรับ CRUD (GET, POST, PUT, DELETE)
- **package.json** : กำหนดข้อมูลโปรเจกต์, dependencies และ scripts
- **package-lock.json** : ล็อกเวอร์ชันของ dependencies เพื่อให้ติดตั้งได้เหมือนกันทุกเครื่อง
- **postman-collection.md** : 
- **README.md** : 

<br>

## ขั้นตอนที่ 3.2 ทบทวนคุณภาพของโค้ด
**โค้ดใน index.js มีการตรวจสอบข้อมูลนำเข้า (validation) ก่อนประมวลผลหรือไม่**
- มีการตรวจสอบ
<br>

**ทุก route มีการตอบกลับด้วย Status Code ที่เหมาะสมกับผลลัพธ์หรือไม่**
- มีความเหมาะสมกับผลลัพธ์
<br>

**โครงสร้างโค้ดในไฟล์เดียวยังอ่านง่ายอยู่หรือไม่ หากมี route เพิ่มขึ้นอีก 10 เส้นทาง จะเกิดปัญหาใดตามมา**
- โค้ดจะมีขนาดใหญ่และซับซ้อนขึ้น ทำให้ค้นหาหรือแก้ไขได้ยาก โอกาสเกิดข้อผิดพลาดก็มากขึ้นตามไปด้วย