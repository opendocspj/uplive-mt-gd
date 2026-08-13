---
tags:
  - tiennt
  - readyUI
---
# Vị trí tính năng
Từ màn hình [[Lobby System (Home)]], chọn biểu tượng bạn bè.

![[20241225100313.png]]

# Mô tả tính năng
![[20241225135834.png]]

| ID  | Detail                                                             |
| --- | ------------------------------------------------------------------ |
| 1   | Nút đóng. Bấm vào đóng Pop-up.                                     |
| 2   | Danh sách bạn. Có ghi số lượng bạn hiện tại/giới hạn.              |
| 3   | **Phần này bỏ**.                                                   |
| 4   | Nút gửi và nhận nhanh. Bấm vào sẽ gửi và nhận hết quà từ mọi người |
| 5   | Avatar của người chơi khác.                                        |
| 6   | Level của người chơi khác.                                         |
| 7   | Tên của người chơi.                                                |
| 8   | Thời gian online cuối cùng của họ.                                 |
| 9   | Nút so tài.                                                        |
| 10  | Nút gửi quà. Trạng thái đã gửi.                                    |
| 11  | Nút gửi quà. Trạng thái chưa gửi.                                  |
| 12  | Nút nhận quà.                                                      |
| 13  | Tab danh sách bạn bè. Chính là tab hiện tại.                       |
| 14  | Tab Kết Bạn.                                                       |
| 15  | Tab Lời Mời Kết Bạn.                                               |
| 16  | Tab Trinh Thám.                                                    |

## [2] Danh sách bạn
Một người chỉ có giới hạn 70 người bạn.

## [4] Nút gửi và nhận nhanh
Tự động gửi và nhận toàn bộ quà từ người chơi khác.
Nếu có quà về sẽ hiển thị [[Pop-up thưởng]].

## [5] Avatar của người chơi khác
Bấm vào sẽ bung ra info đội hình của người chơi đó.

![[20241225141830.png]]

| ID  | Detail                         |
| --- | ------------------------------ |
| 1   | Nút đóng.                      |
| 2   | Cấp người chơi.                |
| 3   | Avatar.                        |
| 4   | ID người chơi.                 |
| 5   | Tên hạm đội.                   |
| 6   | Lực chiến                      |
| 7   | [[Đội hình thủ]].              |
| 8   | Nút xóa bạn. **Xem bên dưới**. |
| 9   | Nút gửi thư. **Xem bên dưới**. |
### [8] Nút Xóa Bạn
Bung ra [[Pop-up]] xác nhận. Nếu ấn xác nhận thì sẽ xóa bạn bè với người chơi đó.

![[MuMu12-20241225-022040.png]]

### Nút Gửi Thư
Ấn vào bung [[Pop-up]] gửi thư.
Phần ID người nhận không thể sửa, chỉ có thể sửa phần nội dung thư.

![[MuMu12-20241225-022111.png]]

Không thể gửi thư trống, hệ thống sẽ hiện ra [[Floating Thông Báo]]: "**Nội dung mail trống**!".

![[MuMu12-20241225-022204.png]]

Khi ấn gửi thành công, hiển thị [[Floating Thông Báo]]: "**Gửi thư thành công**".

![[20241225142310.png]]
## [9] Nút so tài
Khi ấn, hiển thị [[Chuẩn Bị Đội Hình]]. Ấn tấn công sẽ vào [[Battle System]] như bình thường.
Đội hình của người chơi kia chính là [[Đội hình thủ]].

![[MuMu12-20241225-022336.png]]

## [10] Nút gửi quà
Nút này có 2 trạng thái:
1. Đã gửi ![[20241225142435.png]]
2. Chưa gửi ![[20241225142442.png]]
Người nhận sẽ nhận 1x[[Mảnh Hải Tặc 4 Sao]].
Người gửi không mất gì.
Khi ấn gửi, nút sẽ chuyển trạng thái từ chưa gửi thành đã gửi. 

## [12] Nút nhận quà
Nút này có 2 trạng thái:
1. Chưa nhận ![[20241225142629.png]]
2. Đã nhận ![[20241225142708.png]]
Người chơi nhận 1x [[Mảnh Hải Tặc 4 Sao]]. Bung [[Pop-up thưởng]].
Khi nhận xong, nút nhận chuyển trạng thái từ chưa nhận thành đã nhận.
## [14] Tab Kết Bạn
![[20241225143636.png]]

