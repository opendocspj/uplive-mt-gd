# Các vấn đề chính
**Bài toán mà Magic Tiles đang gặp:**
- Game rất dễ bắt đầu, nhưng chưa đủ chiều sâu để trở thành một game mà người chơi có thể “master” trong thời gian dài.
- Skill của player có tăng, nhưng game **không show ngược skill đó cho player**. Hiện tại progression chủ yếu dừng ở việc player tự chơi giỏi hơn, vì vậy mastery motivation chỉ ở mức partial, còn milestone/mastery progression rất yếu.
- Mechanic/pattern mới phải làm gameplay gắn chặt hơn với musical structure.
- Catalogue âm nhạc chưa tham gia vào meta mặc dù có lợi thế về asset song cực lớn.
- Không có đủ identity/self expression.
- Playbook cho rằng artist fandom/music culture / short-form video gần như là một channel chưa được build.

Kết hợp với playbook. Ta có thể tóm gọn lại 3 vấn đề cần giải quyết của Magic Tiles

**CORE PROBLEM**
>Easy to learn nhưng skill/mastery bị cap.
>Chưa có kết nối với meta.

**META PROBLEM**
>Thiếu hệ thống Meta + Progression + Identity + Collection + Social

**MONETIZE PROBLEM**
>Thiếu động lực trả tiền cho giai đoạn sau này (motivation fit)

# Hướng tiếp cận
*Giải quyết từng phần : CORE > META > MON.*

## Core Gameplay

> [!NOTE]
> **CORE PROBLEM**
> >Easy to learn nhưng skill/mastery bị cap.
> >Chưa có kết nối với meta.

### Hệ thống Note
Magic Tiles hiện đã có đủ mechanics để xây dựng một hệ thống gameplay sâu. Vấn đề nằm ở cách chart kết hợp và khai thác chúng.

Tuy vậy, chart hiện tại áp dụng các mechanics này chưa tốt, dẫn đến game có nhiều mechanics nhưng không đủ sâu để tạo ra identity cho dòng.

Để dễ hiểu hơn, ta có thể lấy thí dụ về dòng game Match 3, core game match 3 ở đâu cũng giống nhau nhưng trên thị trường lại có đủ loại: Royal Match, Candy Crush Soda, Candy Crush Saga, Homescapes, Fishdom...
Mỗi một dòng match 3 đều cho một cảm giác chơi rất khác nhau: RM thì hướng đến cảm giác bùng nổ, Homescapes khó hơn thiên về giải tầng đáy nhiều hơn, Candy Crush Saga có blocker rất khó chịu... 

Với cùng cách tiếp cận như vậy. Ta sẽ đưa ra một vài phương án tiếp cận để tạo ra "màu" trong series magic tiles này.

Trước tiên, hệ thống Note của Magic Tiles được hiểu như sau:

| Note →     |                   Tap                    |               Special Tap                |                   Long                   |                  Flick                   |                   Trace                   |                   Rapid                   |
| ---------- | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :---------------------------------------: | :---------------------------------------: |
| **Verb ↓** | ![[Pasted image 20260815143534.png\|78]] | ![[Pasted image 20260815143721.png\|62]] | ![[Pasted image 20260815143546.png\|80]] | ![[Pasted image 20260815143606.png\|62]] | ![[Pasted image 20260815143859.png\|114]] | ![[Pasted image 20260815143837.png\|137]] |
| **Tap**    |                    ✓                     |                    ✓                     |                    ✓                     |                    ✓                     |                     ✓                     |                     ✓                     |
| **Hold**   |                                          |                                          |                    ✓                     |                                          |                     ✓                     |                                           |
| **Flick**  |                                          |                                          |                                          |                    ✓                     |                                           |                                           |
| **Trace**  |                                          |                                          |                                          |                                          |                     ✓                     |                                           |

Nhìn vào bảng và design chart hiện tại. Ta có thể thấy rất rõ ràng lý do tại sao game lại dễ tiếp cận nhưng content để master chưa đủ sâu.

