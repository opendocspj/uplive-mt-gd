# First Impression
- Ngay khi vào game, đập vào mắt là một screen các em mèo rất bắt mắt.

![[Pasted image 20260815031510.png|440]]

- Game rất vui và mới lạ. Game thay thế gần như toàn bộ âm thanh bằng **tiếng mèo**. Từ bài hát, note cho đến các tương tác trong game. 

![[ScreenRecording_08-10-2026 23-19-36_1-00.00.40.422-00.00.43.071.mp4]]

- **PvP có flow tốt:** Hệ thống rank PvP không yêu cầu người chơi tự chọn bài mà **match ngẫu nhiên bài hát**, giúp giảm thời gian chuẩn bị và khiến trận đấu diễn ra nhanh, tự nhiên hơn.
- Kho nhạc được chia thành các **category rõ ràng**, đồng thời có hệ thống **Favorite Song**. Việc tìm thấy một bài hay -> Favorite -> muốn chơi ngay tạo thành một vòng lặp khám phá khá tự nhiên.

Game tạo cảm giác muốn tự đi khám phá bài hát mà mình biết ở dạng mèo sẽ như thế nào.

# Problem Statement

Giả thiết về Fantasy của game:

> [!Problem Statement (từ nay viết tắt là PS)]
> > **Một rhythm game dùng âm nhạc để khám phá và tái hiện quá khứ của một thế giới đã tan vỡ.**

Fantasy này được thể hiện trong mọi mặt của game. Ta sẽ thấy trong các phần bên dưới.
# Core Mechanics

## Song Mechanics

Ngoài 1 Lane bình thường như các game âm nhạc khác, Arcaea đã mở rộng thêm trục trên biến khu vực chơi thành một không gian 2 chiều. Vị trí input trở thành một phần của gameplay. 
Từ đây, cơ chế Arc và Sky Note đã tạo ra tính độc nhất của game.

| Note →     |                    Tap                    |                   Sky                    |                   Long                   |                   Arc                    |
| ---------- | :---------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
| **Verb ↓** | ![[Pasted image 20260814032237.png\|120]] | ![[Pasted image 20260814032320.png\|96]] | ![[Pasted image 20260814032223.png\|81]] | ![[Pasted image 20260814032202.png\|77]] |
| **Tap**    |                     ✓                     |                    ✓                     |                    ✓                     |                    ✓                     |
| **Hold**   |                                           |                                          |                    ✓                     |                    ✓                     |
| **Trace**  |                                           |                                          |                                          |                    ✓                     |

Nhìn vào bảng ta có thể thấy số lượng hành động mà người chơi cần làm khi một note xuất hiện. Số lượng hành động này có thể coi như độ khó của note trong game.
Nhìn vào bảng, ta thấy Arc chắc chắn là note khó nhất.

Bằng cách sắp xếp thứ tự và hình dạng note trong không gian gameplay. Game tạo ra rất nhiều biến thể để diễn chart.

Về lý thuyết, ta có thể đo chính xác độ khó của 1 chart dựa vào số lượng hành động mà người chơi phải làm. Chart design lúc này thực chất là tạo ra chuỗi hành động.

Phần còn lại là tạo ra các combo của Note. Từ đó thấy được dynamic mà người chơi sẽ làm khi tới đoạn đó.

Giả sử, game có combo: Tap + Arc. Dễ dàng tưởng tượng được, người chơi sẽ 1 tay tap và 1 tay trace theo Arc. Với combo khác: Tap, Arc, Double Tap, Arc + Long, ta vẫn dễ dàng tưởng tượng ra hành động của người dùng. 

## Một số design thú vị

Arc note đứng không thì vẫn chỉ đơn giản là note Long nhưng đổi track. Nhưng nhờ có thêm sky input, Arc thực sự trở thành một innovation củarung vào những pattern mình giỏi, tương tự việc spam một tướng để leo rank trong MOBA vậy.

---

# Art/Visual Design
*Phần này bàn về toàn bộ phần nhìn trong game: Art Design, VFX, Animation...* 

