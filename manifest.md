# manifest.json

ใช้เป็นข้อมูลสำหรับ OS ที่จะโต้ตอบกับ Progressive Web App ในรูปแบบต่างๆ 

## สร้างไฟล์ manifest.json

สร้างไฟล์ `manifest.json`

```json
{
  "name": "Your Great Site",
  "short_name": "Site",
  "description": "Learn how to create and share something or other.",
  "start_url": "/index.html",
  "background_color": "#000000",
  "theme_color": "#0f4a73",
  "icons": [{
    "src": "icon-256.png",      
    "sizes": "256x256",
    "type": "image/png"
  }]
}
```                 

แทรกไฟล์ด้วย tag `link` ไปใน `index.html`

```html
<head>
    <link rel="manifest" href="manifest.json" />
</head>
```