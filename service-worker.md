# Service Worker

## สร้าง service worker แบบง่าย

สร้างไฟล์ `sw.js` ด้วยโค้ดด้านล่าง

```js
self.addEventListener('fetch', (event) => {});
```

ในไฟล์ `index.html` เพิ่ม `<script>` ที่ register ตัว service worker ลงไป

```js
if ('serviceWorker' in navigator) {
  // sw.js can literally be empty, but must exist
  navigator.serviceWorker.register('/sw.js');
}
```

## Reference

- [Google's Service Worker](https://developers.google.com/web/fundamentals/primers/service-workers/)
- [Workbox](https://developers.google.com/web/tools/workbox/)