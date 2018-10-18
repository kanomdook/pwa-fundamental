# Hosting PWA on Firebase

รันคำสั่ง `npm run build`

## เตรียมโปรเจค Firebase Hosting

1. สร้าง account firebase และ login เข้า dashboard ของ [Firebase Hosting](https://console.firebase.google.com/u/0/project/_/hosting?pli=1)
2. กด. Add Project
3. จากเมนูด้านซ้าย เลือกในส่วน **Hosting** 
4. กดเลือก **Get Started** และทำตามขั้นตอน
5. ติดตั้ง firebase tool ด้วยคำสั่ง `npm install -g firebase-tools`
6. รันคำสั่ง `firebase login`


### Error 401

ถ้าเจอ error แบบด้านล่าง ให้สั่ง `firebase logout` และสั่ง `firebase login` ใหม่

```bash
 Error: HTTP Error: 401, Request had invalid authentication credentials. Expected OAuth 2 access token, login cookie or other valid authentication credential. 
```

## Deploy to Firebase hosting

1. รันคำสั่ง `firebase init`
2. เลือก hosting โดยการกดปุ่ม space bar และกด enter เพื่อยืนยัน
3. เลือก Project ที่สร้างเตรียมไว้จากรายการ
4. พิมพ์ชื่อโฟลเดอร์ที่ต้องการใช้ในการ deploy ในที่นี้คือ **wwwื**
2. รันคำสั่ง `firebase deploy`
