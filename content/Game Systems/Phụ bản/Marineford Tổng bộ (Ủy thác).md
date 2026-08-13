---
tags:
  - phuban
  - tiennt
  - pve
  - readyUI
---
# Vị trí tính năng
Từ [[Lobby System (Home)]], chọn [[Phụ Bản System]], sau đó chọn Tổng Bộ.

![[HTHT-TongBoPos-ezgif.gif]]

![[20241210151841.png]]

![[20241210162400.png]]

# Mô tả tính năng
![[20241210165242.png]]

| ID  | Giải nghĩa                                                                     |
| --- | ------------------------------------------------------------------------------ |
| 1   | Nút trở về. Bấm vào về lại [[Phụ Bản System]].                                 |
| 2   | Thanh tiền tệ. Gồm [[Kim Cương]], [[Nhiệm Vụ Thường]], [[Nhiệm Vụ Khó]].       |
| 3   | Nút info. Bấm vào bung [[Pop-up]] tỉ lệ nhiệm vụ. **Xem thêm bên dưới**.       |
| 4   | Nút Trợ Giúp. Bấm vào bung [[Pop-up]] trợ giúp. **Xem thêm bên dưới**.         |
| 5   | Đếm ngược thời gian làm mới toàn bộ danh sách 8 nhiệm vụ.                      |
| 6   | Rank nhiệm vụ. Mỗi nhiệm vụ có Rank. **Xem thêm bên dưới**.                    |
| 7   | Thưởng nhiệm vụ. Bấm vào ra [[Tool-tip]].                                      |
| 8   | Trạng thái chưa làm. Thời gian hoàn thành nhiệm vụ. **Xem thêm bên dưới**.     |
| 9   | Trạng thái đang làm. Thời gian hoàn thành nhiệm vụ.                            |
| 10  | Trạng thái hoàn thành. Thời gian hoàn thành nhiệm vụ.                          |
| 11  | Nút khóa nhiệm vụ. **Xem thêm bên dưới**.                                      |
| 12  | Nút hoàn thành nhanh. Trả một lượng [[Kim Cương]] để ngay lập tức hoàn thành.  |
| 13  | Nút hủy bỏ nhiệm vụ. Ấn sẽ bung [[Pop-up]] và xóa bỏ nhiệm vụ này.             |
| 14  | Nút nhận thưởng. Ấn bung [[Pop-up thưởng]].                                    |
| 15  | Nút dùng [[Nhiệm Vụ Thường]]. Spawn ngay 1 nhiệm vụ thường.                    |
| 16  | Nút dùng [[Nhiệm Vụ Khó]]. Spawn ngay 1 nhiệm vụ khó.                          |
| 17  | Nút làm mới. Làm mới danh sách nhiệm vụ. Mỗi nhiệm vụ sẽ mất 10 [[Kim Cương]]. |
| 18  | Background tính năng.                                                          |
  
## [3] Nút Info - Tỉ lệ nhiệm vụ
[[Pop-up]] bung ra:

![[MuMu12-20241210-044127.png]]

Nội dung:
```
Tỉ lệ xuất hiện nhiệm vụ:

1 sao - 25.6%  
2 sao - 27%  
3 sao - 23.2%  
4 sao - 15%  
5 sao - 8%  
6 sao - 1%  
7 sao - 0.2%
```

## [4] Nút Trợ Giúp
[[Pop-up]] bung ra:

![[MuMu12-20241210-044228.png]]

Nội dung:
```
1. Một tướng chỉ có thể làm một nhiệm vụ trong một thời điểm.

2. Mỗi ngày có số nhiệm vụ nhất định, tăng cấp VIP sẽ được thưởng thêm lượt nhiệm vụ.

3. Có thể dùng Kim Cương để làm mới nhiệm vụ. Có thể khóa nhiệm vụ để không bị làm mới. Nếu có nhiệm vụ từ 4 sao trở lên sẽ có cảnh báo.
```

## [6] Rank Nhiệm Vụ
Mỗi nhiệm vụ có một mức rank riêng.

| Rank  | Hình Ảnh                             | Thời Gian Làm | Phân Loại           |
| ----- | ------------------------------------ | :-----------: | ------------------- |
| 7 Sao |                                      |      12h      | [[Nhiệm Vụ Khó]]    |
| 6 Sao | ![[20241211153308.png]] |      10h      | [[Nhiệm Vụ Khó]]    |
| 5 Sao | ![[20241211153353.png]] |      8h       | [[Nhiệm Vụ Khó]]    |
| 4 Sao | ![[20241211153409.png]] |      6h       | [[Nhiệm Vụ Khó]]    |
| 3 Sao | ![[20241211153520.png]] |      4h       | [[Nhiệm Vụ Thường]] |
| 2 Sao | ![[20241211153429.png]] |      2h       | [[Nhiệm Vụ Thường]] |
| 1 Sao | ![[20241211153439.png]] |      1h       | [[Nhiệm Vụ Thường]] |
## [7] Thưởng nhiệm vụ
### Thưởng 1 Sao ★
Random ngẫu nhiên 1 trong số các vật phẩm sau.

