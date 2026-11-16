# Shop Phạm Nhật — Vercel deployment starter

## Deploy giao diện hiện tại
1. Tải thư mục này lên GitHub (hoặc upload ZIP nếu giao diện Vercel của bạn hỗ trợ).
2. Vercel → Add New → Project → Import Git Repository.
3. Framework Preset: Other; Build Command để trống; Output Directory để trống hoặc `.`.
4. Deploy.

## CẢNH BÁO QUAN TRỌNG
Đây mới là bản đóng gói giao diện HTML gốc để triển khai xem trước. File gốc vẫn dùng LocalStorage, có thông tin Admin mặc định hard-code và chưa kết nối Firebase. Không dùng bản này để nhận tiền/nạp tiền hoặc vận hành shop thật.

Để hoàn thiện bản Firebase + Vercel an toàn cần bổ sung backend API, Firebase Admin SDK, Firestore rules, thiết lập quyền Admin bằng custom claims, cùng biến môi trường trên Vercel. Không đưa Service Account private key vào HTML/GitHub. Cấu hình Firebase Web SDK (apiKey...) không thay thế thông tin xác thực phía máy chủ.
