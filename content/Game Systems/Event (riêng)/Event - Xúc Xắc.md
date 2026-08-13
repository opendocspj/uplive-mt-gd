---
tags:
  - event
  - duongnd
  - readyUI
---
# Vị trí tính năng
Ngoài [[Lobby System (Home)]], bấm vào biểu tượng Xúc Xắc. ![[20250210142838.png]]

Trong **thời gian diễn ra sự kiện**, người chơi sử dụng Xúc Xắc tung điểm để đi trên bàn, nhận quà tương ứng. Khi đi hết mỗi vòng, quà sẽ tăng lên

# Luật chơi
## Sự Kiện Xúc Xắc

1. [Xúc Xắc Bình Thường] : ![[20250210143934.png]] Di chuyển ngẫu nhiên 1 – 6 bước tương ứng với số nút đổ xúc xắc.
2. [Xúc Xắc May Mắn] : ![[20250210143943.png]]  Người chơi được chọn số ô muốn di chuyển.
3. [Lá Bài Tarrot] : ![[20250210143900.png]] Khi di chuyển vào ô này, bạn sẽ được chọn 1 trong 3 là bài có hiệu ứng ngẫu nhiên.
4. [Chóng Mặt] : ![[20250210143911.png]] Khi di chuyển vào ô này, ở lần đổ xúc xắc tiếp theo nếu ra **số chẵn sẽ tiến lên**, nếu ra **số lẻ sẽ đi lùi về** theo số bước tương ứng với số nút xúc xắc.
5. [Nguyên Liệu] : Khi di chuyển vào các ô tài nguyên, Thuyền Trưởng sẽ nhận được tài nguyên tương ứng, đồng thời ô tài nguyên đó sẽ được nâng cấp lên 1 level, tối đa 3 level.

6. [Sao May Mắn] : ![[20250210144007.png]] Khi đi qua hoặc di chuyển vào ô Sao May Mắn, Thuyền Trưởng sẽ nhận được Sao. Khi đạt đủ mốc Sao, Thuyền Trưởng sẽ nhận được quà tương ứng theo mốc. Khi di chuyển vào ô Sao May Mắn sẽ nâng cấp level của ô này, tối đa tăng 3 level.

## Hướng dẫn chung:

7. Tiến hành đổ xúc xắc để di chuyển, mỗi lượt đi sẽ tiêu hao 1 xúc xắc, mục tiêu của bạn là đi càng nhiều vòng nhất có thể để thu thập cũng như nâng cấp level tài nguyên và Sao.
8. Mỗi một vòng sẽ cần thu thập 500 Sao, Thuyền Trưởng hãy thu thập đủ 500 sao để nhận toàn bộ mốc quà, sau đó quà sẽ được reset lại và Thuyền Trưởng có thể thu thập Sao & nhận thêm các mốc quà.
9. Xúc xắc thường có thể nhận được thông qua các sự kiện, quà hằng ngày hoặc mua bằng kim cương.
10. Xúc xắc may mắn có thể nhận được khi di chuyển vào ô xúc xắc may mắn trong sự kiện, hoặc thông qua các gói nạp ưu đãi.
11. Xúc xắc có thể tái sử dụng ở lần mở sự kiện tiếp theo.

# Mô tả tính năng

![[20250210143638.png]]

| ID  | Giải nghĩa                    |
| --- | ----------------------------- |
| 1   | "X" thoát cửa sổ sự kiện      |
| 2   | Thời gian còn lại của sự kiện |
| 3   | Tên sự kiện                   |
| 4   | Vòng hiện tại/ tổng số vòng   |
| 5   | Số sao tích lũy               |
| 6   | Trợ giúp                      |
| 7   | Phần thưởng                   |
| 8   | Xúc xắc nhận mỗi ngày         |
| 9   | Main (nhân vật chính)         |
| 10  | Tài nguyên trong vòng quay    |
| 11  | Xúc xắc thường                |
| 12  | Xúc xắc may mắn               |
| 13  | Bỏ qua hiệu ứng               |

