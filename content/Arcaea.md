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

# Problem Statement
Giả thiết về Fantasy của game:

> [!Problem Statement (từ nay viết tắt là PS)]
> > **Một rhythm game dùng âm nhạc để khám phá và tái hiện quá khứ của một thế giới đã tan vỡ.**

Chứng minh:
![[Pasted image 20260814015345.png]]
Ngay từ loading screen, game đã ghi rõ ràng rồi: Hai cô gái trẻ, khám phá thế giưới vụn vỡ, với âm nhạc là thứ chứa đựng quá khứ.



Partners have 3 stats: FRAG, STEP and OVER. These stats can be improved by levelling them up with EXP. EXP is earned for the selected partner when playing songs in World Mode. The three stats work as follows:

- FRAG affects the amount of Fragments earned after playing songs.
    - Partners with high FRAG will earn more Fragments.
- STEP affects the map progress earned after playing songs in World Mode (except in Lost Chapter: Beyond).
    - Partners with high STEP will progress through World Mode maps faster.
- OVER affects the map progress earned after playing songs in World Mode's Beyond Chapters (Lost and Breached).
    - Map progress in the Lost Chapter depends on both OVER and Partner Affinities (see [Partner Affinity](https://arcaea.fandom.com/wiki/World_Mode_Mechanics#Partner_Affinity "World Mode Mechanics")). Different maps have an Affinity for different Partners (Partners with no map Affinity default to x1 Affinity). In general, Partners with a high product of Affinity x OVER will progress through Beyond Chapter maps faster.
    - Map progress in the Breached Chapters is more complicated, and depends on a unique new stat called PROG. PROG depends on OVER, but also on other stats and Partner Level (see the [article](https://arcaea.fandom.com/wiki/World_Mode_Mechanics#Beyond_Mechanics "World Mode Mechanics") for details).

về phần design library, tôi nghĩ là sẽ chia ra nhiều game, mỗi game sẽ được phân tích:

1. problem statement của game đó. (quan sát được)
2. phân tích về phần nhìn (art: anim, fx, ui, ux...), phần tiếng (sfx, music), phần core (mechanics), phần meta (có gì mà phù hợp với core), chúng có hợp với problem statement không.

Trogn phần mechanics, tôi sẽ break các mechanics ra các verb và objects, chỉ ra sự kết hợp của chúng tạo ra dynamics gì trong gameplay. VD: 1 bài hát của game A thường sẽ build như này, sau đó như này, cuối cùng như này.

Trong phần nhìn, tôi nghĩ chủ đề là cái mà game đó phải xuyên suốt. nên fx, ui, anim,... (thậm chí sfx) đều phải hỗ trợ cho chủ đề đó.

Trong phần meta, tôi sẽ phân tích toàn bộ mô hình meta để tìm hiểu source sink và các điểm progression của game. Họ đặt pay wall ở đâu. Chúng phù hợp với kiểu người nào.

Trong phần SFX và Music, tôi sẽ chỉ ra phần nào SFX làm tốt và có ý đồ (nếu tôi nhìn ra), music được sử dụng khéo léo ở đâu,... (thực ra tôi k có kinh nghiệm làm về phần nghe trong game, bạn hãy giúp tôi)

**Không phải game nào cũng cần phân tích sâu tất cả các mục.**

Bạn có thể **đào sâu thứ game đó làm tốt**, thay vì cố ép tất cả game vào cùng một checklist.
## 1. Problem Statement

Chỉ ghi những gì quan sát được, chưa vội giải thích nguyên nhân.
Ví dụ:

Player có thể hiểu core trong 10 giây.
Nhưng sau 5–10 bài, pattern bắt đầu lặp lại.
Feedback khi hit note chưa tạo cảm giác impact.
Meta có nhiều reward nhưng không liên kết rõ với gameplay.

Sau đó mới đặt:
Design hypothesis: Game đang giải quyết vấn đề này bằng cách nào?

Điều này rất hợp với tinh thần playbook: observation → hypothesis → experiment, thay vì nhảy thẳng sang “game này hay vì...”.

# Core Mechanics
Các từ khoá cần biết

| Từ khoá    | Đơn giản là              |
| ---------- | ------------------------ |
| Memories   | Hard Currency            |
| Fragments  | Soft Currency            |
| Beyond-ish | các end game content     |
| Partner    | "waifu", "character"     |
| Core       | item nâng cấp partner    |
| PST        | Past: độ khó dễ nhất     |
| PRS        | Present: độ khó vừa      |
| FTR        | Future: độ khó cao       |
| ETR        | Eternal: độ khó rất cao  |
| BYD        | Beyond: độ khó cực hạn   |
| Potential  | mức pro của người chơi   |

## Stamina
Dùng để chơi bài.
Có thể refill bằng cả 2 loại currency: Memories và Fragments.

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
Ngoài 1 Lane bình thường như các game âm nhạc khác, Arcaea đã mở rộng ra trục trên, từ đó thêm vào cơ chế của Arc và Sky Note

| Note →     |                    Tap                    |                   Long                   |                   Arc                    |                   Sky                    |
| ---------- | :---------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
| **Verb ↓** | ![[Pasted image 20260814032237.png\|120]] | ![[Pasted image 20260814032223.png\|81]] | ![[Pasted image 20260814032202.png\|77]] | ![[Pasted image 20260814032320.png\|96]] |
| **Tap**    |                     ✓                     |                                          |                    ✓                     |                    ✓                     |
| **Hold**   |                                           |                    ✓                     |                    ✓                     |                                          |
| **Aim**    |                     ✓                     |                                          |                    ✓                     |                    ✓                     |
| **Trace**  |                                           |                                          |                    ✓                     |                                          |




| Verb           | Tap                                              | Mechanic            | Ref |
| -------------- | ------------------------------------------------ | ------------------- | --- |
| **Tap**        | Chạm đúng thời điểm                              | Normal Note         |     |
| **Hold**       | Chạm và giữ                                      | Hold Note           |     |
| **Release**    | Nhả tay đúng thời điểm                           | Hold completion     |     |
| **Trace**      | Di chuyển ngón theo đường                        | Arc                 |     |
| **Switch**     | Chuyển tay / chuyển vị trí                       | Arc + note patterns |     |
| **Alternate**  | Đổi tay liên tục                                 | Pattern             |     |
| **Slide**      | Trượt theo hướng                                 | Arc / Trace         |     |
| **Catch**      | Đón note đang rơi                                | Note timing         |     |
| **Coordinate** | Điều khiển nhiều input đồng thời                 | Multi-note / Arc    |     |
| **React**      | Phản ứng với note xuất hiện ở vị trí/độ cao khác | Spatial chart       |     |
| **Maintain**   | Duy trì input trong một khoảng thời gian         | Hold / Arc          |     |
| **Release**    | Kết thúc input chính xác                         | Hold / Arc          |     |
| **Aim**        | Đưa input tới đúng vị trí                        | Spatial Arc         |     |
| **Follow**     | Bám theo chuyển động của Arc                     | Arc movement        |     |

> Với sự xuất hiện của Note tầng trên, combo verbs đã dày hơn rất nhiều. Đây chính là thứ tạo nên nét độc đáo của Arcaea.


Tôi rất thích ý tưởng Verb + Object → Dynamics.

Đừng chỉ ghi:
Game A có Hold Note, Flick Note, Swipe Note.

Mà break thành:
Verb
Tap
Hold
Release
Swipe
Flick
Drag
Dodge
Aim
Collect
Chain...
Object
Note
Lane
Enemy
Beat
Obstacle
Multiplier...

Sau đó:
Verb + Object → Interaction → Dynamics

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

## 3. Art / Visual Design
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

## 4. Audio — bạn chưa có kinh nghiệm thì tôi nghĩ đừng cố phân tích theo kiểu Audio Designer

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

## 5. Meta
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

## 6. Quan trọng nhất: cuối mỗi game phải có "What We Learn"
Đây là phần tôi nghĩ bạn **nên bắt buộc có**.

Sau khi phân tích:

> **Problem → Core → Visual → Audio → Meta**

Cuối cùng phải trả lời:
### What does this teach us about Magic Tiles?

Ví dụ:
**Learn #1 — Gameplay**
> Rhythm mechanics become more memorable when chart structure mirrors the musical structure.

**Learn #2 — Visual**
> VFX should escalate with musical intensity rather than being constant decoration.

**Learn #3 — Audio**
> SFX can communicate mastery, not just input confirmation.

**Learn #4 — Meta**
> Song catalogue can become a progression/collection system rather than simply a content list.

### → MT3 Opportunity

> **Potentially combine these into:**  
> Musical build-up → mechanic escalation → visual/audio escalation → mastery moment → reward/progression.

**Đây mới là output Amanotes cần.**
