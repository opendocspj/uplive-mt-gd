---
tags:
  - phuban
  - tiennt
  - pve
  - readyUI
---
# Vị trí tính năng
Từ [[Lobby System (Home)]], chọn [[Phụ Bản System]], sau đó chọn Đảo Trời.

![[20241210151841.png]]

![[20241223160303.png]]

# Mô tả tính năng
![[20241223171712.png]]

| ID  | Giải nghĩa                                                           |
| --- | -------------------------------------------------------------------- |
| 1   | Nút trở về. Bấm vào về [[Lobby System (Home)]]                       |
| 2   | Thanh tiền tệ: [[Beli]], [[Kim Cương]], Vỏ Ốc Sên, [[Đá Công Trình]] |
| 3   | Nút hướng dẫn. Bấm ra [[Pop-up]], **xem bên dưới.**                  |
| 4   | Background tính năng.                                                |
| 5   | Công trình của Thảo Khấu. **Xem thêm bên dưới**.                     |
| 6   | Thời gian Reset. Xem bên dưới.                                       |
| 7   | Tên công trình.                                                      |
| 8   | Bóng thoại thu hoạch. Bấm sẽ bung [[Pop-up thưởng]].                 |
| 9   | Nút Càn Quét. Tiêu hao Vỏ Ốc Sên để càn quét 1 công trình thảo khấu. |

## [3] Nút Hướng Dẫn
Bấm vào ra [[Pop-up]] như bên dưới

![[MuMu12-20241223-053817.png]]

**Nội dung:**
```
1. Nâng cấp thành chính để mở khóa và tăng cấp các nhà, tăng số lượng mỏ được khai thác.

2. Khoa Kỹ để nâng cấp "Công" và "Máu" chỉ tác dụng cho các tướng khi đi đánh sơn tặc trong đảo trời.

3. Nâng cấp thành chính sẽ nâng độ khó của boss và hải tặc.
```

## [4] Background tính năng
Bản đồ đảo trời trong game gồm 2 khu vực chính:
- Khu vực A: Chỗ này để các công trình Thảo Khấu, Quái, Boss.
- Khu vực B: Chỗ này để các công trình người chơi.

![[20241223175626.png]]

Xem vị trí tương đối trong **video** dưới đây:

![[HTHT-DaoTroiBGMap.mp4]]

Ban đầu là một vùng đảo có mây mù che phủ. Khi mở **đến chỗ nào thì mây sẽ tan** đi đến đó.

![[20241223174400.png]]

![[20241223174446.png]]

2 Trạng thái - bao phủ và mở ra. 
Theo từng cấp độ nhà chính, mây sẽ mở dần ra các công trình bên dưới.

## [5] Công trình của Thảo Khấu
Các loại công trình của Thảo Khấu và trạng thái của nó

| Công trình                      | Hình Ảnh                    | Trong Game                           |
| ------------------------------- | --------------------------- | ------------------------------------ |
| **Thảo Khấu bị tiêu diệt**      | ![[base_ruin.png]]          | ![[20241223175006.png]] |
| **Thảo Khấu**                   | ![[building_enemy.png]]     | ![[20241223175011.png]] |
| **Boss Thảo Khấu**              | ![[building_boss.png]]      | ![[20241223174957.png]] |
| **Boss Thảo Khấu bị tiêu diệt** | ![[building_boss_raid.png]] | ![[20241224094751.png]] |

Ở khu vực A giới hạn 13 công trình Thảo Khấu và 1 Boss Thảo Khấu

![[MuMu12-20241223-210546.png]]

## [6] Thời gian Reset
Thời gian này đếm ngược 12h, tính từ 12 giờ trưa và 12 giờ đêm, không phải tính từ lúc đánh xong Thảo Khấu.


## [7] Tên công trình
Đây là các công trình ở phía khu vực người chơi (khu vực B) (xem lại mục 4).
Các công trình gồm 

| Tên công trình     | Giới Hạn | Hình Ảnh                   |
| ------------------ | -------- | -------------------------- |
| **Nhà Chính**      | 1        | ![[building_main.png]]     |
| **Mỏ Kim Cương**   | 2        | ![[mine_gem.png]]          |
| **Mỏ Đồng**        | 2        | ![[mine_gold.png]]         |
| **Quặng Ma Thuật** | 2        | ![[mine_dust.png]]         |
| **Nhà Nghiên Cứu** | 1        | ![[building_agi.png]]      |
| **Nhà Khoa Kĩ**    | 1        | ![[building_mili.png]]     |
| **Nhà Vỏ Ốc**      | 1        | ![[building_daffodil.png]] |
Các trạng thái của công trình người chơi

| Công trình       | Hình Ảnh                             |
| ---------------- | ------------------------------------ |
| Nhà chờ xây      | ![[local_building.png]]              |
| Mỏ chờ xây       | ![[local_mine.png]]                  |
| Có thể thu hoạch | ![[20241224091740.png]] |

