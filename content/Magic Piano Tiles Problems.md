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
>Easy to learn nhưng skill/mastery bị cap

**META PROBLEM**
>Thiếu hệ thống Meta + Progression + Identity + Collection + Social

**MONETIZE PROBLEM**
>Thiếu User Journey (mastery motivation fit)

# Hướng tiếp cận
*Giải quyết từng phần : CORE > META > MON.*

## Core Gameplay
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
- [[Beatstar#Core Mechanics|Beatstar Core Gameplay]] chart giới hạn trong 3 track, content khó nhất là **Flick**.
- [[Bandori]] có hệ thống **Flick** và **Tap** sâu nhất. 
- [[Project Sekai]] có hệ thống **Trace** phức tạp và thú vị nhất.
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
3. Tạo đường cong trải nghiệm của chart. Từ đây chart có **progression**. Thí dụ:
	- Intro = Pattern Tutorial
	- Verse = Pattern Flow
	- Pre-chorus = Pattern Build Tension
	- Chorus = Pattern Climax 
	- Final Chorus = Pattern MON
	- Outro = Pattern Release
4. Tóm tắt lại chart. Phần này **rất quan trọng**, nó sẽ **dùng cho monetize** và **Build User Journey** (meta progression). 
	- Difficulty. 
	- Playtime. Yêu cầu 1 bài bắt buộc phải nằm trong khoảng 80s trở lên. (Xem thêm Meta)
	- **Tỉ lệ hoàn thành (RẤT QUAN TRỌNG, xem cách check bên dưới).**
	- Core Mechanics: Các note nào có trong bài.
	- Intensity Moment: **đoạn dễ thua nhất ở thời điểm nào.** Yêu cầu moment này phải đặt ở nửa sau của bài hát (>50%). (Xem thêm Meta). Chú ý: Pattern Climax không có nghĩa phải là pattern khó nhất. 
	- Mastery: mechanic/pattern nào cần người chơi thành thạo để hoàn thành chart. Đây là phần đặc biệt, không phải chart nào cũng cần phân tích. (Xem thêm User Journey). 
	- Memorable Moment: hãy mô tả chart này bằng một câu ngắn, nói ra được cái hay của chart. VD: 



Action
- Làm thêm độ khó.
- Làm chart level cao dựa theo guideline.
- Chart legacy phù hợp làm chart beginner.



monetize việc "muốn sở hữu và hoàn thiện collection"

vụ meta weekend album ok đấy
song streak như booster ý
**meta**
tiếp cận dần dần, test xem ok ko đã mới đến cosmetic.

- tạo ra 1 token mới: FIRE. Fire để mua song và mọi thứ khác.
- quy hoạch rõ ràng bài nào unlock được bài nào phải mua bằng FIRE.
- mỗi ngày sẽ có 1 playlist, yêu cầu chơi các bài A - B - C - D. các bài này có thể có hoặc ko có trong lib của người chơi.
- hoàn thành bài thì +1 streak, thua thì mất hết streak. đi sang bài tiếp theo, ko được thử lại bài cũ.
- streak dùng để multiply FIRE nhận được khi chơi.
- độ khó càng cao fire càng nhiều.
- vì mỗi ngày chỉ có hữu hạn bài trong playlist, nên fire kiếm được là hữu hạn.
- gate monetize ở: FIRE, ép phải chơi daily.

Làm sao khiến người chơi muốn mua một bài hát mà họ chưa biết mình có thích hay không?
Tại sao người chơi lại cần FIRE ngay từ đầu?
→ Song ownership

“Làm sao khiến người chơi liên tục rơi vào những tình huống mà họ _muốn có FIRE_?”

1. Muốn chơi bài
→ Đây là motivation mạnh nhất.

2. Muốn sở hữu bài
→ Collection motivation, nhưng yếu hơn việc được chơi.

3. Muốn retry để thắng bài
→ Motivation cực mạnh nếu người chơi đã hình thành attachment với bài/run.

**Song phải liên tục tạo ra desire.**

**mở rộng meta:**
- Fire shield
- Retry token
- Booster khi chơi playlist

Badges
Score card để share

permanent meta

- mỗi event, khi hoàn thành nhiệm vụ người chơi sẽ kiếm được 1 collection card.
- card này nếu bỏ lỡ thì không thể kiếm lại.
- card này cộng stats. hiện tại mới chỉ có FIRE, nên card sẽ tăng bonus Fire khi hoàn thành card. VD: +3 fire each song earned, +0.1% Fire...
- card này stack với nhau mãi mãi ko giới hạn.
- mỗi event sẽ có 1 gameplay khác nhau. nhưng chủ yếu là người chơi vẫn phải chơi core game. VD: event sẽ có 1 playlist event riêng, dài gấp đôi playlist bình thường. token nhận được là token event ko phải song. dùng token event mua trong shop event. shop event bán card, bán fire shield, bán retry, bán song exclusive.
- card trong event có thể craft lên thẻ đẹp hơn, không có tác dụng gì. craft bằng FIRE. trong event chỉ kiếm được thẻ gỗ, người chơi cần dành phần lớn FIRE để upgrade nó lên thẻ DIAMOND.

Có thể:
- đặt card lên profile
- showcase card 
- card có animation
- người khác xem collection
Diamond trở thành **social status**.

Build 1 concrete vertical slice chứng minh rằng core gameplay mới có thể trở thành nền móng cho progression + economy + monetisation.

Bạn cần đi từ Core Loop → Beatmap → Progression → Monetization
Ví dụ:
Core Loop
Choose Song → Play → Master → Reward → Upgrade/Unlock → Replay

Sau đó chọn một bài cụ thể:
Song X
và thiết kế:

Beatmap
Pattern A ở intro
Pattern B ở verse
Pattern C ở chorus
Mechanic X xuất hiện ở build-up
Special moment ở drop
Difficulty curve như thế nào
Feedback/VFX/animation như thế nào