Giống như [[#Core Mechanics]], Art trong game cũng phải phục vụ [[#Problem Statement]].

Thật vậy, ngay từ loading screen, game đã ghi rõ ràng: Hai cô gái trẻ, khám phá thế giới vụn vỡ, thế giới đó đầy những thanh âm chứa đựng quá khứ.

![[Pasted image 20260814015345.png]]

Đây là một minh chứng rất rõ về những gì mà game đang hướng đến.
## Về Art Core Gameplay

Chúng ta có thể dễ dàng thấy, game gợi ra cảm giác của một thế giới rất kì lạ. 

Các background trong bài hát hầu hết đều rất kì ảo. Các đoạn cắt ngang dọc, cảnh vật méo mó lẫn lộn. Một số rất dễ nhận ra, nhưng một số thì lại kì ảo.

Tất cả có thể nói rằng, game đang cố gợi một khung cảnh, một kí ức nào đó trong thế giới mà bài hát đó hướng đến.

![[Pasted image 20260814223816.png]]

Chronostasis (Ảo giác ngưng đọng thời gian), background đen trắng giống như thời gian đã dừng.


![[Pasted image 20260814224217.png]]

Remind the Souls - background thể hiện lore game, đại diện cho phần thế giới Arcaea tươi sáng,  yên bình.

![[Pasted image 20260814224239.png]]

Senkyou - 仙境 (Tiên Cảnh) được thẻ hiện bằng lồng đèn lung linh và khung cảnh lãng mạn.

Như vậy, ta có thể thấy mỗi bài hát đều thể hiện một câu chuyện không chỉ thông qua phần nhạc mà còn cả phần hình ảnh. 

---

Trái ngược với sự chi tiết trong phông nền, Playfield của game thể hiện một sự đối lập. 

>Sạch, ít texture, ít vật thể, chủ yếu là các shape hình học đơn giản. **Điều này giúp playfield trở thành nơi focus rất rõ ràng.** 

Như vậy, Arcaea dùng artwork để kể lore, còn playfield được tối giản để tối ưu core gameplay. 

Với hướng thiết kế như vậy, toàn bộ phần nhìn trong core gameplay vừa đáp ứng functionality, vừa đáp ứng [[#Problem Statement]].

## Về VFX

Khá thú vị là game chỉ có 2 dạng FX: 

| Loại ấn (tap)                             | Loại giữ (hold)                           |
| ----------------------------------------- | ----------------------------------------- |
| ![[Pasted image 20260814230917.png\|201]] | ![[Pasted image 20260814230927.png\|203]] |
|                                           | ![[Pasted image 20260814230943.png\|208]] |

Cả hai loại đều rất sáng, thậm chí có phần chói và cực kì rõ ràng. Một phần vì ngón tay người chơi sẽ che khuất phần lớn hiệu ứng, nên FX cần có kích thước và độ sáng đủ lớn để feedback vẫn dễ nhận biết.

Ngoài ra, mỗi bài khác nhau thì VFX có đổi màu để phù hợp với design của nó

![[Pasted image 20260814234237.png|181]]![[Pasted image 20260814230927.png|166]]

*Cùng là note Long nhưng VFX ở 2 bài khác màu nhau.*

**Quan sát thấy,** FX của loại ấn (tap) tạo ra cảm giác như đang "xé không gian" trong thế giới. Điểm này cũng bám [[#Problem Statement|PS]] được phần nào. Tuy vậy cá nhân người viết thấy, detail của VFX quá nhỏ để thể hiện được bất cứ tính chất nào. Ở phần này, VFX chỉ cần đồng bộ với gameplay là đủ. Mọi thứ sẽ tự kể câu chuyện của riêng nó. Thứ đóng góp phần lớn vào phần nhìn vẫn là background và design của playfield.

## Một số design thú vị

![[Pasted image 20260814233036.png]]

Các dải sọc xám trắng chạy dọc theo track tạo ra **perspective**, khiến người chơi cảm giác note đang di chuyển trong một không gian từ xa đến gần rõ ràng hơn.

# Audio
*Phần này phân tích dưới góc nhìn **Game Design**, chứ không phải sound designer.*

## SFX
**Quan sát:** SFX communicate trạng thái gameplay đến mức nào.
- Game có SFX phản hồi khi input đúng: khi tap, trong lúc ấn giữ.
- Không có SFX input ứng với các trạng thái Pure (Perfect), Far/Late (Good)... 
- SFX trong game rất nhẹ.
- Tất cả các note gần như đều dùng cùng 1 SFX.
- Không có SFX Lost (miss input).

Như vậy, ta có thể kết luận: 

> **SFX của Arcaea chỉ ở mức cơ bản, ưu tiên sự tối giản, không cạnh tranh với âm nhạc. 
> 
> Nó communicate rõ trạng thái input thành công, nhưng không quan tâm đến chất lượng input và failure state. Vì vậy, phần lớn thông tin của input vẫn được truyền tải bằng visual feedback và text thay vì âm thanh.**

## Music
**Quan sát:** Music đóng góp như thế nào vào core gameplay nói riêng và toàn bộ game nói chung? 
- Music và Chart có liên quan đến nhau rất rõ ràng. 
- Note có các pattern bám theo beat, melody và vocal linh hoạt.
- Chart phản ánh cấu trúc của bài nhạc. Verse, Chorus, Bridge, Drop có các pattern khác nhau. Thường được phản ánh bằng mật độ và pattern của chart.
- Khó có thể dự đoán note dựa vào nhạc (đây là cảm giác của Rhthym heaven).
- Hình ảnh, nhạc và note rất khớp nhau. 
- Arc Note cực sync với vocal, khi giọng cao thì arc lên cao, thấp thì nó xuống thấp.
- Có thể nhớ music thông qua **chart pattern**.

![[Screenrecording 08-11-2026 00-03-15 1-00.33.57.224-01.08.01.080-00.29.22.940-00.29.37.999-1.mp4]]
*Music có design chart ấn tượng (video).*

Như vậy, ta có thể kết luận:

>Music và Chart trong Arcaea tạo thành một thể thống nhất, khiến người chơi không chỉ nghe mà còn hiểu được đặc điểm của bài nhạc. 
>Với sự kết hợp giữa âm nhạc và core gameplay mang bản sắc riêng (Sky Input), game đã khiến trải nghiệm chơi rhthym trở nên rất đáng nhớ.

# 5. Meta
*Ở phần này, chúng ta sẽ phân tích meta, tìm hiểu các điểm progression của game từ đó tìm ra các điểm đặt pay wall tiềm năng.*

![[Pasted image 20260815024924.png|700]]

*Toàn bộ hệ thống của Arcaea có thể gói gọn theo sơ đồ sau ([[Arcaea Meta Visualize.canvas|click vào đây để xem file gốc]])*

**Ta có thể thấy:**
- **Stamina** và **World** chính là 2 điểm nghẽn lớn nhất. 
- **Song** là content để bộ máy hoạt động.
- **Partner** ở một line riêng, chỉ có tác dụng tăng tốc progression. 
- Partner thực chất chỉ là **quà tặng kèm** khi mua song pack.

Game có hai con đường monetize:
1. Bán thời gian (Stamina).
2. Bán trực tiếp content (Songs). 

Hai con đường này tách người chơi thành ba nhóm:
1. **F2P**: mãi mãi không nạp tiền, chỉ có thể chơi các bài miễn phí. 
2. **Paid User**: mở khoá cả các bài độc quyền và nhân vật độc quyền.
3. **Paid + Farm:** người cày cả 2 loại content.

Do đó, ta có thể kết luận:

> Stamina là **giới hạn** cho content **progression** (World). 
> 
> Arcaea cho phép premium currency **bypass time** gate này, nhưng monetization chính vẫn nằm ở content pack thay vì bán stamina như một sản phẩm độc lập.