| ID    | Detail                          |
| ----- | ------------------------------- |
| 1     | Nút đóng.                       |
| 2     | Tên [[Pop-up]].                 |
| 3     | Khu vực nhập ID bạn bè.         |
| 4     | Nút kết bạn.                    |
| 5     | Nút làm mới danh sách người lạ. |
| 6     | Avatar người chơi lạ.           |
| 7     | Level người chơi lạ.            |
| 8     | Tên người chơi lạ.              |
| 9     | Nút gửi lời mời kết bạn.        |
| 10-13 | Như trên                        |
### [3] Khu vực nhập ID bạn bè
Người chơi nhập ID bạn bè vào khu vực để tìm chính xác người chơi.
Phần này không thể nhập chữ. Hệ thống không ghi nhận kí tự là chữ.

### [4] Nút kết bạn
Khi người chơi nhập ID người chơi khác thì nút này mới có thể bấm được.
Nếu nhập sai ID thì hiển thị [[Floating Thông Báo]] "Người chơi không tồn tại"

![[20241225145240.png]]

Nhập đúng ID thì hiển thị [[Floating Thông Báo]] "Gửi lời mời kết bạn thành công".

### [5] Nút làm mới danh sách người lạ
Hệ thống ngẫu nhiên xổ ra 15 người lạ có online trong 24 giờ gần nhất trong server.
Không có countdown.
### [9] Nút gửi lời mời kết bạn
Bấm vào thì thông tin của người lạ sẽ biến mất và hiển thị [[Floating Thông Báo]]: "Gửi yêu cầu kết bạn thành công"

![[20241225145431.png]]
Người chơi nhận được yêu cầu kết bạn sẽ hiển thị thông tin trong [15] Tab Lời mời kết bạn.
## [15] Tab Lời Mời Kết Bạn
![[20241225145641.png]]

| ID  | Detail                          |
| --- | ------------------------------- |
| 1   | Nút đóng.                       |
| 2   | Tên tab.                        |
| 3   | Số lượng người yêu cầu kết bạn. |
| 4   | Xóa tất cả lời mời kết bạn.     |
| 5   | Avatar người chơi.              |
| 6   | Level người chơi.               |
| 7   | Tên người chơi.                 |
| 8   | Nút đồng ý.                     |
| 9   | Nút xóa lời mời kết bạn.        |
Khi bấm vào đồng ý kết bạn, có 2 khả năng xảy ra.
1. Thành công. Hiển thị [[Floating Thông Báo]]: "Kết bạn thành công". Và xóa người đó khỏi danh sách.
2. Thất bại. Hiển thị [[Floating Thông Báo]] lỗi tương ứng. VD: "Danh sách bạn bè của người chơi này đã đầy". 

## [16] Tab Trinh Thám
![[20241225150007.png]]

| ID  | Detail             |
| --- | ------------------ |
| 1   | Nút đóng.          |
| 2   | Tên Tab.           |
| 3   | Banner trinh thám. |
| 4   | Nút info.          |
| 5   | Nút trinh thám.    |
### [4] Nút Info
Người chơi bấm sẽ hiển thị [[Pop-up]] hướng dẫn.
Game mình sẽ **bỏ tỉ lệ gặp boss**.

![[MuMu12-20241225-030120.png]]

**Nội dung:**
```
Mỗi 8 giờ sẽ có một lượt trinh thám, mỗi lần trinh thám có xác suất nhận được các vật phẩm và nguyên liệu.
```

### [5] Nút trinh thám
Khi bấm nút Trinh Thám, animation ở Banner sẽ chạy và bung ra [[Pop-up thưởng]].

![[HTHT-TrinhThamButton.mp4]]

Danh sách phần thưởng theo bảng sau

| Vật phẩm         | Số lượng      | Tỉ lệ |
| ---------------- | ------------- | ----- |
| [[Beli]]         | 6~8h rate AFK | 20    |
| [[Beli]]         | 3~4h rate AFK | 50    |
| [[Beli]]         | 1~2h rate AFK | 100   |
| [[Bụi Ma Thuật]] | 6~8h rate AFK | 20    |
| [[Bụi Ma Thuật]] | 3~4h rate AFK | 50    |
| [[Bụi Ma Thuật]] | 1~2h rate AFK | 100   |
| [[Kim Cương]]    | 10~30         | 20    |