| Item               | Số lượng | Tỉ lệ |
| ------------------ | -------- | ----- |
| [[Cốc Bia Thường]] | 1        | 50    |
| [[Kim Cương]]      | 3~4      | 50    |

### Thưởng 2 Sao ★★
Random ngẫu nhiên 1 trong số các vật phẩm sau.

| Item                   | Số lượng | Tỉ lệ |
| ---------------------- | -------- | ----- |
| [[Mảnh Hải Tặc 3 Sao]] | 6~9      | 50    |
| [[Cốc Bia Thường]]     | 2~3      | 50    |
| [[Kim Cương]]          | 5~10     | 50    |
### Thưởng 3 Sao ★★★
Random ngẫu nhiên 1 trong số các vật phẩm sau.

| Item                   | Số lượng | Tỉ lệ |
| ---------------------- | -------- | ----- |
| [[Mảnh Hải Tặc 3 Sao]] | 10~20    | 50    |
| [[Cốc Bia Thường]]     | 3~5      | 50    |
| [[Kim Cương]]          | 11~25    | 50    |
### Thưởng 4 Sao ★★★★
Random ngẫu nhiên 1 trong số các vật phẩm sau.

| Item                   | Số lượng | Tỉ lệ |
| ---------------------- | -------- | ----- |
| [[Mảnh Hải Tặc 4 Sao]] | 5~10     | 50    |
| [[Cốc Bia Vàng]]       | 1~3      | 50    |
| [[Kim Cương]]          | 40~60    | 50    |
| [[Giấy Thách Đấu]]     | 1~2      | 50    |
| [[Xu Vòng Quay]]       | 1~2      | 50    |
### Thưởng 5 Sao ★★★★★
Random ngẫu nhiên 1 trong số các vật phẩm sau.

| Item                   | Số lượng | Tỉ lệ |
| ---------------------- | -------- | ----- |
| [[Mảnh Hải Tặc 4 Sao]] | 11~20    | 50    |
| [[Cốc Bia Vàng]]       | 2~5      | 50    |
| [[Kim Cương]]          | 81~120   | 50    |
| [[Giấy Thách Đấu]]     | 2~4      | 50    |
| [[Xu Vòng Quay]]       | 2~4      | 50    |
### Thưởng 6 Sao ★★★★★★
Random ngẫu nhiên 1 trong số các vật phẩm sau.

| Item               | Số lượng | Tỉ lệ |
| ------------------ | -------- | ----- |
| [[Thuốc Hoán Đổi]] | 30~60    | 50    |
| [[Kim Cương]]      | 150~200  | 30    |

### Thưởng 7 Sao ★★★★★★★
Random ngẫu nhiên 1 trong số các vật phẩm sau.

| Item               | Số lượng | Tỉ lệ |
| ------------------ | -------- | ----- |
| [[Thuốc Hoán Đổi]] | 100~150  | 50    |
| [[Kim Cương]]      | 300~500  | 30    |

## [8] Trạng thái chưa làm
Khi bấm vào nhiệm vụ, [[Pop-up]] để người chơi fill tướng hiện lên.

![[20241211161308.png]]

| ID  | Detail                                                        |
| --- | ------------------------------------------------------------- |
| 1   | Nút đóng.                                                     |
| 2   | Rank nhiệm vụ.                                                |
| 3   | Thưởng nhiệm vụ.                                              |
| 4   | Thời gian hoàn thành nhiệm vụ.                                |
| 5   | Nút hướng dẫn. Bấm bung ra [[Pop-up]]. **Xem thêm bên dưới**. |
| 6   | Vị trí nhét tướng. Bấm để chọn tướng. **Xem bên dưới.**       |
| 7   | Danh sách yêu cầu của nhiệm vụ. **Xem bên dưới.**             |
| 8   | Nút tự động điền tướng. **Xem bên dưới**.                     |
| 9   | Nút bắt đầu nhiệm vụ. Nhiệm vụ chuyển trạng thái.             |
| 10  | Nút bỏ hết nhân vật.                                          |
### [5] Nút hướng dẫn
Bung ra [[Pop-up]] hướng dẫn:

![[MuMu12-20241211-041654.png]]

**Nội dung:**
```
1. Thuyền viên không bị mất khi thực hiện nhiệm vụ.

2. Mỗi thuyền viên chỉ thực hiện một nhiệm vụ tại một thời điểm.
Sau khi nhận phần thưởng, thuyền viên có thể thực hiện các nhiệm vụ khác.
```

