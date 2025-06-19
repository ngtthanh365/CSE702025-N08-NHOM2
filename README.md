CSE702025-N08-NHOM2
# GROUP 2: XÂY DỰNG GIAO DIỆN ỨNG DỤNG ĐẶT VÉ XEM PHIM 
## LINK FIGMA: https://www.figma.com/design/0YMDhNtTyNCacMMk3kaMf3/KTPM-LT8-GROUP2?node-id=0-1&t=x2y7rGnXjZ8FhG0L-1
## Giới Thiệu Dự Án
- Ứng dụng Đặt Vé Xem Phim là một giao diện người dùng thân thiện, hiện đại giúp người dùng dễ dàng tìm kiếm rạp chiếu phim, chọn suất chiếu, đặt vé và thanh toán nhanh chóng.
- Dự án này tập trung vào thiết kế giao diện người dùng (UI/UX) trên Figma nhằm mô phỏng trải nghiệm đặt vé trực tuyến như các ứng dụng phổ biến hiện nay.
## Giới thiệu thành viên:
1. **Nguyễn Tuấn Thành**: Phát triển giao diện phần mềm toàn diện.
- MSSV: 23010626
- Email: tuanthanh365bt@gmail.com

2. **Nguyễn Huy Hoàng**: Phát triển giao diện phần mềm toàn diện.
- MSSV: 23010143
- Email: hoang20052810@gmail.com

3. **Nguyễn Đăng Nhật**: Phát triển giao diện phần mềm toàn diện.
- MSSV: 23010629
- Email: nhattnguyenn2005@gmail.com
## Bảng phân chia công việc chi tiết theo tuần:
| Thành viên            | Tuần 1 (Phân tích yêu cầu)                                              | Tuần 2 (Thiết kế Use‑case & Flow)                                           | Tuần 3 (Thiết kế hướng đối tượng)                                                  | Tuần 4 (UI Flow & Prototype)                                   | Tuần 5 (Hoàn thiện & Đánh giá)                                                   |
|-----------------------|---------------------------------------------------------------------------|------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|----------------------------------------------------------------|------------------------------------------------------------------------------------|
| **Nguyễn Tuấn Thành** | - Thu thập yêu cầu<br>- Xác định actors & chức năng chính                 | - Phân tích chức năng theo actor<br>- Vẽ Use‑case diagram<br>- Mô tả chi tiết từng use‑case | - Xác định class chính và thuộc tính<br>- Thiết kế quan hệ giữa các class (UML)     | - Liên kết màn hình, thiết lập điều hướng (Prototype)         | - Tổng hợp phản hồi<br>- Chạy test UI flow<br>- Ghi nhận và sửa lỗi trong prototype |
| **Nguyễn Huy Hoàng**  | - Nghiên cứu người dùng & kịch bản thực tế                                | - Chọn flow diagram (Sequence hoặc Activity)<br>- Vẽ sơ đồ flow              | - Viết đặc tả phương thức các class (method signatures)                             | - Bố trí layout chính, style guide trên Figma                | - Đánh giá ưu/nhược điểm<br>- Ghi nhận lỗi<br>- Đề xuất cải tiến tính năng            |
| **Nguyễn Đăng Nhật**  | - Tham khảo ứng dụng tương tự<br>- Soạn thảo đề bài toán                   | - Chuẩn hóa sơ đồ Use‑case                                                    | - Chuẩn hóa sơ đồ Class                                                              | - Vẽ UI flow diagram (Wireflow)                              | - Viết phần đánh giá<br>- Báo cáo kết quả                                            |
## Phân tích yêu cầu:
### Đặt vấn đề bài toán
Trong bối cảnh nhu cầu giải trí trực tuyến ngày càng cao, việc phát triển một ứng dụng đặt vé xem phim tiện lợi, trực quan và nhanh chóng là thiết yếu. Hệ thống của nhóm chúng tôi cho phép người dùng:
•	Đăng ký / Đăng nhập,
•	Xem danh sách phim, vị trí rạp phim, lịch chiếu, các ưu đãi, 
•	Chọn rạp phim, chỗ ngồi, mua bỏng-nước, 
•	Thanh toán và nhận vé điện tử.
Mục tiêu là tối ưu trải nghiệm người dùng, giảm thiểu thao tác thừa và đảm bảo tính ổn định, bảo mật.
### Tác nhân, người dùng
| Tác nhân                    | Mô tả                                                    |
|-----------------------------|-----------------------------------------------------------|
| **Khách hàng (User)**       | Đăng ký/Đăng nhập, duyệt phim, đặt vé                     |
| **Quản trị viên (Admin)**   | Quản lý danh sách phim, rạp phim, lịch chiếu, doanh thu   |
### Chức năng & Phân tích chức năng (theo tác nhân)
•	Khách hàng (User)
1.	Đăng ký / Đăng nhập
2.	Xem danh sách phim: Theo thể loại, ngày chiếu,…
3.	Xem chi tiết phim: Mô tả, trailer, đánh giá
4.	Chọn rạp phim, vị trí rạp phim, xem mô tả rạp
5.	Chọn lịch chiếu
6.	Chọn chỗ ngồi
7.	Thanh toán
8.	Nhận vé điện tử: qua app
•	Quản trị viên (Admin)
1.	Quản lý phim: Thêm/sửa/xóa phim
2.	Thiết lập rạp phim
3.	Thiết lập lịch chiếu
4.	Quản lý đặt vé: Xem doanh thu, hủy vé
5.	Quản lý người dùng
3. Đặc tả và thiết kế
## 3.1. Use case + Mô tả
### 3.1.1 Mô tả
1.	UC1: Đăng ký/Đăng nhập
•	Actor: User
•	Mô tả: Cho phép user tạo tài khoản mới hoặc đăng nhập để thực hiện đặt vé.
2.	UC2: Duyệt phim
•	Actor: User
•	Mô tả: Xem danh sách phim, tìm theo thể loại, từ khóa.
3.	UC3: Đặt vé
•	Actor: User
•	Mô tả: Chọn rạp phim, lịch chiếu, chỗ ngồi, thanh toán và nhận vé.
4.	UC4: Quản lý phim
•	Actor: Admin
•	Mô tả: Thực hiện CRUD phim và lịch chiếu.
### 3.1.2. Sơ đồ diagram Use-case User:
![Screenshot (330)](https://github.com/user-attachments/assets/44e9112a-65c2-4595-bb19-9f3b47160646)

