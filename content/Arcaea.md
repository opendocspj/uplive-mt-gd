# Quan sát
- Vào game, ta thấy ngay 1 nhân vật tóc trắng và cần tải thêm gần 1GB content nhạc.
*Điều này chứng tỏ đây là một game được đầu tư rất nhiều content. Dù chưa cần chơi, nhưng với sự chăm chút về đồ hoạ đã là một lời hứa hãy chờ tải xong để được thấy thêm nhiều thứ tươi đẹp.*

![[Pasted image 20260814014620.png|496]]

cover đã thấy gái xinh r  
thế giới toàn gái  
chạy map đi theo step, bán nhạc  
kiếm nhạc khó, ép người chơi phải chơi mấy bài  
vào ô restrict phải chơi đúng bài của nó  
nhân vật tác động vào điểm bài, chỉ số nhân vật tác động vào nó luôn.

Design hypothesis: Game đang giải quyết vấn đề này bằng cách nào?

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
Stamina dùng để chơi bài. Max 12 thể lực, mỗi bài sẽ tốn 0-2 stamina.
Có thể refill bằng cả 2 loại currency: **Memories** và **Fragments**.

### Currency
Tên của 2 loại currency chính: Memories và Fragments.
Memories về cơ bản là Hard Currency, Fragments là Soft Currency.

