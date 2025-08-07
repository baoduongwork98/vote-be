# Food Vote Backend (Node.js + Socket.IO)

## Mục đích
Backend realtime cho tính năng vote món ăn, sử dụng Express và Socket.IO.

## Cách chạy

1. Cài đặt dependencies:
   ```bash
   npm install
   ```
2. Chạy server:
   ```bash
   node server.js
   ```

Server sẽ chạy ở cổng 4000 (hoặc PORT bạn cấu hình).

## API
- `GET /api/menu`: Lấy danh sách món ăn mẫu.
- `GET /api/votes`: Lấy kết quả vote hiện tại.
- Socket.IO: Kết nối tới server, lắng nghe sự kiện `votes` và gửi sự kiện `vote` để vote realtime.

## Ghi chú
- Bạn có thể mở rộng thêm API hoặc lưu dữ liệu vào database nếu cần.
- Để kết nối từ frontend, dùng socket.io-client với URL server này.
