---
tags:
  - hero
  - phuongch
  - readyUI
---
# Vị trí tính năng
Từ [[Lobby System (Home)]], bấm vào [[Thông Tin Tướng]], mở tab [[Bảo Vật]] và ấn vào ô Bảo Vật.
![[HTHT-TrangBiNone_baovatgif.gif]]

# Mô tả tính năng
- Mỗi Tướng có 1 **ô bảo vật**
![[20241126164457.png]]
- Điều kiện mở khóa: [[Unlock Tính Năng]]
- Khi click vào ô bảo vật: sẽ xuất hiện danh sách bảo vật 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe7NelI0pTNsMnk3eFInIBPNTBWHeC4Tf83ZuwsUfUr30o8HvrpqDTt1k2wxjkPOt5WqD-jrdFuNPxbMvsjoxRYUvQ_-EcX6bRXlBKjNEuc07bJC07qTc-18oNPnixbqnWkoMARtg?key=OAGsZBxi1N9J8bm8LC37Hi3-)


- Người chơi chọn bảo vật để Bảo Vật cho nhân vật. Hệ thống bung [[Pop-up]] hỏi người chơi lắp đồ.
![[HTHT-FlowTrangBigif.gif]]
- Sắp xếp bảo vật từ phẩm thấp>cao>sao
- Danh sách các phẩm bảo vật: Lục; Tím; Vàng; Bỏ
- Chọn bảo vật user muốn
- Ấn X để quay lại Bảo Vật
# Các trạng thái
![[20241126164948.png]]
Bảo vật có 2 trạng thái: chưa có và đã có đồ.

# Nâng cấp bảo vật
Full Flow tại video bên dưới
![[HTHT-NangCapTrangBi.mp4]]

Ấn vào biểu tượng nâng cấp khi thay bảo vật trong [[Pop-up]]. ![[20241126165457.png]]

![[20241126165419.png]]
![[MuMu12-20241126-045509.png]]
- Các bảo vật phẩm lục trở lên có thể nâng cấp
- Sử dụng bảo vật khác để nâng sao cho bảo vật
- Khi nâng cấp, được lựa chọn số lượng dùng 1 hay dùng 10.
![[MuMu12-20241126-045530.png]]
![[MuMu12-20241126-045558.png]]
Nếu còn dư EXP, hệ thống sẽ bung [[Pop-up]] qui đổi lại thành bảo vật cấp thấp nhất.
![[20241126165630.png]]

| Phẩm | Sao  | Exp (bảo vật trắng*10) |
| ---- | ---- | ---------------------- |
| Lục  | 1->2 | 190                    |
|      | 3    | 190                    |
|      | 4    | 190                    |
| Tím  | 1->2 | 1440                   |
|      | 3    | 1440                   |
|      | 4    | 1440                   |
|      | 5    | 1440                   |
| Vàng | 1->2 | 2880                   |
|      | 3    | 2880                   |
|      | 4    | 2880                   |
|      | 5    | 2880                   |
| Đỏ   | 1->2 | 5400                   |
|      | 3    | 5400                   |
|      | 4    | 5400                   |
|      | 5    | 5400                   |
|      | 6    | 5400                   |

| Phẩm  | EXP | Phẩm | EXP |
| ----- | --- | ---- | --- |
| Trắng | 10  | Vàng |     |
| Lục   |     | Đỏ   |     |
| Tím   |     |      |     |

## Thêm chỉ số
- Các bảo vật vàng với đỏ khi đeo đúng lớp nhân vật sẽ tăng thêm chỉ số

## Icon Bảo Vật

![[20241126172056.png]]

| id  | Là gì                                                                   |
| --- | ----------------------------------------------------------------------- |
| 1   | Khung ứng với từng phẩm bao bên ngoài (màu sắc khung đại diện cho phẩm) |
| 2   | Hiệu ứng khung Bảo Vật nếu có                                           |
| 3   | Background cùng màu với phẩm                                            |
| 4   | Hình ảnh Bảo Vật                                                        |
| 5   | Hình ảnh hiệu ứng Bảo Vật(nếu có)                                       |
| 6   | Sao Bảo Vật ở góc dưới trái                                             |
| 7   | Số lượng ở góc dưới bên phải                                            |
| 8   | Hệ (nếu có) ở góc trên bên phải                                         |