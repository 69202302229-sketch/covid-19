# COVID-19 Epidemiology Dashboard

นี่คือชุดเครื่องมือสำหรับนักวิชาการสาธารณสุข เพื่อใช้แสดงผลข้อมูลทางระบาดวิทยา (COVID-19) จาก Google Sheets แบบ Real-time

## ฟีเจอร์หลัก
1. **Real-time Data Parser:** ดึงข้อมูล CSV อัตโนมัติด้วย `PapaParse` จาก Google Sheets
2. **ESRI Map Integration:** แสดงพิกัดจุดเกิดโรคระดับพื้นที่และระดับบุคคลบนแผนที่ผ่าน `ArcGIS API for JavaScript`
3. **Interactive Charts:** แสดงกราฟแนวโน้ม (Timeline) และสัดส่วนรายพื้นที่โดยใช้ `Chart.js`
4. **Responsive Design:** แสดงผลได้อย่างเหมาะสมบนทุกขนาดหน้าจอด้วย `Bootstrap 5`

## วิธีการนำไปใช้งาน (Deploy to GitHub Pages)
1. นำไฟล์ทั้งหมดในโฟลเดอร์นี้อัปโหลดขึ้น GitHub Repository ของคุณ
2. ไปที่เมนู **Settings** ของ Repository 
3. เลือกเมนู **Pages** ที่แถบด้านซ้าย
4. ในส่วนของ Source ให้เลือก `main` (หรือ `master`) branch แล้วกด Save
5. รอสักครู่ คุณจะได้รับ URL สำหรับเข้าถึง Dashboard ของคุณได้ทันที!

## การแก้ไขข้อมูล
- แดชบอร์ดนี้เชื่อมต่อกับลิงก์ CSV ปัจจุบันของคุณแล้ว: `https://docs.google.com/spreadsheets/d/e/2PACX-1vRTskVb86j9vKRJOuzor-bF-_OjtHwqsmC_O2OojfE5oREjRJFf0F36Mzqy3hxeuA/pub?output=csv`
- หากมีการเปลี่ยนแปลงคอลัมน์ ระบบจะพยายามค้นหาคอลัมน์เกี่ยวกับ `lat, lon, date, province` โดยอัตโนมัติ
