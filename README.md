# Smart Farm Online Dashboard

หน้าเว็บดูสถานะ ESP32 ผ่าน HiveMQ Cloud แบบ read-only สำหรับ GitHub Pages

## ติดตั้งบน GitHub Pages

1. สร้าง Public repository ชื่อ `smartfarm-dashboard`
2. อัปโหลดไฟล์ `index.html` ไว้ที่หน้าแรกของ repository
3. เปิด `Settings` > `Pages`
4. ที่ `Build and deployment` เลือก `Deploy from a branch`
5. Branch เลือก `main` และโฟลเดอร์ `/ (root)` แล้วกด `Save`
6. เปิด `https://PW68-206.github.io/smartfarm-dashboard/`

หน้าเว็บจะถามบัญชี `smartfarm_dashboard` และรหัสผ่านทุกครั้งที่เปิดใหม่
รหัสผ่านไม่ถูกเขียนไว้ในไฟล์และไม่ถูกเก็บบน GitHub

## MQTT

- Secure WebSocket: port 8884, path `/mqtt`
- Subscribe: `smartfarm/device01/status`
- Subscribe: `smartfarm/device01/availability`
- ไม่มีปุ่มควบคุมและไม่มีการ Publish คำสั่ง
