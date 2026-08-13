---
tags:
  - thamhiem
  - duongnd
  - readyUI
---
Diễn hoạt giữa đội hình user **3 tướng ngẫu nhiên** chạy idle đánh quái trong map với 1 quái random theo từng [[địa điểm thám hiểm]].
- Quái đánh lần lượt nhân vật hàng trước rồi tới hàng sau. Bị chết nếu bị tấn công 2 lần. Khi chết, tài nguyên sẽ rơi vào [[Hòm AFK]].
- Tướng trong đội hình có thể nói chuyện, mỗi bóng thoại hiển thị trong 5s, cách nhau 20s. 
	- Thường xuyên ghé thăm để thu thập tài nguyên nhé.
	- Đội trưởng cứ việc nghỉ ngơi, chúng tôi sẽ thu thập tài nguyên.
- Các thông tin mô tả khác xem trong video.

![[HTHT_AFK.mp4]]

Mỗi khi quái chết, item rơi ra và tài nguyên sẽ bay về hòm. 
![[bandicam2024-12-0514-24-51-686.mp4]]


Hòm có 3 trạng thái (từ trái sang phải): Rỗng, Có Tài Nguyên, Đầy.
![[20241113111319.png]]

**Chuyển trạng thái khi**:
Từ hòm rỗng: Có 2 lần tài nguyên bay vào sẽ sang trạng thái có tài nguyên.
Từ hòm có tài nguyên: Từ hòm có tài nguyên, sau 5 phút không nhận thì chuyển trạng thái đầy.

Ở trạng thái Đầy, có bàn tay chỉ vào nhận. 
![[HTHT_AFK_Full.mp4]]

Khi nhận hòm AFK, hiện ra [[Pop-up]] thưởng. Chi tiết chỉ số xem trong file Balance.
![[20241205142655.png]]


Nhận quà AFK , với điều kiện exp nhận đủ đạt level sẽ hiện thông báo đạt level
![[20241204150149.png]]

FX khi mở hòm
![[HuyềnThoạiHảiTặc(9).mp4]]

FX tài nguyên bay lên thanh tài nguyên khi nhận
Tài nguyên bay lên
Thanh tài nguyên sáng nhấp nháy
![[HuyềnThoạiHảiTặc(10).mp4]]