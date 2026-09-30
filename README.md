 Hệ thống Quản lý Bán hàng & Truy vấn Đám mây (Cloud Database)

Ứng dụng Web Full-stack quản lý bán hàng toàn diện được phát triển cho dự án môn học Cơ sở dữ liệu Đám mây. Hệ thống sử dụng **Google Firebase Firestore** làm cơ sở dữ liệu NoSQL trên mây và giao diện tương tác trực quan viết bằng HTML5, CSS3, JavaScript.

---

 Thành viên nhóm (Nhóm 2 - Lớp 12A1 SenTia School)
* Đặng Hiền Anh[cite: 6]
* Lê Nam Khánh[cite: 6]
* Quách Hoàng Lâm[cite: 6]

---

 Tính năng chính của hệ thống

Hệ thống quản lý đồng thời **4 bảng (Collections)** trên cơ sở dữ liệu đám mây:
1. **Quản lý Sản phẩm (`products`)**: Thêm mới, hiển thị danh sách sản phẩm và giá tiền[cite: 4].
2. **Quản lý Đơn hàng (`orders`)**: Tạo đơn hàng, cập nhật thông tin (Sửa), xóa đơn hàng và quản lý chi tiết giao dịch[cite: 4].
3. **Quản lý Khách hàng (`users`)**: Lưu trữ thông tin định danh và email liên hệ của khách hàng[cite: 4].
4. **Quản lý Danh mục (`categories`)**: Phân loại nhóm hàng hóa kèm mô tả chi tiết[cite: 4].

 5 Thuật toán Truy vấn & Thống kê Nâng cao:
* **Truy vấn 1:** Lọc danh sách đơn hàng theo mã/tên người dùng cụ thể[cite: 4].
* **Truy vấn 2:** Đếm số lượng đơn hàng phát sinh theo từng ngày[cite: 4].
* **Truy vấn 3:** Thống kê tổng số lượng sản phẩm đã bán ra[cite: 4].
* **Truy vấn 4:** Tự động khớp giá sản phẩm để tính tổng doanh thu toàn hệ thống (quy đổi định dạng VNĐ)[cite: 4].
* **Truy vấn 5:** Lọc và truy xuất dữ liệu đơn hàng theo khoảng thời gian tùy chọn (`Start Date` đến `End Date`)[cite: 4].

---

 Công nghệ sử dụng
* **Frontend:** HTML5, CSS3 (Grid & Flexbox Layout), JavaScript (ES6+).
* **Backend & Database:** Google Firebase Firestore (Modular SDK v10.8.0).
* **Mô hình kiến trúc:** Client-Server / Cloud Database (DBaaS).

---
 Cấu trúc Cơ sở dữ liệu (ERD Model)

Hệ thống thiết kế gồm 4 thực thể liên kết logic với nhau:
* `USERS` (1) ──< `ORDERS` (N): Quản lý lịch sử mua hàng của khách[cite: 4].
* `CATEGORIES` (1) ──< `PRODUCTS` (N): Phân loại nhóm sản phẩm[cite: 4].
* `PRODUCTS` (1) ──< `ORDERS` (N): Sản phẩm xuất hiện trong các giao dịch đơn hàng[cite: 4].

---
 Hướng dẫn Cài đặt & Chạy ứng dụng

1. **Clone hoặc tải mã nguồn** về máy tính của bạn.
2. Mở file mã nguồn (ví dụ: `hankhl.html` hoặc đổi tên thành `index.html`) bằng một trình duyệt web bất kỳ (Chrome, Edge, Safari,...).
3. Đảm bảo máy tính có kết nối **Internet** để ứng dụng có thể kết nối thành công với cụm cơ sở dữ liệu Google Firebase Firestore đã được cấu hình sẵn trong mã nguồn.
4. Thao tác trực tiếp trên giao diện Dashboard để thêm, sửa, xóa dữ liệu hoặc bấm chạy các nút truy vấn nâng cao!
