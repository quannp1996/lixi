# 🎉 Lucky Draw - Bốc Thăm Lì Xì

Một trang web tương tác với theme **Tết** - bốc thăm câu hỏi lì xì với hiệu ứng cây đào rung rinh!

## 🌟 Tính Năng Chính

### 📝 Phần Quản Lý Câu Hỏi (Admin)
- ✅ Thêm câu hỏi không giới hạn
- ✅ Mỗi câu hỏi có 4 đáp án để chọn
- ✅ Chỉ định 1 đáp án đúng
- ✅ Tùy chỉnh lời chúc khi trả lời đúng
- ✅ Xem danh sách tất cả câu hỏi
- ✅ Xóa câu hỏi không cần thiết
- ✅ Lưu trữ dữ liệu trên trình duyệt (localStorage)

### 🎮 Phần Chơi Game (Game)
- 🎄 Cây đào đẹp mắt với hiệu ứng cây xanh
- 🧧 Phong bao lì xì được sắp xếp trên cây theo số thứ tự
- ❌ Phong bao đã mở sẽ mờ đi và không thể bấm lại
- 📋 Popup hiển thị câu hỏi và 4 đáp án
- 🎯 Kiểm tra đáp án ngay lập tức
- ✨ Hiệu ứng confetti khi trả lời đúng
- 💌 Hiển thị lời chúc tùy chỉnh
- 📊 Thống kê trúng/sai

### 🌸 Hiệu Ứng Đặc Biệt
- 🌺 Hoa đào rơi liên tục trên cây
- ✨ Confetti animation khi trả lời đúng
- 🎨 UI theme Tết đỏ vàng tươi sáng
- 📱 Responsive design - dùng được trên mobile

## 🚀 Cách Sử Dụng

### Bước 1: Mở trang web
Mở file `index.html` trong trình duyệt (hoặc dùng Live Server)

### Bước 2: Thêm Câu Hỏi (Tab Quản Lý)
1. Chuyển sang tab **"⚙️ Quản Lý Câu Hỏi"**
2. Nhập câu hỏi
3. Nhập 4 đáp án
4. Chọn đáp án đúng từ dropdown
5. Nhập lời chúc nếu trả lời đúng
6. Click **"➕ Thêm Câu Hỏi"**

**Ví dụ:**
```
Câu hỏi: Năm nay là năm con gì?
Đáp án 1: Con Rồng
Đáp án 2: Con Rắn
Đáp án 3: Con Ngựa
Đáp án 4: Con Dê

Đáp án đúng: Con Rồng

Lời chúc: "🎆 Chúc bạn năm mới an khang thịnh vượng!"
```

### Bước 3: Chơi Game (Tab Chơi Game)
1. Chuyển sang tab **"🎮 Chơi Game"**
2. Bấm vào phong bao lì xì bất kỳ (những cái có số)
3. Đọc câu hỏi và chọn đáp án
4. Click **"Nộp Câu Trả Lời"**
5. Xem kết quả - có lời chúc nếu trúng!
6. Tiếp tục bấm các phong bao khác

## 💾 Lưu Trữ Dữ Liệu
- Tất cả câu hỏi được lưu trong **localStorage** của trình duyệt
- Không cần server hay database
- Dữ liệu vẫn lưu lại khi đóng trình duyệt
- Để xóa dữ liệu: Xóa cache/storage trình duyệt hoặc dùng DevTools

## 📂 Cấu Trúc Thư Mục
```
LuckyDraw/
├── index.html          # Trang chính
├── css/
│   └── styles.css      # Tất cả CSS styling
├── js/
│   ├── data.js         # Quản lý dữ liệu (localStorage)
│   ├── admin.js        # Logic admin panel
│   ├── game.js         # Logic game chính
│   └── main.js         # Navigation và khởi tạo
└── README.md           # File này
```

## 🎨 Tùy Chỉnh

### Thay đổi màu sắc
Mở `css/styles.css` và chỉnh `--primary-color`, `--success-color` trong `:root`

### Thay đổi số lượng phong bao
Trong `js/game.js`, tìm dòng:
```javascript
this.envelopesCount = Math.max(questions.length, 6);
```
Thay `6` thành số phong bao mong muốn

### Thay đổi hiệu ứng hoa đào
Tùy chỉnh trong `game.js` - hàm `createFallingPetals()`

## 🔧 Yêu Cầu Hệ Thống
- Trình duyệt hiện đại (Chrome, Firefox, Safari, Edge)
- JavaScript bật
- Không cần cài đặt gì thêm

## 📝 Ghi Chú
- Dữ liệu được lưu trên mỗi trình duyệt/thiết bị khác nhau
- Để backup: Dùng export/import từ DevTools
- Mobile: Trang được tối ưu cho mobile (responsive)

## 🎯 Ý Tưởng Nâng Cao
- Thêm import/export CSV
- Thêm timer cho mỗi câu hỏi
- Thêm difficulty levels
- Thêm multiplayer
- Tích hợp nhạc Tết

---

**Chúc bạn thành công! Tết vui vẻ! 🎆🧧🎉**
