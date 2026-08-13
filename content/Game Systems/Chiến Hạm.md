---
tags:
  - tiennt
  - readyUI
---
# Vị trí tính năng
Từ [[Lobby System (Home)]], chọn biểu tượng Chiến Hạm 

![[20250106110847.png]]

# Mô tả tính năng
![[20250106111350.png]]

| ID  | Detail                                           |
| --- | ------------------------------------------------ |
| 1   | Nút quay lại, bấm sẽ về [[Lobby System (Home)]]. |
| 2   | Thanh tiền tệ: [[Beli]], [[Gỗ]], [[Kim Loại]].   |
| 3   | Nút Hướng Dẫn. Bấm ra [[Pop-up]].                |
| 4   | Banner 1 chiến hạm.                              |
| 5   | Nút xem info chiến hạm.                          |
| 6   | Tên chiến hạm.                                   |
| 7   | Nút nâng cấp. **Xem thêm bên dưới**.             |
| 8   | Sang trang mới khi có nhiều hơn 3 thuyền.        |
| 9   | Background tính năng.                            |
| 10  | Số lượng tab.                                    |
| 11  | Tính năng Nội Thất.                              |
| -   | Danh sách chiến hạm trong game                   |
## [3] Nút Hướng Dẫn
Bấm vào sẽ bung ra [[Pop-up]].

![[MuMu12-20250105-231745.png]]

**Nội dung**
```
1. Chọn Chiến Hạm để kích hoạt và mang vào trong trận đánh. Mỗi Chiến Hạm có 1 kĩ năng chủ động và 4 kĩ năng bị động tăng sức mạnh cho tướng. Kĩ năng bị động sẽ cộng thêm chỉ số cho tất cả thuyền viên khi chiến hạm tham chiến cùng trận đấu đó.

2. Nâng cấp bằng Beli, gỗ, sắt. Gỗ và sắt có thể nhận được trong Đảo Trời, vượt ải và Sự Kiện.

3. Trong trận đánh, kĩ năng chủ động của Chiến Hạm sẽ cần năng lượng để sử dụng. Năng lượng này có được khi mỗi tướng ra kĩ năng và khi thanh năng lượng này đầy thì chiến hạm sẽ tự động xuất kĩ năng chủ động.

4. Bạn có thể tái lập lại chiến xa về trạng thái ban đầu và được nhận lại toàn bộ nguyên liệu gỗ, sắt đã dùng để nâng cấp nhưng Beli sẽ không được hoàn trả.
```

## [4] Banner một chiến hạm
Mỗi chiến hạm sẽ có 1 Animation Idle tương ứng.

![[HTHT-ChienHam-Banner-ezgif.gif]]
## [5] Nút xem info chiến hạm
Bấm vào sẽ bung ra [[Pop-up]] xem trước sức mạnh của chiến hạm. 
Mọi thông tin ghi ở đây là **sức mạnh cao nhất** của chiến hạm đó.

![[MuMu12-20250105-232018.png]]

Ấn giữ vào từng biểu tượng sẽ bung ra [[Tool-tip]].

![[HTHT-ChienHam-Tooltip-ezgif.gif]]

## [7] Nút nâng cấp
Người chơi phải mua chiến hạm mới hiện ra nút nâng cấp. 
Nếu chưa mua chiến hạm, nút nâng cấp chuyển thành nút mua chiến hạm. 

![[MuMu12-20250107-031605.png]]

Khi ấn mua, nút sẽ chuyển thành nâng cấp

![[MuMu12-20250107-031631.png]]

Bấm vào sẽ bung ra [[Pop-up]] nâng cấp Chiến Hạm. Nền Background tối đi.

![[20250106113129.png]]

| ID  | Detail                                                           |
| --- | ---------------------------------------------------------------- |
| 1   | Thanh tiền tệ: [[Beli]], [[Gỗ]], [[Kim Loại]].                   |
| 2   | Nút đóng.                                                        |
| 3   | Tab Cấp Độ. (Tab hiện tại).                                      |
| 4   | Tab Kĩ Năng. Xem thêm bên dưới.                                  |
| 5   | Tab Nội Tại. Xem thêm bên dưới.                                  |
| 6   | Banner Chiến hạm.                                                |
| 7   | Nút Tái Tạo. Bấm để trả chiến hạm về Level 1. Xem thêm bên dưới. |
| 8   | Tên Chiến Hạm.                                                   |
| 9   | Level Chiến Hạm.                                                 |
| 10  | Nút nâng cấp chiến hạm. Biến mất khi đạt max.                    |
| 11  | Phẩm Chiến Hạm. Giống [[Phẩm]] tướng.                            |
| 12  | Tài nguyên nâng cấp kế tiếp: [[Beli]], [[Gỗ]].                   |
| 13  | Mô tả kĩ năng của Chiến Hạm.                                     |
### [6] Banner Chiến hạm
Mặc định có animation Idle

![[HTHT-Banner-ShipInside-ezgif.com.gif]]

### [7] Nút Tái Tạo
Bấm sẽ bung ra [[Pop-up]].

