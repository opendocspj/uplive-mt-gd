---
tags:
  - thu
  - tiennt
---
# Vị trí tính năng
Từ [[Lobby System (Home)]], ấn vào biểu tượng Thư để mở tính năng.
![[20241120101835.png]]
**Video**
![[HTHT-Mail.mp4]]

# Mô tả
![[20241120150005.png]]

| ID  | Detail                       |
| --- | ---------------------------- |
| 1   | Button - Đóng                |
| 2   | Tên UI - **Hòm Thư**         |
| 3   | Trạng thái thư chưa nhận quà |
| 4   | Trạng thái thư đã nhận quà   |
| 5   | Trạng thái đang select thư   |
| 6   | Nội dung thư                 |
| 7   | Quà đính kèm trong thư       |
| 8   | Nút nhận quà của thư đó      |
| 9   | Nhận toàn bộ quà trong thư   |
| 10  | Xóa thư đang select          |
# Loại thư
Thư có 2 loại chính:
1. Thư có đính kèm quà: Có 2 trạng thái nhỏ hơn: đã nhận và chưa nhận quà. 
2. Thư thông báo (không đính kèm quà)
![[20241120150258.png]]

# Cấu trúc thư
## Tiêu đề thư 
Tiêu đề gồm: Tên ở dòng trên và giờ gửi dòng dưới.
![[20241120150806.png]]
## Nội dung thư
### Với thư có quà
Hiển thị nút nhận quà trong nội dung thư.
![[20241120150522.png]]
Nếu người chơi bấm nhận quà, bung ra [[Pop-up thưởng]]
![[20241120150630.png]]
Nút nhận lúc này biến thành nút Xóa, các vật phẩm sẽ có trạng thái đã nhận.
![[20241120150657.png]]

### Với thư hệ thống
Chỉ có nút xóa và nội dung thư.
![[20241120150856.png]]

# Luật Xóa Thư
Thư đã nhận hoặc chưa nhận đều bị **xóa sau 7 ngày** tính từ thời điểm gửi đi.