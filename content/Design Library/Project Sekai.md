# First Impression
- Ngay khi vào game, người chơi được giới thiệu một nhân vật nổi bật và phải tải một lượng lớn music/content trước khi chơi.
- Artwork của game đặt character ở vị trí rất nổi bật, đặc biệt trên cover và song artwork. Character là một phần quan trọng trong game.

![[Pasted image 20260814014620.png]]

- Game có cơ chế hoạt động phức tạp, cách dùng từ lạ lẫm (Fragments, World, PURE, Past...).
- **World Mode** cho phép người chơi di chuyển trên map dựa trên Step để nhận reward và unlock content. 

![[Pasted image 20260815030151.png]]

- Mở khoá nhạc mới khá rất lâu.
- Core gameplay khó, độc đáo.

![[Pasted image 20260815030131.png]]

Tại sao game lại mang một vẻ phức tạp như vậy? Họ đang giải quyết vấn đề gì?

# Problem Statement

Giả thiết về Fantasy của game:

> [!Problem Statement (từ nay viết tắt là PS)]
> > **Một rhythm game dùng âm nhạc để khám phá và tái hiện quá khứ của một thế giới đã tan vỡ.**

Fantasy này được thể hiện trong mọi mặt của game. Ta sẽ thấy trong các phần bên dưới.
# Core Mechanics

Các từ khoá cần biết

| Từ khoá    | Đơn giản là             |
| ---------- | ----------------------- |
| Memories   | Hard Currency           |
| Fragments  | Soft Currency           |
| Beyond-ish | các end game content    |
| Partner    | "waifu", "character"    |
| Core       | item nâng cấp partner   |
| PST        | Past: độ khó dễ nhất    |
| PRS        | Present: độ khó vừa     |
| FTR        | Future: độ khó cao      |
| ETR        | Eternal: độ khó rất cao |
| BYD        | Beyond: độ khó cực hạn  |
| Potential  | mức pro của người chơi  |

## Stamina và Currency
### Stamina
Stamina dùng để chơi rhythm. Max 12 thể lực, mỗi bài sẽ tốn 0-2 stamina.
Có thể refill bằng cả 2 loại currency: **Memories** và **Fragments**.

### Currency

![[Pasted image 20260814212617.png]]

Tên của 2 loại currency chính: Memories và Fragments.
Memories về cơ bản là Hard Currency, Fragments là Soft Currency.