## [9] Nút Càn Quét
Khi bấm sẽ bung [[Pop-up]] hỏi người chơi có đồng ý càn quét toàn bộ thảo khấu

![[MuMu12-20241223-211951.png]]

Người chơi đồng ý sẽ hiển thị màn hình [[Chuẩn Bị Đội Hình]].

![[MuMu12-20241223-212154.png]]

Ấn Tấn công sẽ hiển thị ra [[Pop-up thưởng]].
Hệ thống sẽ căn cứ vào số Vỏ Ốc mà tấn công Thảo Khấu. 

**Video trong game**

![[HTHT-DaoTroi-CanQuet.mp4]]
# Các Logic khác
## Giới hạn cấp độ công trình

| Tên công trình     | Giới Hạn Cấp Độ                 |
| ------------------ | ------------------------------- |
| **Nhà Chính**      | 20                              |
| **Mỏ Kim Cương**   | 40                              |
| **Mỏ Đồng**        | 40                              |
| **Quặng Ma Thuật** | 40                              |
| **Nhà Vỏ Ốc**      | 40                              |
| **Nhà Nghiên Cứu** | 20 với nâng cấp, 40 với khoa kĩ |
| **Nhà Khoa Kĩ**    | 20 với nâng cấp, 40 với khoa kĩ |

## Khi tương tác với các công trình
### Công Trình Thảo Khấu
Bấm vào sẽ bung [[Pop-up]]

![[20241224093243.png]]

| ID  | Detail                                                            |
| --- | ----------------------------------------------------------------- |
| 1   | Đóng Pop-up                                                       |
| 2   | Tên Công Trình - Thảo Khấu                                        |
| 3   | Số lượng Vỏ Ốc đang có                                            |
| 4   | Danh sách kẻ địch, mỗi kẻ địch có: [[Hệ]], [[Sao]], Cấp Độ        |
| 5   | Tổng % máu còn lại của kẻ địch.                                   |
| 6   | Phần thưởng. Bấm vào mỗi phần thưởng có [[Tool-tip]].             |
| 7   | Nút Ủy thác. Xem bên dưới.                                        |
| 8   | Nút Tấn Công. Bấm vào sẽ hiển thị màn hình [[Chuẩn Bị Đội Hình]]. |
#### Nút Ủy Thác
Hiển thị [[Pop-up]] chọn số lượng vỏ ốc. Sau đó là màn [[Chuẩn Bị Đội Hình]], hệ thống tự động đánh cho đến khi hết vỏ ốc ủy thác. Nếu không dùng hết vỏ ốc thì trả lại.

![[HTHT-DaoTroi-UyThac.mp4]]

#### Nút Tấn Công
Hiển thị [[Chuẩn Bị Đội Hình]], ấn tấn công để vào [[Battle System]] như bình thường.

![[HTHT-DaoTroi-TanCong.mp4]]

#### Công trình bị phá hủy
Khi bấm vào, nút Ủy Thác và Tấn Công xám lại.

![[MuMu12-20241223-214613.png]]

### Công Trình Boss Thảo Khấu
Bấm sẽ ra [[Pop-up]] Boss. 

![[20241224094158.png]]

| ID  | Detail                                                            |
| --- | ----------------------------------------------------------------- |
| 1   | Đóng Pop-up                                                       |
| 2   | Tên Công Trình - Thảo Khấu                                        |
| 3   | Số lượng Vỏ Ốc đang có                                            |
| 4   | Thời gian cho đến khi reset.                                      |
| 5   | Danh sách kẻ địch, mỗi kẻ địch có: [[Hệ]], [[Sao]], Cấp Độ        |
| 6   | Tổng % máu còn lại của kẻ địch.                                   |
| 7   | Nút Tự Động. Hoạt động giống nút ủy thác.                         |
| 8   | Nút Hỗ Trợ                                                        |
| 9   | Nút Tấn Công. Bấm vào sẽ hiển thị màn hình [[Chuẩn Bị Đội Hình]]. |

#### [8] Nút Hỗ Trợ
Bấm vào sẽ bung [[Pop-up]] mời bạn bè. Người chơi có thể chọn bất cứ ai để mời.

![[MuMu12-20241223-214346.png]]

Thông tin của bạn bè gồm: Cấp độ, Avatar, Tên, Giờ Online cuối cùng.
Khi mời, hệ thống sẽ cho mình xem battle của bạn bè với kẻ địch.

Giới hạn hỗ trợ 1 boss: 2 lần.

#### Công trình phá hủy
Nút Tự Đông, Hỗ Trợ và Tấn Công Xám lại.

![[MuMu12-20241223-214702.png]]

### Nhà Chính
UI của nhà chính

![[MuMu12-20241223-214803.png]]

UI Tại Level Max

