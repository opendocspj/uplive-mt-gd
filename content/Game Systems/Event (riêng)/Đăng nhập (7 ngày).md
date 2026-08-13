---
tags:
  - event
  - duongnd
  - readyUI
---
# Tài liệu
Docs System gốc: [Link](https://docs.google.com/document/d/1mrTc6qHIMISd3wN_wcpB0UwF7JBZEoenx2Jp3-7OxO0/edit?tab=t.0#heading=h.76545dsn0x58)
Docs Balance gốc: Link

# Vị trí tính năng
Tại [[Lobby System (Home)]], ấn vào Đăng Nhập.
![[20241119160604.png]]
# Mô tả tính năng
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfJlOACxC2qn7xZSq0u6mg9Z51Xnrs8BvoLbh2MhZefixxC1126b64HZEn-WZzOj9nsMI9MVXuNqS-jteVhm_vOdzX6FBOkDNdzIH08X0QTs6GBmGvsmoAipEUVqUHlV4oBCzNVzQ?key=pDt4uHqJE9Sz5EOKsztYyTBi)

| ID  | Giải nghĩa                                   |
| --- | -------------------------------------------- |
| 1   | Nhấn ra ngoài về lại [[Lobby System (Home)]].       |
| 2   | Tên tính năng [7 ngày mở server]             |
| 3   | Ngày hiện tại hoặc ngày đang chọn            |
| 4   | Đặc trưng quà nhận cho ngày đang chọn        |
| 5   | Tab đang chọn                                |
| 6   | Tab chưa chọn                                |
| 7   | Phúc lợi ngày chọn                           |
| 8   | Quà Phúc lợi ngày                            |
| 9   | Button [Nhận]                                |
| 10  | Quest ngày đang chọn (list)                  |
| 11  | Quà quest                                    |
| 12  | Button [Đến] - đi tới tính năng làm nhiệm vụ |
| 13  | Ngày chưa mở hoặc ngày không chọn            |
| 14  | Quà đặc trưng                                |
| 15  | Đồng hồ đếm ngược thời gian 7 ngày           |

# 7 ngày mở Server
## Quy tắc
- Data quest, Thưởng: File Balance
- Tổng quan: hệ thống quest chỉ available trong 7 ngày đầu tính từ khi người chơi mở app lần đầu. Mỗi ngày trong 7 ngày sẽ unlock 1 hệ thống quest mới. Sau 7 ngày hệ thống quest sẽ biến mất. Và lặp lại 7 ngày nữa với hệ thống quest mới Ngoài reward ở mỗi quest
- Hệ thống quest: track các action của người chơi, tính số lượt người chơi thực hiện action. Các milestone tính action sẽ cộng dồn và tăng dần 
- Hệ thống reward: với mỗi nhiệm vụ hoàn thành người chơi sẽ nhận được phần thưởng tương ứng với quest

# Log cần bổ sung
- Số user theo số lượng điểm danh

# Config
- Danh sách quà điểm danh