Game không đặt tên chúng là Kim Cương và Vàng như các game thông thường, chúng đã được đổi tên để hoà hợp vào Fantasy mà game đang mô tả ([[#Problem Statement|PS]]).

**Mục đích của Fragments:** 
- **Gắn trực tiếp với core**: chơi rhythm -> kiếm currency.
- Người chơi có thể đốt **Fragments** để **tăng tốc progression** trong [[#World]].
- Người chơi luôn có lý do để tiếp tục chơi ngay cả khi chưa muốn mua content.

**Mục đích của Memories:**
- Mua premium content. 

**Hướng design:**
- Game **tách biệt rõ** content trả phí và content có thể cày. Tức là progression và monetization được chia làm 2 lớp rất rõ rệt.

## World

![[Pasted image 20260814211740.png]]

World tạo từ các bậc. 

Để khám phá world, cần leo bậc.

Để leo bậc, cần chơi bài.

Để chơi bài, cần stamina.

**Người chơi vượt các world chủ yếu để lấy:**
- Song mới
- Partner mới
- Chart mới (Beyond Chart - end game content)
- Core (item nâng cấp cho partner)
- Fragments (soft currency)

**Mục đích của World:**
- Biến việc chơi nhạc thành progression **thấy được**.
- Mở khoá content trong game.
- Là nơi để **partner tham gia vào progression**.
- Là bước đệm để tạo nhiều cơ chế meta sâu hơn: các bậc có mechanics riêng, buff thế giới,... 

>World là meta thể hiện [[#Problem Statement|PS]] của game. Gắn chặt chẽ với core rhthym.

## Partner
Từ [[#Problem Statement|PS]], partner là nhân vật đồng hành cùng người chơi để khám phá thế giới.

Một Partner sẽ có **chỉ số** và **kĩ năng** khác nhau. Việc lựa chọn Partner ảnh hưởng đến cả meta và core.

Về chỉ số, một partner có 3 loại (nâng cấp theo level): 
- **FRAG**: lượng Fragment nhận được sau khi chơi.
- **STEP**: lượng **map progress** nhận được khi chơi World Mode.
- **OVER**: progress trong Beyond Chapters.

Về kĩ năng, partner tác động vào nhiều thứ: Gameplay, cách tính score, cách tính world step, tăng tài nguyên và các hiệu ứng đặc biệt khác.

Ngoài ra, partner có thể nâng cấp từ đó tăng cao chỉ số.
-> Tức là, việc lựa chọn partner ảnh hưởng đến chiến thuật progression chứ không đơn thuần là cosmetic. 

**Mục đích của Partner:**
- Tạo trải nghiệm gắn kết.
- Mở rộng meta game. 
- Kết nối về mặt mechanics: giữa Core gameplay và World. 
- Là trung gian để người chơi quan tâm đến các content meta khác: Story, World, Event, DLC.

## Potential và Beyond Chapters

**Vấn đề:**
> Những người chơi giỏi khi đã mở khoá hết content game thì còn gì níu kéo họ chơi nữa?

**Vấn đề phát sinh:**
>Mà, làm sao để biết một người chơi là "người chơi giỏi"?

**Potential** sinh ra để giải quyết vấn đề đánh giá 1 người chơi là người chơi giỏi.
**Beyond** sinh ra để giải quyết content end-game cho những người đó.

### Potential
Khi chơi xong mỗi bài, game sẽ chấm điểm. 
Điểm này chỉ đánh giá được 1 lần chơi của người chơi.
Điểm số của người chơi có thể bị ảnh hưởng bởi kĩ năng của [[#Partner]].

![[Pasted image 20260814214759.png]]

Vậy thì, việc dùng điểm để đánh giá không còn đúng nữa.

Như vậy game sẽ cần 1 chỉ số khác để đánh giá toàn bộ quá trình chơi của họ. Đóng vai trò như một **skill gate**.

**Mục đích của Potential**: 
- Ngăn người chơi mới vào content endgame quá sớm.
- Tạo ra thước đo để mở khoá end-game content.

### Beyond

![[Pasted image 20260814215050.png]]

*Beyond Chart*

![[Pasted image 20260814215110.png]]

*Beyond Chapter*

![[Pasted image 20260814215513.png]]

*Beyond World/Map*

Sau khi đã có thước đo đánh giá năng lực người chơi. 
Tất cả họ sẽ tiếp tục đối mặt với content end-game cuối cùng.

**Mục đích của Beyond-ish:**
- Tạo thử thách dành cho người chơi đã master core gameplay.
- Tạo mục tiêu dài hạn cho người chơi chưa đạt trình độ Beyond.
- Tái sử dụng content cũ bằng các chart Beyond mới.
- Làm dày meta game mà không cần thay đổi quá nhiều thứ (chỉ số OVER của Partner ảnh hưởng lớn đến progress trong Beyond).

> Beyond không mở rộng theo chiều ngang (thêm nhiều bài hơn), mà mở rộng theo chiều sâu (đào sâu mastery của gameplay hiện có).

## Độ khó

Để phù hợp với [[#Problem Statement|PS]] của game. Cách đặt tên độ khó trong Arcaea cũng không giống các game âm nhạc bình thường.
Họ tạo ra các khái niệm mới, độ khó tăng dần từ trái sang phải. Dễ nhất là PST, khó nhất là BYD.

| PST  | PRS     | FTR    | ETR     | BYD    |
| ---- | ------- | ------ | ------- | ------ |
| Past | Present | Future | Eternal | Beyond |

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

Arc note đứng không thì vẫn chỉ đơn giản là note Long nhưng đổi track. Nhưng nhờ có thêm sky input, Arc thực sự trở thành một innovation của dòng. 

![[Pasted image 20260814233607.png]]

Nhân vật có chỉ số tác động vào content game. Người chơi phải chọn build nhân vật nào để kiếm cái gì. Game chia rất rõ ràng các hệ thống progress nhỏ, các chỉ số nhân vật cũng tác động vào chính xác những progress đó, khiến game có chiều sâu meta hơn.

![[Pasted image 20260814233952.png|317]]![[Pasted image 20260814234031.png|320]]

**Potential chuyển trọng tâm đánh giá từ “kết quả của một bài” sang “trình độ tổng thể của người chơi”.** Tuy nhiên, vì Potential vẫn được tính từ một tập thành tích cụ thể, nó chưa phản ánh đầy đủ độ đa dạng về kỹ năng: người chơi có thể tối ưu Potential bằng cách tập trung vào những pattern mình giỏi, tương tự việc spam một tướng để leo rank trong MOBA vậy.

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