## 1. Xúc xắc hằng ngày
- Mỗi ngày người chơi sẽ được nhận free: 2 [Xúc Xắc Thường] - cần ấn nhận mới nhận được thưởng
## 2. Cấu tạo bàn xúc xắc
### a. Bàn xúc xắc 
- Có 22 ô tài nguyên. Bao gồm: 15 ô tài nguyên, 3 ô sao may mắn, 1 ô choáng, 1 ô bài tarot, 1 ô xúc xắc thường, 1 ô xắc may mắn
- Có 1 ô: [Start], main sẽ bắt đầu ở đó.
### b. Tài nguyên
- 15 ô tài nguyên: gồm các loại tài nguyên và số lượng khác nhau, khởi điểm đều level 1
- Mỗi khi main dừng ở ô tài nguyên nào, ô đó sẽ tăng level tài nguyên, tối đa 3 level. Khi tăng level số lượng quà cũng tăng lên. [**File Balance | Danh sách tài nguyên + số lượng**](https://docs.google.com/spreadsheets/d/1uSZCHcOM-FG_FCv4v_xMnhVttvERaSoRw7NNHp7AQhk/edit?gid=340885960#gid=340885960&range=A1)
### c. Sao may mắn
- Sao may mắn cách đều nhau 6 ô
- Khi đi qua ô này thì nhận được số sao tương ứng. Tích luỹ sao để đổi các phần quà rất giá trị
- Mỗi khi người chơi tung xúc xắc: đi qua hoặc dừng lại ở ô đều nhận được số sao may mắn tương ứng
- Khi dừng ở ô sao may mắn, số level sao may mắn cũng tăng lên
### d. Choáng
- Đi vào ô này bạn sẽ bị choáng. Nếu lần xúc xắc kế tiếp là chẵn thì được đi tiến, lẻ thì bị đi lùi theo số chấm trên xúc xắc
### e. Bài Tarot
- Chọn 1 trong 3 lá bài ngẫu nhiên. Lá bài có thể: May mắn hoặc Xui Xẻo!
- Nội dung lá bài: [**File Balance | Danh sách lá bài + hiệu ứng**](https://docs.google.com/spreadsheets/d/1uSZCHcOM-FG_FCv4v_xMnhVttvERaSoRw7NNHp7AQhk/edit?gid=340885960#gid=340885960&range=A1)
### f. Xúc xắc thường
- Đi vào để nhận thêm 1 xúc xắc thường
### g. Xúc xắc may mắn
- Đi vào để nhận thêm 1 xúc xắc may mắn
### h. Vòng
- Mỗi 1 vòng quay người chơi cần thu thập 500 sao. Khi đủ sẽ sang vòng tiếp theo
- Có tối đa 3 vòng
## 3. Phần thưởng
- Người chơi thu thập sao may mắn, khi đạt mốc sẽ được quà tương ứng
- Phần thưởng tự động gửi
- [**File Balance | Danh sách mốc sao + quà tương ứng**](https://docs.google.com/spreadsheets/d/1uSZCHcOM-FG_FCv4v_xMnhVttvERaSoRw7NNHp7AQhk/edit?gid=340885960#gid=340885960&range=A1)
## 4. Xúc xắc
### a. Xúc xắc thường
- Mua: **150** kim cương / 1 xúc xắc thường
- Nhận qua các sự kiện, quà hằng ngày. [**File Balance | Số lượng xúc xắc thưởng tại các sự kiện**](https://docs.google.com/spreadsheets/d/1uSZCHcOM-FG_FCv4v_xMnhVttvERaSoRw7NNHp7AQhk/edit?gid=340885960#gid=340885960&range=A1)
	- Sự kiện: gói ưu đãi
		- Giá: 22k : 2 xúc xắc, 2 chìa khóa vượt ngục
		- Giá: 69k: 2 xúc xắc, 5 chìa khóa vượt ngục
		- Giá 129k: 4 xúc xắc, 10 chìa khóa vượt ngục
		- Giá 499k: 16 xúc xắc, 40 chìa khóa vượt ngục
		- Giá 749k: 24 xúc xắc, 60 chìa khóa vượt ngục
		- Giá 1299k: 40 xúc xắc, 100 chìa khóa vượt ngục
		- Giá 2199k: 80 xúc xắc, 200 chìa khóa vượt ngục
	- Vòng quay Siêu cấp
		- 25 điểm: 1 xúc xắc
		- 50 điểm: 1 xúc xắc
		- 100 điểm: 1 xúc xắc
		- 150 điểm: 1 xúc xắc
		- 250 điểm: 2 xúc xắc
		- 350 điểm: 2 xúc xắc

### b. Xúc xắc may mắn
- Nhận khi quay trúng ô
# Video 
![[HuyềnThoạiHảiTặc(18).mp4]]

## 1. Anim
- Main ![[20250210152951.png]]
- Choáng: ![[20250210153344.png]]

- Xúc xắc may mắn: ![[20250210153145.png]]
- Bài tarot ![[20250210153057.png]]
- Thưởng (7)
![[MuMu12-20250313-162415.png]]