Nếu quy về Verb (hành động của người chơi), chart trong game hầu hết chỉ bắt người chơi **Tap** và **Hold**. **Flick** và **Trace** ít khi xuất hiện dù ở các bài khó. 

### Core Design của Chart
*Magic Tiles không nhất thiết cần thêm mechanics. Magic Tiles cần một “chart language” riêng.*

Đầu tiên, nhìn vào library ta có thể thấy cách họ xây dựng identity của mình:
- [[Beatstar (404)#Core Mechanics|Beatstar Core Gameplay]] chart giới hạn trong 3 track, content khó nhất là **Flick**.
- [[Bandori (404)]] có hệ thống **Flick** và **Tap** sâu nhất. 
- [[Project Sekai (404)]] có hệ thống **Trace** phức tạp và thú vị nhất.
- [[Arcaea#Core Mechanics]] có vùng sky input kết hợp với **Trace** tạo nhiều biến thể nhất. 

Suggest lựa chọn dùng **Flick** để làm identity game. Vì:
- Dễ tạo ra nhiều biến thể. Flick + direction sẽ tạo ra tới 8 note mới mà người chơi không cần học lại (low learning cost). Từ đó mở rộng không gian biểu đạt của chart.
- Không chọn Trace vì không gian **màn hình dọc không phù hợp** để **Trace**. Đây cũng có thể là lí do mà Beatstar không có dạng note này.
- **Trace** mạnh khi game có đủ không gian để người chơi thực hiện các gesture dài/liên tục.
- Với màn hình dọc và core của MT, Trace dễ trở thành mechanic chiếm nhiều diện tích nhưng lại phá chart nếu không dùng đúng thời điểm.
- Trong khi đó, Flick có thể xuất hiện ở bất cứ thời điểm nào trong bài mà vẫn đảm bảo chart hoạt động đúng ý đồ.

Tuy vậy, Flick đã được Beatstar sử dụng, nên ta sẽ coi Flick là một interaction layer có thể kết hợp với các loại note khác.

> **Mục tiêu là tạo ra một interaction mà người chơi phải đồng thời đọc “Note” và “Direction” của nó, từ đó hình thành một chart language riêng cho MT.**

Flick có thể được kết hợp với các note khác như Tap, Hold, Trace... để tạo ra những interaction mới.

| Base Note | + Flick     | Interaction                     |
| --------- | ----------- | ------------------------------- |
| Hold      | Hold Flick  | **giữ + vuốt**                  |
| Trace     | Trace Flick | **trace + đổi hướng rồi flick** |
| Rapid     | Rapid Flick | flick liên tục                  |

>Beatstar đã chứng minh Flick chart work. MT chỉ cần mang những bài học đó áp dụng vào một design space lớn hơn. Lúc này, chart của MT sẽ có một identity riêng, vừa quen thuộc vừa mới lạ so với Beatstar.

### Chart Design
*Sau khi đã có core design rồi, việc tiếp theo là tạo các pattern để xếp vào bài hát.*

Nếu coi từng Note tượng trưng cho Verb thì để ghép thành Grammar, các Note cũng phải sắp xếp một cách có chủ đích.

**Define Pattern Grammar:**
Mỗi Pattern sẽ được làm thủ công bằng tay. Ngoài việc phải bám theo nhạc, mỗi pattern cần đạt đủ các tiêu chí ở mỗi mục.
Các tiêu chí hầu hết đều có thể nới lỏng, nhưng tiêu chí số lượng Input Flick phải được qui định chặt chẽ (do ta đã xác định Flick là core design của chart).

Đây chính là library pattern design của game để tạo chart. Vì thời lượng giới hạn, người viết chỉ liệt kê một số mẫu tham khảo. 

1. **Pattern để Build Tension**
Mục tiêu: làm người chơi cảm thấy bài đang nhanh/dồn lên. Cần :
- Có Alternating.
- Note sắp xếp thấy rõ sự lặp lại.
- Khoảng cách giữa các note ngắn dần.
- Cuối pattern là khoảng nghỉ.
- **Số Input Flick không vượt quá 1/8 pattern.** 
- Kết pattern thường là Flick.

2. **Pattern để Climax**
Mục tiêu: tạo signature moment của bài. Cần:
- Kết hợp hoàn toàn mới của **Flick với các note khác**: Hold + Flick, Trace + Flick... theo các hướng khác nhau và cách sắp xếp khác nhau (tuỳ vào bài). **Số lượng input Flick** phải xuất hiện **trên 50%** thời lượng pattern.
- Có sự tương phản rõ rệt với pattern trước đó (thường là Build Tension).
- Pattern có tính bất ngờ nhưng vẫn đọc được.
- Nên đặt vào musical accent mạnh: Drop, Chorus, Beat mạnh...

3. **Pattern để Tutorial**
Mục tiêu: Được làm dựa trên Climax hoặc MON. Cần:
- Pattern đơn giản hơn phiên bản Climax.
- Chỉ introduce **một concept mới tại một thời điểm**.
- Có Alternating để người chơi làm quen với nhịp và lane.
- Không đặt quá sát tutorial với các pattern khác.
- Lặp lại đủ nhiều để người chơi hình thành muscle memory.
- **Số Input Flick không vượt quá 50% số Input Flick có trong Climax.** 

4. **Pattern MON** (Optional)
Mục tiêu: Phục vụ cho **Monetize**, tạo ra một đoạn gameplay khó nhất của chart (Ép người chơi thua). Cần:
- Có **Difficulty cao nhất** so với các pattern còn lại.
- Sử dụng **Core Mechanics** ở mức độ phức tạp nhất.
- Ưu tiên **combination** giữa các mechanic, đặc biệt là các **Flick combination**.
- Có **Intensity tăng dần** trước khi bước vào pattern.
- Đặt ở **nửa sau bài hát (>50%)**.
- Có **payoff rõ ràng** sau khi hoàn thành.
- **Số lượng Input Flick phải trên 70% Pattern**.

5. **Pattern để Release**
Mục tiêu: giải tỏa sau một đoạn khó (thí dụ: climax). Cần:
- Giảm density.
- Giảm complexity.
- Có khoảng nghỉ rõ ràng.
- Số Input Flick chỉ được nằm trong khoảng **12.5%~25%** pattern.


---

Ta đã có Pattern và công dụng của nó (Grammar và cách dùng).
Giờ là lúc design full chart (ghép thành đoạn văn). 
Hướng design: 
1. Xác định **musical structure** (để gán pattern):
	- Intro
	- Verse
	- Pre-chorus
	- Chorus
	- Bridge
	- Drop
	- Outro
2. Đánh dấu các phần (để design pattern):
	- Beat mạnh/yếu.
	- Vocal phrase.
	- Kick / snare / hi-hat.
	- Musical accent.
	- Điểm làm bài hát tăng/giảm năng lượng.
	- Ý đồ riêng.
	- ...
3. Tạo đường cong trải nghiệm. Từ đây chart có **progression**. Thí dụ:
	- Intro = Pattern Tutorial
	- Verse = Pattern Flow
	- Pre-chorus = Pattern Build Tension
	- Chorus = Pattern Climax 
	- Final Chorus = Pattern MON
	- Outro = Pattern Release
4. Tóm tắt lại chart. Phần này **rất quan trọng**, nó sẽ **dùng cho monetize** và **Build User Journey** (meta progression). 
	- Difficulty. 
	- Playtime. Yêu cầu 1 bài bắt buộc phải nằm trong khoảng 80s trở lên. (Xem thêm Meta)
	- Core Mechanics: Các note nào có trong bài.
	- Intensity Moment: **đoạn dễ thua nhất ở thời điểm nào.** Yêu cầu moment này phải đặt ở nửa sau của bài hát (>50%). (Xem thêm Meta). Chú ý: Pattern Climax không có nghĩa phải là pattern khó nhất. 
	- Mastery: mechanic/pattern nào cần người chơi thành thạo để hoàn thành chart. Đây là phần đặc biệt, không phải chart nào cũng cần phân tích. (Xem thêm User Journey). 
	- **Tỉ lệ hoàn thành (chờ data).**

### Kết luận về cách tiếp cận Core Gameplay
Mục tiêu của toàn bộ phần này:
- **Giữ Learning Curve thấp** nhưng **tăng Depth** thông qua **Pattern Complexity**.
- Core gameplay có mức trần cao hơn. Chart được build lại có ý đồ hơn -> **Replay Value cao hơn** trước. 

## Meta 
*Đây là cách hệ thống vận hành chứ không phải game design document.*

> [!NOTE]
> **META PROBLEM**
> >Thiếu hệ thống Meta + Progression + Identity + Collection + Social

**Meta được design tập trung hoàn toàn vào Retry Economy.**

### Giới thiệu hệ thống mới

**Mô tả:**
- Đầu tiên, ta cần tạo ra 1 token mới: **FIRE**. Fire được dùng để **mua nhạc** và mọi thứ khác sau này.
- Nhạc trong game sẽ được quy hoạch lại. Chia làm 2 phần chính: 
	- Nhạc mở khoá sẵn. 
	- Nhạc mua bằng Fire.
- Chơi nhạc sẽ nhận được Fire. **Độ khó càng cao** Fire nhận được càng nhiều.
- Hệ thống trong game sẽ được chia làm **2 Mode** rõ rệt:
	- **Practice Mode**. Trong này chứa toàn bộ collection nhạc của người chơi. Người chơi có thể chơi thoải mái. **Chơi trong practice mode vẫn nhận được một lượng nhỏ Fire sau mỗi bài.**
	- **Playlist Mode**. Chế độ mới. **Nơi kiếm Fire.**
- **Playlist Mode:**
	- Mỗi ngày, người chơi sẽ có 1 playlist nhiệm vụ. 
	- Playlist này yêu cầu họ chơi các bài theo thứ tự: A - B - C - D. 
	- Các bài này có thể có **hoặc không có** trong library của người chơi.
	- **Hoàn thành mỗi bài, người chơi sẽ được +1 streak, thua thì mất hết streak và bắt buộc phải sang bài tiếp theo.** Max 10 Streak. Nghĩa là, người chơi chỉ có 1 cơ hội mỗi bài.
	- Streak được dùng để multiply **FIRE** nhận được khi chơi nhạc ở chế độ playlist.
	- Vì mỗi ngày chỉ có hữu hạn bài trong playlist, nên Fire kiếm được gần như là hữu hạn.
- Cuối cùng, người chơi dùng Fire kiếm được để mua nhạc và các vật phẩm khác trong cửa hàng. 

![[Pasted image 20260816011859.png]]
*Sơ đồ tối giản của hệ thống meta mới. Xem file gốc [[MT Meta Visualize.canvas|MT Meta Visualize]].*

**Hệ thống Playlist Mode mới:**
- **Tạo ra pain point mới: Streak, và Fire.**
- Người chơi luôn lo sợ mình sẽ mất streak khi gặp chart mới. Như vậy chúng ta sẽ bán được retry, shield, booster cho playlist.
- Playlist cho người chơi thử những bài họ chưa sở hữu, lúc này họ muốn FIRE.
- Cửa hàng thậm chí còn bán những Chart đặc biệt được thiết kế kĩ lưỡng. 
- Ép người chơi tích luỹ Fire, vào game daily.
- Không làm cấu trúc game thay đổi quá nhiều.
- Ngoài ra, đây là base để build các tầng MON sâu hơn.

Tại đây, playlist đã tạo ra nhu cầu để người chơi bỏ tiền vào mua các content meta thông thường. VD: Daily Quest, Battle Pass, 7 Day Login... 

Tuy vậy, đây chỉ là những bước mid term journey.
### Bức tranh về Long Term Journey
*Một khi đã trở nên giỏi hơn, người chơi càng muốn thể hiện bản thân.*

**Mô tả:**
- Khi người chơi đã quen với Playlist Mode, họ sẽ cần một thứ gì đó khác biệt để tạo cảm giác mới mẻ.
- Đây là lúc đưa Event vào.
- Mechanics của Event như thế nào sẽ không bàn tới. Miễn Event bắt người chơi phải chơi core game là được. Thí dụ:
	- Event có 1 playlist riêng, dài gấp đôi playlist bình thường. 
	- Token nhận được trong event chỉ được dùng trong event.
	- Token Event dùng để đổi đồ trong shop event. Shop bán fire shield, bán retry, bán song exclusive và bán card.
- Điểm chính: mỗi event, người chơi sẽ kiếm được 1 collection card.
- **Card này là duy nhất. Nếu bỏ lỡ event thì không thể kiếm lại.**
- Card sẽ cộng chỉ số cho người chơi. VD:
	- Tăng 1% Fire kiếm được.
	- Tăng 1% Token Event.
	- Giảm 1% giá trong cửa hàng Event.
	- ...
- Card stack với nhau mãi mãi. **KHÔNG GIỚI HẠN.**
- Card có thể dùng FIRE để craft lên Card đẹp hơn. VD trong event chỉ kiếm được Card Gỗ, người chơi cần dành rất nhiều FIRE để upgrade nó lên Card DIAMOND.
- Card càng cao thì **hiệu ứng càng đẹp**. Từ lấp lánh, khung viền, animation bên trong Card. Tham khảo video bên dưới: Mavel Snap Card Upgrade.

![[MAX card upgrade (Common to Infinity) in MARVEL Snap [Ro7CVCb-pi8].mp4]]

*Mavel Snap Card Upgrade (video ref)*

---
**Hệ thống Card có thể:**
- Đặt lên profile
- Showcase card 
Card cấp cuối trở thành **social status** cho những player trên BXH.

Như vậy, toàn bộ hệ thống meta chính đã hoàn thiện. 

| Giai đoạn         | Người chơi đang muốn                                      | Meta đáp ứng bằng                      |
| ----------------- | --------------------------------------------------------- | -------------------------------------- |
| **Early Game**    | **Chơi vui + khám phá + tiến bộ**                         | Song, Practice, FIRE, Song Unlock      |
| **Mid Game**      | **Chơi giỏi + tối ưu progression + sở hữu nhiều hơn**     | Playlist, Streak, FIRE, Collection     |
| **Late/End Game** | **Challenge + Collection + Prestige + thể hiện bản thân** | Event, Card, Card Upgrade, Leaderboard |

## **MONETIZE** 
*Người chơi có động lực chơi game nhờ tính năng nào, và ta có thể làm gì để kiếm tiền từ chúng.*

> [!NOTE]
> **MONETIZE PROBLEM**
> >Thiếu động lực trả tiền cho giai đoạn sau này (motivation fit)

### EARLY GAME
**Primary motivations:**
- **Discovery**
- **Progression**
- **Collection**

> “Tôi muốn khám phá game, chơi tốt hơn và mở thêm content.”

Điểm kiếm tiền:
- **FIRE Pack**: mua thêm FIRE để unlock Song.
- **Song Bundle**: bundle nhiều bài.
- **Premium/Exclusive Song**: bài chỉ mua bằng tiền.
- **Starter Pack**: FIRE + một số Song hấp dẫn.

**Funnel:**
> Play Song -> thích Song -> muốn sở hữu -> thiếu FIRE -> **Purchase**

**Điểm mạnh:** monetization dựa trên **content**. Nhưng Chart lúc này phải làm tốt mới có thể bán được.

### MID GAME
**Primary motivations:**
- **Mastery**
- **Challenge**
- **Progression**
- **Loss Aversion**

> “Tôi đã hiểu game rồi. Giờ tôi muốn chơi tốt và tối ưu progression (cơ chế độ khó càng cao Fire càng nhiều và Streak Lost)”

Đây là giai đoạn **Streak quan trọng**, đánh dấu việc người chơi hoàn toàn hook vào meta. Nó biến Mastery thành một thứ có consequence. **Chơi giỏi thì kiếm được càng nhiều Fire!**

Điểm kiếm tiền:
- Mua **Fire Shield/Streak Protection**.
- Retry Ticket.
- FIRE Multiplier.
- Playlist Reset. Một ngày có thể chơi nhiều hơn một Playlist.

### LATE GAME
**Primary motivations:**
- **Challenge**
- **Collection**
- **Completion**

> “Tôi đã có phần lớn content. Hãy cho tôi thứ khó hơn và thứ để sưu tầm.”

Đây là lúc **Event** trở thành monetization engine.

Điểm kiếm tiền:
- Battle Pass.
- Event Token Boost.
- Exclusive Song.
- Card

### END GAME
**Primary motivations:**
- **Status**
- **Social Competition**
- **Completion**
- **Self-expression**
- **Mastery**

> “Tôi đã chơi rất lâu. Bây giờ tôi muốn thành tích của mình có giá trị và được nhìn thấy.”

Điểm kiếm tiền:
- Card Cosmetic Upgrade. (Sink của FIRE).
- Profile Customization
	- Card Showcase.
	- Profile background.
	- Nameplate.
	- Special title.
	- Animation.
	- Showcase slot.
- Leaderboard

# Next Step (as a Game Designer)
*Các hệ thống chính của game vẫn có thể giữ lại. Trừ những thứ sau*
## 0. Some Art Tuning
Đồng bộ lại toàn bộ art game. 
Nếu xác định sau này sẽ bán cosmetic cho end-game player. Ta nên đồng bộ style của tất cả các bài, tránh mỗi bài một kiểu sẽ khiến game thiếu đi độ nhận diện.

Nếu đã chọn Flick làm identity thì đây là phần **phải đầu tư mạnh nhất**.
- Mũi tên trên note sẽ chuyển động theo hướng flick.
- Khi flick đúng, note bị kéo văng theo hướng flick.
- Particle/trail cũng chạy theo flick.

Rapid Tap nên có thêm
- Càng tap càng rung/càng to.
- SFX khi tap cao dần.
- Particle tăng dần.
- Background reaction tăng dần
Mục đích là tạo cảm giác **đang build tension -> đạt đỉnh -> release**. (ref muse dash).

## 1. Chốt Chart Design Guideline
Framework trong bài phân tích.
> Note → Verb → Pattern → Grammar → Full Chart → Musical Structure → Experience Curve

**Các đầu mục:**
- [ ]  Chốt **Flick là chart identity**
- [ ]  Define toàn bộ Flick interaction
    - Flick direction
    - Hold + Flick
    - Rapid + Flick
    - Các combination khác
- [ ]  Làm **Pattern Library**
    - Tutorial
    - Flow
    - Build Tension
    - Climax
    - MON
    - Release
    - ...
- [ ]  Define rule cho từng pattern
    - density
    - complexity
    - Flick %
    - lane usage
    - alternating
    - repetition
    - ...
- [ ]  Define guideline để chart bám vào nhạc và phục vụ cho meta (các con số trong bài đều là giả thiết).
- [ ]  Define lại độ khó của bài **Easy / Medium / Hard / Expert**. 

**Output cuối cùng là một Chart Guideline Document** mà trong đó có tính toán số liệu thực tế phù hợp với các GATE mà playbook đánh giá.

## 2. Làm chart level cao dựa theo guideline
Nên chọn khoảng **10–20 bài đại diện** và làm thêm chart mới.

## 3. Xử lí content cũ
Chia content cũ thành 3 nhóm:

**Legacy Content**
Các chart cũ giữ nguyên. Dùng cho:
- Early game
- Practice
- onboarding
- người chơi casual
- filler content

**Rework Content**
Những bài cũ **có tiềm năng về song/chart** thì remake theo guideline mới.

**Premium Content**
Chart được thiết kế **100% theo guideline mới**. Là content có giá trị cao nhất, có thể dùng cho:
- Playlist
- Event
- Hard/Expert
- Shop
- Exclusive Song
- Monetization

## 4. Measurement
Guideline cuối cùng phải được chứng minh bằng data.

Cần tìm ra sweet spot để đặt các điểm ép fail trong bài hát (Pattern MON).
Hiện tại, thời điểm intensity của bài ở >50% thời gian bài chỉ là giả thiết. Nếu 80% player fail ở 36% bài thì MON đặt ở 50% không có ý nghĩa.

