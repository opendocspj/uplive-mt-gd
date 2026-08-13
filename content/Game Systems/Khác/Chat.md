---
tags:
  - tiennt
  - readyUI
---
# Vị trí tính năng
Từ màn hình [[Lobby System (Home)]], chọn biểu tượng chat.

![[20241226160510.png]]
# Mô tả tính năng
![[20241226160753.png]]

| ID  | Detail                                       |
| --- | -------------------------------------------- |
| 1   | Tab - Thế Giới.                              |
| 2   | Tab - Máy Chủ.                               |
| 3   | Tab - [[Hạm Đội]].                           |
| 4   | Tab - Tuyển Mộ.                              |
| 5   | Tab - Hệ Thống.                              |
| 6   | Avatar và cấp độ của người chat.             |
| 7   | Nội dung chat.                               |
| 8   | Tên nhân vật và VIP của người chat.          |
| 9   | Thời gian chat - không có ngày.              |
| 10  | Nút đóng UI.                                 |
| 11  | Nơi nhập nội dung chat.                      |
| 12  | Nút gửi nội dung chat.                       |

## [1-5] Các Tab Chat
Mỗi tab có đều có chức năng giống nhau. Có giới hạn thời gian 1 lần chat là 5s và hệ thống lọc từ. Các từ bị lọc sẽ thành dấu *

Hiển thị bóng thoại chat: 500 bóng thoại gần nhất.

![[HTHT-ChatTab-ezgif.gif]]

### Tab Thế Giới
Là nơi người chơi ở tất cả các server có thể chat với nhau.
### Tab Máy Chủ
Chỉ người chơi ở máy chủ đó mới có thể chat với nhau.
### Tab Hạm Đội
Chỉ người chơi ở cùng hạm đội mới có thể chat với nhau.
Nếu chưa tham gia hạm đội, hiển thị khung chat trống và [[Floating Thông Báo]] "Bạn chưa tham gia hạm đội".

![[MuMu12-20241226-212328.png]]

### Tab Tuyển Mộ

![[MuMu12-20241226-212539.png]]

Người chơi không thể gửi tin nhắn ở kênh này.
### Tab Hệ Thống
Người chơi không thể gửi tin nhắn ở kênh này.

![[MuMu12-20241226-212614.png]]

## [6] Avatar và cấp độ của người chat
Khi bấm vào sẽ bung ra [[Pop-up]] thông tin người chơi. Xem thêm tại mục [5] trong [[Bạn Bè]].

![[MuMu12-20241226-210839.png]]

## [7] Nội dung chat
Bóng Thoại Thường

![[20241227090518.png]]

Bóng thoại chia sẻ trận đấu, có nút Xem lại. Khi ấn vào sẽ vào xem trận đấu luôn.

![[20241227090530.png]]

Tự chat thì bóng thoại sẽ ở bên phải, chat của người khác ở bên trái

![[MuMu12-20241226-210704.png]]

Share thông tin nhân vật sẽ share tên nhân vật, màu đỏ nằm trong ngoặc vuông.

![[20241227090816.png]]

Bấm vào dòng đỏ sẽ bung [[Pop-up]] thông tin tướng.

![[MuMu12-20241226-210820.png]]

Bóng thoại ở riêng tab tuyển mộ sẽ có nút gia nhập

![[20241227090610.png]]

Khi bấm vào nút gia nhập sẽ hiển thị [[Floating Thông Báo]]
1. Nếu đang ở trong bang mà xin vào bang khác, hiện "Bạn đang ở bang khác."
2. Nếu không có bang mà xin vào thì hiện "Đã nộp đơn xin gia nhập."

## [12] Nút gửi nội dung chat
Người chơi không thể gửi nội dung trống.
Người chơi chỉ có thể chat ở kênh thế giới nếu đạt cấp 80. Nếu chưa đạt, bung [[Pop-up]].

![[MuMu12-20241226-212909.png]]