![[MuMu12-20241223-221338.png]]


### Các trạng thái công trình
#### Thu Hoạch
![[HTHT-DaoTroi-ThuHoachMoDong-ezgif.gif]]

#### Phá Hủy
![[HTHT-DaoTroi-PhaHuy.mp4]]

#### Nâng Cấp
![[HTHT-DaoTroi-NangCap.mp4]]

Khi không thể nâng cấp được thì sẽ xám lại nút nâng cấp và đổi màu ở tài nguyên thiếu

![[MuMu12-20241223-215910.png]]

#### Xây Dựng
![[HTHT-DaoTroi-XayDung.mp4]]

Một số công trình bị giới hạn số lượng xây dựng sẽ hiển thị [[Floating Thông Báo]].

![[HTHT-DaoTroi-XayDungLimit.mp4]]

### Các Mỏ
#### Mỏ đồng
![[MuMu12-20241223-214904.png]]

#### Mỏ Kim Cương
![[MuMu12-20241223-220240.png]]

#### Quặng Ma Thuật
![[MuMu12-20241223-220227.png]]

#### Nhà Vỏ Ốc
![[MuMu12-20241223-220249.png]]

### Nhà Nghiên Cứu và Khoa Kĩ
Khi bấm vào sẽ bung một slide nhỏ từ dưới lên, người chơi chọn Nâng Cấp hoặc Nghiên Cứu.

![[HTHT-DaoTroi-NhaNghienCuu-Selection.mp4]]

|            | Nhà Nghiên Cứu                  | Nhà Khoa Kĩ                                               |
| ---------- | ------------------------------- | --------------------------------------------------------- |
| Nâng Cấp   | Tăng giới hạn cấp độ nghiên cứu | Tăng giới hạn cấp độ nghiên cứu                           |
| Nghiên Cứu | Tăng % sản lượng ở các mỏ.      | Tăng % Công và Máu của nhân vật khi đi tấn công thảo khấu |
#### Nâng Cấp
**Với Nhà Nghiên Cứu**

![[MuMu12-20241223-220636.png]]

**Với Nhà Khoa Kĩ**

![[MuMu12-20241223-220646.png]]

#### Nghiên Cứu
##### Nhà Nghiên Cứu
Với nhà Nghiên Cứu, tăng sản lượng [[Beli]] và [[Bụi Ma Thuật]].

![[MuMu12-20241223-220739.png]]

Ấn vào nút nâng cấp sẽ hiển thị màn hình nâng cấp

![[MuMu12-20241223-220810.png]]

**Video trong game**

![[HTHT-DaoTroi-NhaNghienCuu.mp4]]

##### Nhà Khoa Kĩ
Nhà Khoa Kĩ tăng % Máu và Công khi tấn công các Thảo Khấu.

![[MuMu12-20241223-221035.png]]

Ấn nâng cấp sẽ bung ra màn hình nâng cấp tương ứng

| Nâng cấp công                   | Nâng cấp máu                    |
| ------------------------------- | ------------------------------- |
| ![[MuMu12-20241223-221109.png]] | ![[MuMu12-20241223-221114.png]] |

**Video trong game**

![[HTHT-DaoTroi-NhaKhoaKi.mp4]]

# Animation Request
Gồm Animation Idle của tất cả các công trình và thảo khấu.

| Công trình         | Animation Idle                   |
| ------------------ | -------------------------------- |
| **Thảo Khấu**      | ![[idleThaoKhau-ezgif.gif]]      |
| **Boss Thảo Khấu** | ![[idleThaokhauboss-ezgif.gif]]  |
| **Nhà Chính**      | ![[idleNhaChinh-ezgif.gif]]      |
| **Mỏ Kim Cương**   | ![[idleMoKimCuong-ezgif.gif]]    |
| **Mỏ Đồng**        | ![[idleMoDong-ezgif.gif]]        |
| **Quặng Ma Thuật** | ![[idleQuangMaThuat-ezgif.gif]]  |
| **Nhà Vỏ Ốc**      | ![[idleNhaVoOc-ezgif.gif]]       |
| **Nhà Nghiên Cứu** | ![[idle-nhaNghienCuu-ezgif.gif]] |
| **Nhà Khoa Kĩ**    | ![[idleNhaKhoaKi-ezgif.gif]]     |

Ngoài ra còn có animation Xây Dựng công trình. Game sẽ hiển thị 2 chiếc cuốc vào nhà đó

![[20250110144519.png]]

Xem video tham khảo xây dựng mỏ đồng.

![[HTHT-DaoTroi-XayDung.mp4]]
# Vị trí unlock khi nâng cấp nhà chính
Khi nhà chính nâng cấp, các vị trí sẽ được mở khóa dần theo thứ tự trong hình (cùng số là cùng được mở khóa)

![[20250225141211.png]]

![[20250225141713.png]]