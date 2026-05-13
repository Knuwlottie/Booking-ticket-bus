# 🚌 Bus Ticket System

Ứng dụng Java desktop đặt vé xe buýt, hỗ trợ giao diện thân thiện, mã hóa mật khẩu, tạo hóa đơn PDF và biểu đồ doanh thu.

---

## 🛠 Công nghệ sử dụng

- **Java Swing** + FlatLaf (giao diện hiện đại)
- **SQL Server** (quản lý CSDL)
- **BCrypt** (mã hóa mật khẩu người dùng)
- **iTextPDF** (in hóa đơn PDF)
- **JFreeChart** (biểu đồ doanh thu)
- **JDBC Driver** (kết nối SQL Server)

---

## 📂 Cấu trúc dự án

```
Busticketsystem/
├── lib/               ← Các file thư viện .jar cần thiết
├── src/               ← Mã nguồn Java (controller, model, view, dao, ...)
├── datavexe.sql       ← Script tạo CSDL (import bằng SSMS)
├── README.md          ← File hướng dẫn này
├── .gitignore
└── Busticketsystem.iml (dành cho IntelliJ IDEA)
```

---

## ▶️ Hướng dẫn chạy

### ✅ Yêu cầu:
- JDK 11 trở lên
- IntelliJ IDEA (khuyên dùng) hoặc NetBeans
- SQL Server + SSMS

### ✅ Các bước:
1. **Clone repo:**
```bash
https://github.com/Knuwlottie/Booking-ticket-bus.git
```

2. **Mở bằng IntelliJ IDEA** → Chọn thư mục `Busticketsystem`

3. **Thêm thư viện:**
    - Vào `File > Project Structure > Libraries`
    - Thêm tất cả `.jar` trong thư mục `lib/`

4. **Kết nối CSDL:**
    - Mở SQL Server Management Studio
    - Tạo database mới: `QuanLyVeXe`
    - Mở file `datavexe.sql` → Nhấn `F5` để chạy

5. **Chạy chương trình:**
    - Tìm và chạy file `Main.java` (thường nằm trong `main` package)

---

## 🔑 Thông tin JDBC mẫu (nếu cần chỉnh sửa trong code)

```java
String connectionUrl = "jdbc:sqlserver://localhost:1433;databaseName=QuanLyVeXe;user=YOUR_USERNAMEa;password=YOUR_PASSWORD;";
```

---

## 💡 Ghi chú

- Nếu chương trình không nhận thư viện, hãy kiểm tra lại phần **Project Libraries**
- Nếu lỗi kết nối SQL, kiểm tra tên database, port SQL Server, và tài khoản

---

## 📬 Liên hệ

> 👤 Tác giả: **Huỳnh Lê Khả NHư**  
> 📫 Email: huynhlekhanhu.kg@gmail.com

