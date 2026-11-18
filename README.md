# Mitube

Ứng dụng xem YouTube không quảng cáo (dùng cá nhân), có bản điện thoại và bản **Android TV / Google TV**.

## Cài lần đầu — điện thoại

1. Tải ở bản mới nhất: **[Releases → Latest](https://github.com/nct-code/mitube-releases/releases/latest)**
   - Hầu hết điện thoại: `Mitube-arm64-v8a.apk`
   - Máy cũ / không chắc: `Mitube-universal.apk`
2. Mở file, cho phép "Cài ứng dụng không rõ nguồn gốc" nếu máy hỏi, rồi cài.
3. Mở Mitube, bấm **Cho phép** khi app xin quyền thông báo (để nhận tin có bản mới).

## Cài lần đầu — TV (Mitube TV)

Cách dễ nhất là qua ADB từ máy tính cùng Wi-Fi (bật Gỡ lỗi USB / mạng trong Tuỳ chọn nhà phát triển của TV):

```bash
adb connect <ip-tv>:5555
adb install -r Mitube-TV-armeabi-v7a.apk   # hoặc Mitube-TV-arm64-v8a.apk / Mitube-TV-universal.apk
```

Điều khiển: OK phát/dừng · Trái/Phải tua 10 giây · Lên/Xuống hiện bảng điều khiển · nút micro trên remote để tìm bằng giọng nói ·
"Hey Google, phát … trên Mitube TV".

## Cập nhật

Không cần tải lại thủ công: khi có bản mới, Mitube tự hiện **"Có bản Mitube mới"** → bấm **Cập nhật** → **Cài đặt**.
Lần đầu cập nhật, Android sẽ hỏi cho phép Mitube cài ứng dụng — bật một lần là xong. Dữ liệu (lịch sử, playlist, kênh) được giữ nguyên.