### [6] Vị trí nhét tướng
Bấm vào từng ô để bung ra [[Pop-up]] chọn tướng

![[MuMu12-20241211-041853.png]]

Tướng sẽ có trạng thái lựa chọn và không lựa chọn

![[20241211161946.png]]

Nếu đã được lựa chọn, hình ảnh tướng (gồm [[Hệ]] và Cấp) sẽ được hiển thị.

![[20241211162013.png]]

![[HTHT-UyThac-ChonTuong-ezgif.gif]]

### [7] Danh sách yêu cầu nhiệm vụ
Có 2 trạng thái đạt và chưa đạt yêu cầu. 

| Trạng thái       | Hình ảnh                             |
| ---------------- | ------------------------------------ |
| Chưa đạt yêu cầu | ![[20241211162130.png]] |
| Đạt yêu cầu      | ![[20241211162148.png]] |
Các yêu cầu là ngẫu nhiên theo bảng sau

| Rank  | Số Điều Kiện | Số Slot | Điều Kiện                                                      |
| ----- | :----------: | :-----: | :------------------------------------------------------------- |
| 7 Sao |      4       |    4    | 1 Nhân vật từ 5 [[Sao]].<br>Random 1 [[Lớp]] hoặc 1 [[Hệ]] x3. |
| 6 Sao |      4       |    4    | 1 Nhân vật từ 5 [[Sao]].<br>Random 1 [[Lớp]] hoặc 1 [[Hệ]] x3. |
| 5 Sao |      3       |    3    | 1 Nhân vật từ 5 [[Sao]].<br>Random 1 [[Lớp]] hoặc 1 [[Hệ]] x2. |
| 4 Sao |      3       |    3    | 1 Nhân vật từ 4 [[Sao]].<br>Random 1 [[Lớp]] hoặc 1 [[Hệ]] x2. |
| 3 Sao |      2       |    2    | 1 Nhân vật từ 3 [[Sao]]. <br>Random 1 [[Lớp]] hoặc 1 [[Hệ]].   |
| 2 Sao |      2       |    2    | Random 1 [[Lớp]] hoặc 1 [[Hệ]].<br>1 Nhân vật bất kì.          |
| 1 Sao |      1       |    1    | Random 1 [[Lớp]] hoặc 1 [[Hệ]]                                 |

### [8] Nút tự động điền tướng
Khi bấm vào nút tự động, tướng sẽ ngay lập tức được fill vào các trống. Nếu không có tướng phù hợp, hệ thống sẽ hiển thị [[Floating Thông Báo]] "*Không có thuyền viên phù hợp*".

![[HTHT-UyThac-ChonTuongAuto-ezgif.com.gif]]

### [9] Nút bắt đầu nhiệm vụ
Người chơi có thể bắt đầu nhiệm vụ và chuyển trạng thái nhiệm vụ từ chưa làm thành đang làm khi đã đáp ứng đủ các điều kiện.
Nếu chưa đáp ứng đủ, hệ thống bung [[Floating Thông Báo]] "*Thuyền viên không thỏa mãn yêu cầu*"

![[20241211162624.png]]
## [11] Nút khóa nhiệm vụ
Khi bấm vào biểu tượng ổ khóa nhiệm vụ, một [[Pop-up]] sẽ bung ra xác nhận có khóa hay không.

![[MuMu12-20241211-040118.png]]

Lúc này, nhiệm vụ sẽ ở trạng thái khóa.

![[20241211160157.png]]

Khi khóa, nhiệm vụ không bị làm mới khi ấn nút làm mới.
## [12] Nút hoàn thành nhanh
Để hoàn thành nhanh một nhiệm vụ, người chơi có thể trả [[Kim Cương]] để tiến hành. Số lượng Kim Cương tùy thuộc vào thời gian còn lại của nhiệm vụ.

| Thời gian còn lại | [[Kim Cương]] phải trả |
| ----------------- | ---------------------- |
| Dưới 1h           | 1                      |
| Dưới 2h           | 2                      |
| Dưới 4h           | 10                     |
| Dưới 6h           | 20                     |
| Dưới 8h           | 30                     |
| Dưới 10h          | 40                     |
| Trên 10h          | 50                     |
Khi bấm trả, một [[Pop-up]] sẽ hiển thị xác nhận

![[MuMu12-20241211-040938.png]]

## [13] Nút hủy bỏ nhiệm vụ
Khi hủy bỏ nhiệm vụ, [[Pop-up]] sẽ bung ra hỏi người chơi xác nhận hủy bỏ

![[MuMu12-20241211-044239.png]]

Nhiệm vụ sẽ bị **xóa** trong danh sách nhiệm vụ.