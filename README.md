# 🎓 LMS AI Assistant

Trợ lý AI hỗ trợ giải câu hỏi và ôn tập trực tiếp trên hệ thống **Canvas Portal** (`portal.uet.vnu.edu.vn`) và **LMS VNU**.

---

## 🚀 Cách cài đặt (Chỉ mất 1 phút)

Do extension phục vụ mục đích cá nhân, bạn cài đặt trực tiếp thông qua chế độ Developer Mode của Chrome:

1. **Mở trang quản lý Tiện ích:**
   - Mở trình duyệt Chrome (hoặc Edge, Cốc Cốc, Brave).
   - Nhập vào thanh địa chỉ: `chrome://extensions/` rồi nhấn **Enter**.
2. **Bật Chế độ nhà phát triển:**
   - Bật công tắc **Developer mode** (ở góc trên cùng bên phải màn hình).
3. **Tải extension vào trình duyệt:**
   - Nhấn vào nút **Load unpacked** (Tải tiện ích đã giải nén) ở góc trên bên trái.
   - Chọn thư mục dự án `LMS-AI-Assistant`.
   - **Xong!** Extension sẽ xuất hiện trên thanh công cụ của trình duyệt.

---

## ⚙️ Hướng dẫn cấu hình (Lần đầu sử dụng)

1. Nhấn vào biểu tượng **LMS AI Assistant** trên thanh công cụ trình duyệt.  
   *(💡 Mẹo: Nhấn nút `[ ↗ ]` ở góc trên bên phải header để mở cài đặt trong một **tab riêng**, tha hồ chuyển tab copy key/model mà không lo popup bị tắt).*
2. **Nhập Endpoint & API Key:**
   - **Endpoint URL:** Nhập base URL API của bạn (mặc định: `http://localhost:20128/v1` nếu dùng 9Router/server local, hoặc URL gateway của bạn).
   - **Chuẩn API:** Để **Tự động phát hiện** (hoặc chọn OpenAI / Anthropic).
   - **API Key / Token:** Dán key của bạn vào.
3. **Bắt & Chọn Model:**
   - Nhấn nút **Kiểm tra kết nối**.
   - Khi kết nối thành công, danh sách model bắt được từ endpoint sẽ tự động hiện ra ngay bên dưới để bạn chọn nhanh (hoặc có thể tự gõ tên model vào ô).
   - Nhấn **Lưu cài đặt**.
   *(Lưu ý: Mọi thay đổi đều được tự động lưu nháp ngay khi bạn gõ, không sợ mất dữ liệu khi đổi tab).*

---

## 🎯 Cách sử dụng trên Canvas Portal

1. Mở bài tập hoặc bài kiểm tra trên **Canvas Portal** (`portal.uet.vnu.edu.vn`).
2. **Hỏi từng câu lẻ:**
   - Bên dưới mỗi câu hỏi sẽ có nút **Hỏi AI**. Nhấn vào để AI phân tích đề và tự động gợi ý/điền đáp án.
3. **Hỏi tất cả (Ask All):**
   - Trên đầu bài thi có thanh công cụ **"Hỏi tất cả"**. Nhấn nút (hoặc bấm `Alt + A`), AI sẽ lần lượt giải từng câu theo nhịp độ tự nhiên.
4. **Xuất đề ôn tập:**
   - Nhấn nút **"Xuất đề (.md)"** trên thanh công cụ để tải toàn bộ đề thi kèm đáp án và lời giải về máy dưới dạng file Markdown để ôn thi cuối kỳ.

---

## ⌨️ Phím tắt nhanh

| Phím tắt | Chức năng |
| :--- | :--- |
| **`Alt + A`** | Tự động hỏi tất cả câu hỏi trên trang |
| **`Alt + C`** | Mở / Đóng khung Chat AI nổi kéo thả |
| **`Alt + Q`** | **Boss Key:** Ẩn / Hiện tức thời toàn bộ dấu vết AI trên trang |

---

## 💡 Các tính năng nổi bật (Tab Tùy chọn)

- 🟢 **Chế độ chấm siêu nhỏ (Micro-Dot):** Thay vì hiện khung giải thích lớn làm biến đổi bố cục câu hỏi, extension chỉ gắn một chấm xanh nhỏ (5px) cạnh đáp án đúng. Người ngoài nhìn vào màn hình sẽ không thấy dấu vết AI. Rê chuột vào chấm để xem giải thích.
- ⏱️ **Nhịp độ nghỉ khi Hỏi tất cả:** Tùy chỉnh nhịp độ ngẫu nhiên giữa các câu (Nhanh 1-2s, Tự nhiên 3-5s, Thong thả 6-9s) để tránh lỗi quá tải API và mô phỏng nhịp đọc đề tự nhiên.
- ✍️ **Tự động điền đáp án:** Tự động click chọn radio/checkbox hoặc điền số vào ô trống sau khi AI giải xong.
- 💾 **Bộ nhớ Cache 24h:** Các câu hỏi đã giải sẽ được lưu cache tự động, hỏi lại không tốn thêm token.

---

> ⚠️ **Lưu ý về Safe Exam Browser (SEB):**  
> Extension hoạt động trơn tru trên mọi bài tập, quiz tuần mở trên trình duyệt Google Chrome thông thường. Đối với các bài thi chính thức bắt buộc sử dụng ứng dụng chuyên dụng *Safe Exam Browser*, bài thi sẽ chạy trong môi trường phần mềm riêng biệt độc lập và không thể can thiệp bằng extension trình duyệt.
