---
tags:
  - thanhtuu
  - duongnd
  - tiennt
  - readyUI
---
# Vị trí tính năng
Từ màn hình [[Lobby System (Home)]], bấm vào Nhiệm Vụ để hiện ra [[Pop-up]] Nhiệm Vụ Hằng Ngày.
![[20241119143823.png]]

# Mô tả tính năng
![[20241119143702.png]]
  
| ID  | Giải nghĩa                                                 |
| --- | ---------------------------------------------------------- |
| 1   | Back Button. Bấm về [[Lobby System (Home)]].                      |
| 2   | Tên Tính năng [Nhiệm vụ]. Không thể bấm.                   |
| 3   | Đồng hồ đếm ngược làm mới. Không thể bấm.                  |
| 4   | Tiêu đề nhiệm vụ tổng.                                     |
| 5   | Quà nhận khi hoàn thành all nhiệm vụ. Bấm ra [[Tool-tip]]. |
| 6   | Thanh tiến độ tổng nhiệm vụ.                               |
| 7   | Tiêu đề nhiệm vụ ngày.                                     |
| 8   | Thanh tiến độ của nhiệm vụ ngày.                           |
| 9   | Quà khi hoàn thành nhiệm vụ ngày. Bấm ra [[Tool-tip]].     |
| 10  | Thực hiện. Bấm sẽ dẫn đến tính năng để làm nhiệm vụ.       |

# Nhiệm vụ ngày
## Thời gian
- Nhiệm vụ ngày sẽ chỉ được làm trong ngày từ 0:00 → 23:59:59
- Qua ngày mới sẽ được Làm mới. Có đồng hồ đếm ngược thời gian làm mới
## Số lượng nhiệm vụ
- Có 10 nhiệm vụ ngày cần thực hiện
- Danh sách nhiệm vụ và số lần thực hiện. File Balance
- Thanh tiến độ: Đang làm, Hoàn thành, Chưa làm

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfsi327xcPc3fQkF7NBN7tyQtYzfCAan1dJeAizaXaP973i57vwaRlHrg2NfPZm3xQXP36qp14suo1qKHdIlKqrYkCoinmHkAchY9_FaAJZ7LPxrs11CDdVhLEpKA-ld92yoD_x?key=RVbebzSoXuxmWJKRlFJX8PxQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd_onDSn1xdo3uq31gi9tRgifM2x0VBz40VhPaKcbfo-h-R0zRb2xRAycsIvSP-6pWPcdMtDgloYuaOqy5IEypaVUgpNjdCBCzKcThpm0TdPTHGxzun7Qs8PtdcNz-QbU3NbCSXlg?key=RVbebzSoXuxmWJKRlFJX8PxQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc8xq4iV2yNO19odCVmPUnYwYzuhNShXdgI9MilTHXFbegH4pfgYYPEfy3JjTt2IofhoMf6ZXYhi-f372izpnlRiAWaHJWAa4OSgHTmsIFMRUILKWMhhjc-y0RtK-HPRPn3bNeUPg?key=RVbebzSoXuxmWJKRlFJX8PxQ)

## Quà
- Mỗi nhiệm vụ khi hoàn thành sẽ có quà thưởng riêng. Khi nhận quà sẽ bung [[Pop-up thưởng]].
- Khi hoàn thành tất cả nhiệm vụ ngày trong ngày sẽ được bonus thêm thưởng.
- Quà khi hoàn thành nhiệm vụ và tất cả nhiệm vụ. File Balance.
- Khi user không nhận ngay thưởng, qua ngày thưởng sẽ chuyển qua [[Thư]]
## Thực hiện & Nhận thưởng
- Button **Thực hiện** sẽ đưa user đến tính năng tương ứng để làm nhiệm vụ
- Thực hiện sẽ chuyển thành **Nhận thưởng** khi user hoàn thành nhiệm vụ.
- Khi Nhận thưởng xong sẽ có trạng thái hoàn thành
![[20241119145740.png]]

## Log cần bổ sung
- Quest được hoàn thành/số user
- Quest được hoàn thành nhiều nhất
- Số user hoàn thành tất cả nhiệm vụ/ số user
# Config
- Nhiệm vụ & quality cả nhiệm vụ
- Thưởng nhiệm vụ
