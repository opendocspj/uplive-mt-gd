---
tags:
  - battle
  - tiennt
  - readyUI
---
# Vị trí
Hệ thống chiến đấu chia làm 2 phe đấu nhau 6 vs 6, đánh theo lượt. 
Một vòng được tính khi tất cả nhân vật đều tấn công ít nhất 1 lần.

Nhân vật luôn tấn công ưu tiên theo vị trí 1->6.
Nhân vật tấn công theo tốc độ đánh. **Tốc độ** cao hơn tấn công trước.
Cùng tốc độ thì ưu tiên theo vị trí.
![[20241106162841.png]]

# Sát thương
**Hiển thị text dmg phân chia màu theo hiệu ứng: Hiện ra rồi bay từ từ lên và biến mất.**
Khi critical - số to hơn rất nhiều rồi thu bé lại, màu đỏ
![[20241122143111.png]]

Khi đánh thường, số màu trắng
![[20241122143421.png]]

Khi hồi máu, số màu xanh lá
![[20241122143513.png]]

Gây sát thương chuẩn, số màu cam
![[20241122143534.png]]

Gây sát thương ngay khi bắt đầu lượt, căn cứ vào loại sát thương mà nó màu trắng, cam hoặc đỏ.
# Nhân Vật
Trên đầu nhân vật sẽ có
![[20241122142010.png]]
Cấp độ ![[20241122142039.png]]
[[Hệ]] ![[20241122142044.png]]
**Thanh Máu** và **Thanh Nộ** ![[20241122142049.png]]
Thanh Nộ có thể lên 3 Tầng, càng lên màu càng đậm ![[20241122144005.png]] 
Trong trận đấu, các buff sẽ hiển thị trên đầu nhân vật, theo thứ tự từ phải ngoài cùng. Hiệu ứng xấu nằm hết về bên phải, hiệu ứng tốt nằm hết về bên trái. (Xem danh sách trong [[Hiệu Ứng Battle]])
![[20241122143739.png]]
Nếu buff có hiệu ứng trên 2 lượt sẽ có con số để thể hiện số turn mà hiệu ứng gây ra ![[20241122144126.png]]
Các hiệu ứng buff vĩnh viễn sẽ có biểu tượng vô cực.
