# PayOS Payout API Sample

Ví dụ mẫu gọi API chuyển tiền (payout) PayOS bằng Node.js.

## Cài đặt

```bash
npm install
```

## Sử dụng

```bash
node index.js
```

## Lưu ý

- Không public các key thật lên repo công khai.
- Nên sử dụng biến môi trường để bảo mật thông tin.
- Tham khảo thêm tài liệu chính thức của PayOS để biết chi tiết các trường dữ liệu.
- Nên sinh giá trị `x-idempotency-key` là một UUID cho mỗi request thực tế để tránh trùng lặp giao dịch (đã tự động sinh trong code).

## Cấu trúc repo

- `index.js`: Mã mẫu gọi API chuyển tiền.
- `lib/signature.js`: Hàm tạo signature HMAC SHA-256.
- `.env.sample`: File mẫu biến môi trường.

## Tham khảo
- [Tài liệu PayOS](https://docs.payos.vn/) 