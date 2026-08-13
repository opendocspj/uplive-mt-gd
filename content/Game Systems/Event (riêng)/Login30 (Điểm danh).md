---
tags:
  - event
  - duongnd
  - readyUI
---
# Tài liệu
Docs System gốc: [Link](https://docs.google.com/document/d/1-s9oifMxRcEZhxFoN-5jqgSjrpiHfZK5GFswidQiV8w/edit?tab=t.0#heading=h.76545dsn0x58)
Docs Balance gốc: Link

# Vị trí tính năng
Ngoài [[Lobby System (Home)]], ấn vào biểu tượng Điểm Danh
![[20241119160012.png]]
# Mô tả tính năng

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcQVhPQek5l9qdAHy7KT0lN-6XjFz8JmfTPeOzSxV4DvpM-vlcTQmvMRE1yQsxIz6cGpHNm6VlCUiLBdEbLjgOsOHtD4K-zn8vFE8eXwseCGuCZ68aPOviSyA9NT4SJf1lp6fRhPA?key=UYuBNwVCqT9SSJ0NTE9fyi3-)

| ID  | Giải nghĩa                                      |
| --- | ----------------------------------------------- |
| 1   | Nhấn ra ngoài về lại màn hình chính             |
| 2   | Tên tính năng [Điểm danh]                       |
| 3   | Khung + BG popup [Điểm danh]                    |
| 4   | Trạng thái Quà đã nhận - xám đi và có dấu tích. |
| 5   | Trạng thái quà có thể nhận - có hiệu ứng.       |
| 6   | Đồng hồ đếm ngược quà nhận                      |
| 7   | Trạng thái quà chưa thể nhận                    |
| 8   | Button Điểm danh                                |

# Điểm danh
## Quy tắc
- Người chơi online trong ngày, được tính điểm danh thành công, có thể nhận quà lần thứ x điểm danh
- Người chơi không online, sẽ không tính lượt điểm danh
- Điểm danh không tính theo số ngày thực tại, chỉ tính lượt điểm danh
- Điểm danh thành công nhận quà, không online sẽ không nhảy cóc quà
## Thời gian
- Trong thời gian 0h → 23:59:59 người chơi online vào game được tính có thể nhận quà ở ngày hôm đó. Hiển thị trạng thái Có thể nhận.
![[20241119160149.png]]
- Đồng hồ đếm ngược thời gian đến 0h ngày kế tiếp. ![[20241119160213.png]]
## Số lượng item/quà
- Có 30 slot trong bảng Điểm danh - tương ứng 30 ngày, 30 lần điểm danh
- Danh sách item. File Balance

## Nhận thưởng
- Click button **Điểm danh** để nhận quà
- Với những ngày online thành công, nhưng chưa nhận quà thì có thể ấn **Điểm danh** liên tục để nhận quà lần lượt
- Quà sẽ trả qua thư. Tiêu đề: "Điểm Danh", nội dung "Phần thưởng điểm danh hằng ngày"
![[20241119160440.png]]
- Khi nhận hết quà, button **Điểm danh** sẽ biến mất
# Log cần bổ sung
- Số user theo số lượng điểm danh
# Config
- Danh sách quà điểm danh