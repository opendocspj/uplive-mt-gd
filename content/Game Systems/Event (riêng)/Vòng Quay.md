---
tags:
  - event
  - duongnd
  - readyUI
---
# Tài liệu
Docs System gốc: [Link](https://docs.google.com/document/d/157v7k435b_zcDH5bT2jzmQ3ZQxnGAMZ7I9Z_VVGxfgQ/edit?tab=t.0#heading=h.76545dsn0x58)
Docs Balance gốc: Link

# Vị trí tính năng
Từ màn hình [[Lobby System (Home)]], vào Vòng Quay.
![[20241119153810.png]]
  
# Mô tả tính năng
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc701niDtM4R1cPp1JsnFkJrktxqtbLOaE2OUnxHJ-cWX5s2tXzZJhDI-QIgLBk7B_ovQJr4oAzTJmR74axZv_Ymtw3It_VbivTPByXdP_mwlM8sAxBe2o2aaubHrvH-gYK9Tuz?key=_NwE6L7Nsvuah99xBrIqnscI)

| ID  | Giải nghĩa                        |
| --- | --------------------------------- |
| 1   | Back Button về lại màn hình chính |
| 2   | Nền popup/background              |
| 3   | Khung & BG Vòng quay thường       |
| 4   | Khung & BG Vòng quay siêu cấp     |
| 5   | Vòng quay thường                  |
| 6   | Vòng quay siêu cấp                |

# Vòng Quay Thường
![[HTHT-VongQuay.mp4]]

![[20241128145635.png]]

| ID  | Giải nghĩa                                                     |
| --- | -------------------------------------------------------------- |
| 1   | Back Button về lại [[Lobby System (Home)]].                           |
| 2   | Thanh tài nguyên. Không bấm được.                              |
| 3   | Đồng hồ đếm ngược làm mới. Không bấm được.                     |
| 4   | Vòng quay.                                                     |
| 5   | Item thưởng trong vòng quay. Bấm vào hiển thị ra [[Tool-tip]]. |
| 6   | Nút Quay 1 lượt                                                |
| 7   | Nút Quay 10 lượt                                               |
| 8   | Nút Quay 100 lượt                                              |
| 9   | Nút Làm mới                                                    |
| 10  | Background Vòng quay thường (có anim + fx)                     |
| 11  | Trợ giúp. Bấm vào mở [[Pop-up]] [[Trợ Giúp Vòng Quay]].        |
| 12  | Cửa hàng. Bấm vào tới [[Shop Vòng Quay]]                       |
# Vòng Quay Siêu Cấp
![[HTHT-VongQuaySieuCap.mp4]]

![[20241128145737.png]]

| ID  | Giải nghĩa                                                     |
| --- | -------------------------------------------------------------- |
| 1   | Back Button về lại [[Lobby System (Home)]].                           |
| 2   | Thanh tài nguyên. Không bấm được.                              |
| 3   | Đồng hồ đếm ngược làm mới. Không bấm được.                     |
| 4   | Vòng quay                                                      |
| 5   | Item thưởng trong vòng quay. Bấm vào hiển thị ra [[Tool-tip]]. |
| 6   | Nút Quay 1 lượt                                                |
| 7   | Nút Quay 10 lượt                                               |
| 8   | Nút Quay 100 lượt                                              |
| 9   | Nút Làm mới                                                    |
| 10  | Background Vòng quay thường (có anim + fx)                     |

# Vòng quay Thường
## Thời gian
- Vòng quay Thường tồn tại suốt thời gian của game
- Khi 0h (qua ngày mới) sẽ bắt buộc Làm mới phần thưởng trong vòng quay

## Số lượng item/quà
- Có 8 slot trong 1 vòng quay
- Danh sách item và tỷ lệ ra theo vòng quay. File Balance
## Quay

| Quay | [[Xu Vòng Quay]] | Điều kiện       |
| ---- | ---------------- | --------------- |
| 1    | 1                | Không điều kiện |
| 10   | 8                | VIP3 hoặc LV80  |
| 100  | 80               | Thẻ Rảnh tay    |
Khi quay mà không đủ điều kiện sẽ hiển thị [[Floating Thông Báo]]. 
## Làm mới
- Đến 0h mỗi ngày sẽ bắt buộc làm mới item trong vòng quay
- Lần đầu trong ngày sẽ free làm mới (không mất kim cương).
- Các lần tiếp theo mất 40 [[Kim Cương]], không giới hạn lượt làm mới.

| Lần | Kim cương |
| --- | --------- |
| 1   | 0         |
| 2   | 40        |
| 3   | 40        |
| 4   | 40        |
| 4+  | 40        |

## Cỏ 4 Lá
- 1 lần quay vòng quay sẽ nhận được 10 [[Cỏ 4 Lá]]
- Cỏ 4 Lá là tiền tệ mua đồ trong [[Shop Vòng quay]]
# Vòng quay Siêu cấp

## Thời gian
- Vòng quay Thường tồn tại suốt thời gian của game
- Khi 0h (qua ngày mới) sẽ bắt buộc Làm mới phần thưởng trong vòng quay.
## Số lượng item/quà
- Có 8 slot trong 1 vòng quay
- Danh sách item và tỷ lệ ra theo vòng quay. File Balance
## Quay

| Quay | [[Xu Quay Siêu Cấp]] | Điều kiện       |
| ---- | -------------------- | --------------- |
| 1    | 1                    | Không điều kiện |
| 10   | 10                   | VIP3 hoặc LV80  |
| 100  | 100                  | Thẻ Rảnh tay    |
Khi quay mà không đủ điều kiện sẽ hiển thị [[Floating Thông Báo]].
## Làm mới
- Đến 0h mỗi ngày sẽ bắt buộc làm mới item trong vòng quay
- Mỗi ngày sẽ free làm mới 1 lần (không mất kim cương)
- Các lần tiếp theo mất 100 kim cương, không giới hạn lượt làm mới

| Lần | Kim cương |
| --- | --------- |
| 1   | 0         |
| 2   | 100       |
| 3   | 100       |
| 4   | 100       |
| 4+  | 100       |

- Quay vòng quay Siêu cấp không nhận được [[Cỏ 4 Lá]]
# Xu Quay 
- Khi hết có thể mua bằng [[Kim Cương]]

| Xu                     | Kim Cương      |
| ---------------------- | -------------- |
| 1 [[Xu Vòng Quay]]     | 50             |
| 1 [[Xu Quay Siêu Cấp]] | Không mua được |

# Log cần bổ sung
- Số vé quay thường tiêu thụ của mỗi user
- Số vé quay thường tiêu thụ theo level user
- Số vé quay siêu cấp tiêu thụ của mỗi user
- Số vé quay siêu cấp tiêu thụ theo level user
# Config
- Quà vòng quay
- Giá mua vé thường
- Số lượng cỏ 4 lá khi quay vé thường
# Art Request List
- Nhân vật trong BG có anim.
- Vòng quay có anim quay khi idle.
