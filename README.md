# 📄 TRÌNH GHÉP ẢNH THÀNH PDF THEO KÍCH THƯỚC GỐC

> **Tác giả:** Dương Tấn Chánh  
> **Nền tảng:** Single-page Web Application (HTML5 / CSS3 / Vanilla JavaScript)  
> **Giấy phép:** MIT License  

---

## 🌟 Giới thiệu

**Trình Ghép Ảnh Thành PDF Theo Kích Thước Gốc** là một công cụ web mã nguồn mở, hoạt động 100% phía trình duyệt (Client-side). Ứng dụng giải quyết triệt để vấn đề ảnh bị méo tỉ lệ hoặc bị chèn viền trắng thừa khi chuyển đổi sang PDF theo các khổ giấy tiêu chuẩn (như A4/Letter). 

Mỗi trang trong file PDF xuất ra sẽ có **kích thước (Pixel) và hướng xoay (Ngang/Dọc) trùng khớp chính xác tuyệt đối với từng bức ảnh gốc**.

---

## ✨ Tính năng nổi bật

- 🎯 **Chuẩn kích thước 1:1 từng trang:** Tự động đọc thông số chiều rộng và chiều cao thực tế của từng ảnh để tạo trang PDF tương ứng. Không viền trắng, không méo hình.
- 🔄 **Linh hoạt xoay trang:** Tự động nhận diện và thiết lập khổ ngang (*Landscape*) hoặc khổ dọc (*Portrait*) độc lập cho từng trang.
- 📥 **3 phương thức nạp ảnh tiện lợi:**
  1. Bấm nút chọn nhiều file từ thiết bị (*hỗ trợ cả PC, Android và iOS*).
  2. Kéo và thả tập tin trực tiếp vào trình duyệt (*Drag & Drop*).
  3. Dán trực tiếp từ bộ nhớ tạm (*Ctrl + V / Paste Clipboard*).
- 🗂️ **Quản lý trang trực quan:** Xem trước ảnh thu nhỏ (thumbnail), xem độ phân giải `WxH`, dung lượng, điều chỉnh thứ tự (lên/xuống/đảo ngược) hoặc xoá từng ảnh.
- 🔒 **Bảo mật & Riêng tư:** Toàn bộ quá trình xử lý diễn ra trực tiếp trong RAM của thiết bị, không tải ảnh lên máy chủ trung gian.
- ⚡ **Hỗ trợ chạy Offline:** Tích hợp sẵn thư viện cục bộ trong thư mục `js/` kết hợp cơ chế dự phòng tự động tải CDN qua Internet.
- 📱 **Tương thích di động (Mobile Responsive):** Giao diện tự động co giãn, bo tròn góc hiện đại, nút bấm tối ưu thao tác cảm ứng trên điện thoại thông minh và máy tính bảng.

---

## 📁 Cấu trúc thư mục

```text
├── index.html              # File giao diện và mã nguồn logic duy nhất
├── js/
│   └── jspdf.umd.min.js    # Thư viện jsPDF (Bản 2.5.1 UMD dùng Offline)
└── README.md               # Tài liệu hướng dẫn dự án
```

---

## 🚀 Hướng dẫn cài đặt và sử dụng

### 1. Chạy trực tiếp trên máy tính (Offline)
1. Tải toàn bộ mã nguồn hoặc clone repository về máy:
   ```bash
   git clone https://github.com/[ten-tai-khoan]/[ten-repo].git
   ```
2. Đảm bảo file `jspdf.umd.min.js` đã nằm trong thư mục `js/`.
3. Nhấp đúp chuột vào file `index.html` để mở bằng trình duyệt web bất kỳ (*Chrome, Edge, Firefox, Safari...*).

### 2. Triển khai miễn phí lên GitHub Pages
1. Đẩy mã nguồn lên kho lưu trữ GitHub của bạn.
2. Vào **Settings** > **Pages**.
3. Tại mục **Branch**, chọn nhánh `main` (hoặc `master`) và thư mục `/root`.
4. Bấm **Save**. Website của bạn sẽ hoạt động trực tuyến qua đường link `https://[ten-tai-khoan].github.io/[ten-repo]/`.

---

## 🛠️ Công nghệ sử dụng

- **HTML5 & Semantic Elements**
- **CSS3:** Biến màu sắc CSS Variables, Bố cục CSS Grid & Flexbox, Đồ hoạ SVG Vector thuần.
- **Vanilla JavaScript (ES6+):** Xử lý bất đồng bộ `Promise` / `async-await`, API `FileReader`, DOM Events.
- **Thư viện bên thứ ba:** [jsPDF v2.5.1](https://github.com/parallax/jsPDF) (Bản quyền MIT).

---

## 👨‍💻 Tác giả

* **Dương Tấn Chánh**
* Mọi đóng góp, báo lỗi hoặc yêu cầu tính năng mới vui lòng mở mục [Issues](https://github.com) trên GitHub.

---

## 📄 Giấy phép (License)

Dự án được phân phối dưới giấy phép **MIT License**. Bạn được toàn quyền sử dụng, chỉnh sửa và tích hợp vào mục đích cá nhân hoặc thương mại.