![[MuMu12-20250107-031953.png]]

Ấn vào Tái Tạo:
- TH 1: nếu người chơi đã ở cấp 1 thì bung ra [[Floating Thông Báo]] "Chiến Hạm đã ở cấp thấp nhất."
- TH 2: nếu người chơi đã nâng cấp thì bung ra [[Pop-up]] hoàn trả [[Gỗ]]. 

![[MuMu12-20250107-032112.png]]

### [10+11] Nút nâng cấp chiến hạm + Phẩm Chiến Hạm
Cứ **30 cấp độ** sẽ phải **đột phá** để **tăng 1 phẩm**.

![[HTHT-NangCapTangPham-ezgif.gif]]

### [4] Tab Kĩ Năng
![[20250106114135.png]]

| ID  | Detail                                                          |
| --- | --------------------------------------------------------------- |
| 1-8 | Xem bên trên.                                                   |
| 9   | Stats chiến hạm.                                                |
| 10  | Biểu tượng kĩ năng chiến hạm.                                   |
| 11  | Cấp độ kĩ năng chiến hạm.                                       |
| 12  | Kĩ năng chưa học ở trạng thái xám                               |
| 13  | Tài nguyên cần để **nâng cấp kĩ năng**: [[Beli]], [[Kim Loại]]. |
| 14  | Nút nâng cấp.                                                   |
#### [9] Stats chiến hạm
**Gồm:**
1. Máu
2. Tấn công
3. Sát thương chí mạng
4. Tốc độ
5. Chí mạng

![[20250108144857.png]]

Nếu có nhiều stats hơn thì sẽ tiếp tục thêm 1 ô.

#### [10] Biểu tượng kĩ năng chiến hạm
Mỗi chiến hạm có **4 biểu tượng kĩ năng dùng chung**.

![[20250108145145.png]]

#### [14] Nút nâng cấp

| Trạng thái            | Hình Ảnh                             |
| --------------------- | ------------------------------------ |
| Chưa mở khóa          | ![[20250108145555.png]] |
| Có thể nâng cấp       | ![[20250108145549.png]] |
| Nâng cấp đạt giới hạn | ![[20250108145605.png]] |

### [5] Tab Nội Tại
Mở khóa khi người chơi nâng cấp toàn bộ 4 kĩ năng của Chiến Hạm lên **level max**.

| Trạng thái       | Hình Ảnh                        |
| ---------------- | ------------------------------- |
| **Chưa mở khóa** | ![[MuMu12-20250108-025628.png]] |
| **Mở khóa**      | ![[MuMu12-20250108-025721.png]] |

## [11] Tính năng Nội Thất
Tính năng này sẽ bổ sung sau.

## [-] Danh sách chiến hạm trong game
Tổng cộng gồm 6 chiến hạm.

![[MuMu12-20250108-052600.png]]

![[MuMu12-20250108-052605.png]]

| Tên            | Hình Ảnh            | Kĩ năng                                                                                                                                  |
| -------------- | ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Thousand Sunny | ![[Shiphome_2.png]] | Gây sát thương lên 5 kẻ địch ngẫu nhiên và có tỉ lệ gây choáng chúng. Tăng cho 5 đồng minh ngẫu nhiên sát thương chuẩn.                  |
| Germa 66       | ![[Ship_6.png]]     | Gây sát thương lên 5 kẻ địch ngẫu nhiên, giảm thủ và tốc của chúng. Tăng 5 đồng minh ngẫu nhiên công.                                    |
| Perfume Yuda   | ![[Shiphome_3.png]] | Gây sát thương lên 5 kẻ địch ngẫu nhiên. Hồi máu cho 5 đồng minh ngẫu nhiên, tăng thủ và công.                                           |
| Snapper Head   | ![[Shiphome_4.png]] | Gây sát thương lên 5 kẻ địch ngẫu nhiên và câm lặng chúng. Đồng thời, hồi nộ cho 5 đồng minh ngẫu nhiên.                                 |
| Red Force      | ![[Shiphome_1.png]] | Gây sát thương lên 5 kẻ địch ngẫu nhiên, gây thêm sát thương mỗi vòng. Tăng sát thương cho 5 đồng minh dựa trên sát thương kẻ địch nhận. |
| Sexy Foxy      | ![[Ship_5.png]]     | Gây sát thương lên 5 kẻ địch ngẫu nhiên và hóa đá chúng. Tăng sát thương chí mạng cho 5 đồng minh ngẫu nhiên.                            |
Khi mở khóa chiến hạm, người chơi có thể chọn chiến hạm trong danh sách [[Chuẩn Bị Đội Hình]].

![[20250108173348.png]]

Bấm vào sẽ bung ra [[Pop-up]] chọn chiến hạm.

![[MuMu12-20250108-053405.png]]

Ở trong [[Battle System]], khi người chơi mở khóa chiến hạm sẽ có thêm một thanh nộ.

![[20250108173515.png]]

Khi đầy thanh nộ, chiến hạm sẽ tung ra kĩ năng tương ứng.

![[HTHT-ChienHamBattle.mp4]]