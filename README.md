# VinFast CRM – CSKH, quy tắc 3 ngày & Marketing hàng ngày

Web app (React + Tailwind qua CDN, một file `index.html`) quản lý khách hàng VinFast:
đăng nhập/đăng ký, đồng bộ đa thiết bị bằng Firebase Auth + Firestore, lịch sử chăm sóc,
hàng đợi chăm sóc lại sau 3 ngày, theo dõi bài viết/video hàng ngày, nhập/xuất CSV.

## Cài đặt Firebase
1. Tạo project tại https://console.firebase.google.com, thêm Web app và copy `firebaseConfig`.
2. Authentication → bật phương thức **Email/Password**.
3. Tạo **Firestore Database**, rồi publish nội dung `firestore.rules`.
4. Mở `index.html`, tìm `FIREBASE_CONFIG` và dán 4 giá trị (apiKey, authDomain, projectId, appId).

## Chạy / triển khai
- Chạy thử cục bộ: `npx serve .` (đừng mở trực tiếp bằng file://).
- Triển khai: `npm i -g firebase-tools && firebase login && firebase deploy`
  (hoặc GitHub Pages / Netlify).