Game không đặt tên chúng là Kim Cương và Vàng như các game thông thường mà chúng đã được đổi tên để hoà hợp vào Fantasy mà game đang mô tả trong PS. [[#Problem Statement|PS]]

Memories về cơ bản là Hard Currency, Fragments là Soft Currency.

Game **tách biệt rất rõ** content trả phí và content có thể cày. Tức là progression và monetization đã được chia làm 2 lớp rõ rệt.

Về Memories: 
- **Gắn trực tiếp với core loop**: chơi rhythm → kiếm currency.
- Currency không chỉ để mua content mà còn **accelerate progression**.
- Người chơi luôn có lý do để tiếp tục chơi ngay cả khi chưa muốn mua content.
- Có **currency sink** tương đối rõ: stamina / World progression.

## World
Người chơi vượt các world chủ yếu để lấy:
- Song mới
- Partner mới
- Chart mới (Beyond Chart - end game content)
- Core (item nâng cấp cho partner)
- Fragments (soft currency)
World là một meta thể hiện PS của game. Gắn kết chặt chẽ với core rhthym.

World tạo từ các bậc. 
Để khám phá world, cần leo bậc.
Để leo bậc, cần chơi bài.
Để chơi bài, cần stamina.

Partner tác động đến tốc độ khám phá World.
///


Bản thân mỗi bậc lại có các cơ chế khác nhau: 

## Partner
Partner sẽ có Story riêng. Thông qua story của partner, người chơi sẽ có thêm góc nhìn về thế giới.
Ngoài ra, một Partner sẽ có **chỉ số** và **kĩ năng** khác nhau. Việc lựa chọn Partner ảnh hưởng đến cả meta và core.

Về chỉ số, một partner có 3 loại (nâng cấp theo level): 
- **FRAG**: lượng Fragment nhận được sau khi chơi.
- **STEP**: lượng **map progress** nhận được khi chơi World Mode.
- **OVER**: progress trong Beyond Chapters.

Về kĩ năng, partner tác động vào nhiều thứ: Gameplay, cách tính score, cách tính world step, tăng tài nguyên và các hiệu ứng đặc biệt khác.

Ngoài ra, partner có thể nâng cấp từ đó tăng cao chỉ số.
-> Tức là, partner giờ thực sự trở thành PARTNER (cost để rebuild cao). Việc lựa chọn partner giờ đây trở thành lối build chiến thuật chứ không phải đơn thuần cosmetic.

## Potential và Beyond Chapters
**Potential** là điểm **đánh giá năng lực chơi game**. Đóng vai trò như một **skill gate**.
Khác với Grade là đánh giá 1 lần chơi, Potential là đánh giá toàn bộ quá trình chơi.

Đây chính là điểm số để người chơi có thể mở khoá End game content: **Beyond Chapters (Lost/Breached)**, beyond trở thành **endgame dành cho người chơi có năng lực**, thay vì chỉ là content mở khóa bằng tiền hoặc grind.

## Độ khó
**vocabulary riêng cho difficulty**:

**Past → Present → Future → Eternal**

Điều này rất hợp với identity của game và khiến difficulty trở thành một phần của product language.

Đặc biệt **Beyond** không đơn giản là “Harder”. Nó là một **lớp chart đặc biệt**, được gắn với World Mode và progression endgame.

Nếu đưa vào Design Library:

> **Difficulty system = một phần vừa của skill progression, vừa của world vocabulary.**

## Người chơi thấy bản thân progress trong game ở rất nhiều nơi

| Hệ thống          | Là thước đo                |
| ----------------- | -------------------------- |
| **Grade**         | một chart                  |
| **Potential**     | độ thành thạo              |
| **STEP**          | Progress của **World Map** |
| **FRAG**          | Economy                    |
| **Partner Stats** | Character progression      |

## Song Mechanics
Ngoài 1 Lane bình thường như các game âm nhạc khác, Arcaea đã mở rộng ra trục trên, từ đó thêm vào cơ chế Arc và Sky Note. Tạo ra tính độc nhất của game.

| Note →     |                    Tap                    |                   Sky                    |                   Long                   |                   Arc                    |
| ---------- | :---------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
| **Verb ↓** | ![[Pasted image 20260814032237.png\|120]] | ![[Pasted image 20260814032320.png\|96]] | ![[Pasted image 20260814032223.png\|81]] | ![[Pasted image 20260814032202.png\|77]] |
| **Tap**    |                     ✓                     |                    ✓                     |                    ✓                     |                    ✓                     |
| **Hold**   |                                           |                                          |                    ✓                     |                    ✓                     |
| **Trace**  |                                           |                                          |                                          |                    ✓                     |

Nhìn vào bảng ta có thể thấy số lượng hành động mà người chơi cần làm khi một note xuất hiện. Số lượng hành động này có thể coi như độ khó của note trong game.
Nhìn vào bảng, ta thấy Arc chắc chắn là note khó nhất.

Bằng cách sắp xếp thứ tự và hình dạng note trong không gian gameplay. Game tạo ra rất nhiều biến thể để diễn chart.

Về lý thuyết, ta có thể đo chính xác độ khó của 1 chart dựa vào số lượng hành động mà người chơi phải làm. 
Phần còn lại là tạo ra các combo của Note. Từ đó thấy được dynamic mà người chơi sẽ làm khi tới đoạn đó.
Giả sử, game có combo: Tap + Arc. Dễ dàng tưởng tượng được, người chơi sẽ 1 tay tap và 1 tay trace theo Arc. Với combo khác: Tap, Arc, Double Tap, Arc + Long, ta vẫn dễ dàng tưởng tượng ra hành động của người dùng. 

## Dynamic từ hệ thống Core

Trong phần mechanics, tôi sẽ break các mechanics ra các verb và objects, chỉ ra sự kết hợp của chúng tạo ra dynamics gì trong gameplay. VD: 1 bài hát của game A thường sẽ build như này, sau đó như này, cuối cùng như này.



Ví dụ:
Tap + Note
→ timing interaction
→ tạo anticipation → reaction → reward

Hold + Note → Release
→ tension → timing judgment → release reward

Swipe + Note
→ directional input → anticipation → physicality

Sau đó mới đi lên level cao hơn:

Pattern / Song Structure
Intro → establish mechanic
Verse → introduce variation
Build-up → increase density
Chorus → mechanic combination
Drop → peak difficulty / feedback
Outro → resolution

Đây mới là thứ cực kỳ actionable cho Magic Tiles.

Bạn không chỉ lấy mechanic, mà lấy grammar của gameplay.
Mechanics = vocabulary
Patterns = grammar
Song/chart = sentence
Gameplay moment = punctuation / climax

Đây là thứ tôi nghĩ rất đáng đưa vào library.

# Art / Visual Design


![[Pasted image 20260814015345.png]]


Ngay từ loading screen, game đã ghi rõ ràng: Hai cô gái trẻ, khám phá thế giới vụn vỡ, với âm nhạc là thứ chứa đựng quá khứ.

Trong phần nhìn, tôi nghĩ chủ đề là cái mà game đó phải xuyên suốt. nên fx, ui, anim,... (thậm chí sfx) đều phải hỗ trợ cho chủ đề đó.

Ý của bạn về **Theme** rất đúng.

Tôi sẽ không coi Theme = “forest / cyberpunk / cute”.
Mà:
> **Theme là một visual language xuyên suốt experience.**

Sau đó kiểm tra:
**Theme**  
↓  
Art Direction  
↓  
UI  
↓  
UX feedback  
↓  
Animation  
↓  
VFX  
↓  
Note design  
↓  
Stage  
↓  
SFX

Tức là hỏi:
> **Các thành phần có đang cùng nói một ngôn ngữ không?**

Ví dụ một game có theme “magical music”:
- Note shape → magical
- Hit VFX → magical
- Combo animation → magical
- UI transition → magical
- Stage → magical
- SFX → magical

Nếu mỗi thứ đẹp riêng nhưng ghép lại không cùng một fantasy → **design system không coherent**.

Điểm này rất hợp với hướng playbook về **identity + differentiation**.

# Audio

Bạn vẫn hoàn toàn có thể làm phần này, nhưng nên phân tích dưới góc **Game Design / Player Experience**, không cần giả vờ mình là sound designer.

Tôi đề xuất 4 câu hỏi:
### A. SFX có communicate gameplay không?

Ví dụ:
**Tap → sound**

Player có lập tức biết:
- hit đúng?
- hit perfect?
- miss?
- combo?
- special note?
→ Đây là **information**, không chỉ là sound effect.
### B. SFX có reinforce impact không?

Ví dụ:
> Note nhỏ → click nhỏ  
> Perfect → sound lớn hơn / brighter  
> Combo → layer thêm  
> Special mechanic → unique sound

Bạn đang xem:
> **Input → SFX → perceived impact**
### C. Audio có tạo progression không?

Ví dụ:
Combo càng cao → music/SFX càng layered.

Hoặc:
Special section → music thay đổi.
→ Audio trở thành **feedback của player mastery**.
### D. Music có được dùng như gameplay material không?
Đây là phần đặc biệt quan trọng với Magic Tiles.

Hỏi:
> **Game có biến music thành một phần của mechanic không, hay chỉ dùng music làm background?**

Ví dụ:
**Music build-up**  
→ note density tăng  
→ VFX tăng  
→ mechanic phức tạp hơn

**Drop**  
→ major gameplay moment

Nếu music và chart cùng build tới climax → rất đáng học.

# 5. Meta
Trong phần meta, tôi sẽ phân tích toàn bộ mô hình meta để tìm hiểu source sink và các điểm progression của game. Họ đặt pay wall ở đâu. Chúng phù hợp với kiểu người nào.

Phần này bạn nói **source / sink / progression / paywall** là đúng.

Tôi sẽ thêm một layer:
### Motivation → Meta System → Economy

Ví dụ:
**Collection motivation**  
→ Song Collection  
→ Song fragments / coins  
→ Album completion  
→ reward

**Mastery motivation**  
→ Mastery level  
→ XP  
→ Upgrade / unlock

**Expression motivation**  
→ Cosmetics  
→ Currency  
→ Collection

Sau đó map:

### Economy
**Sources**
- gameplay
- daily
- event
- ad
- pass
↓
**Currencies**
↓
**Sinks**
- unlock
- upgrade
- retry
- cosmetics
- collection
↓
**Progression**
- account
- song
- collection
- event
- mastery
↓
**Monetisation**
- RV
- IAP
- pass
- bundle
- paywall
↓
**Player motivation / archetype**

Đây sẽ giúp phần Meta của bạn **không biến thành catalog feature**.

# 6. What We Learn
Đây là phần tôi nghĩ bạn **nên bắt buộc có**.

