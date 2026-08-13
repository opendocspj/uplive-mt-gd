---
tags:
  - battle
  - system
  - tiennt
  - readyUI
---
# Cấu Trúc
**Gồm 3 phần** 
1. [[Chuẩn Bị Đội Hình]] - người chơi chuẩn bị và sắp xếp đội của mình.
2. Battle - cơ chế [[Turnbased]]. 
3. [[Kết Quả Trận Đấu]].
![[20241112155058.png]]
![[20241122141555.png]]

| ID  | Detail                                                                                |
| --- | ------------------------------------------------------------------------------------- |
| 1   | Nút [[Info Khắc Hệ]]. Bấm vào hiện ra [[Pop-up]] [[Info Khắc Hệ]]                     |
| 2   | Số Vòng Đấu                                                                           |
| 3   | Nút tăng tốc [[Battle Speed]]. Bấm vào tăng tốc trận đấu.                             |
| 4   | Nút [[Skip Trận Đấu]]. Bấm vào kết thúc trận đấu và dẫn đến màn [[Kết Quả Trận Đấu]]. |
| 5   | Danh sách các [[Hệ]] trong đội hình. Bấm vào hiển thị tool-tip (xem bên dưới).        |
| 6   | Đội hình phe mình                                                                     |
| 7   | Đội hình phe địch                                                                     |
| 8   | Background màn chơi -> Xem [[Danh sách Background Battle]].                           |
# UX mong muốn 
![[20241122161022.png]]
![[20241122141017.png]]
Khi tap vào biểu tượng sẽ có [[Tool-tip]] hiện ra.
![[20241122141201.png]]
![[20241122155459.png]]
Các dòng được kích lên sẽ có màu xanh, chi tiết thông tin xem trong [[Kích Dòng Class]].

# Ref ART
![[MuMu12-20241118-170158.png]]
**Video UI Battle**
![[1119.mp4]]

# Update 26 Nov 2024
![[20241126093818.png]]
Các cánh sao sẽ sáng theo các màu hệ của các nhân vật trong battle.
Sao trong trận là 6 cánh - tương đương với 6 nhân vật.
