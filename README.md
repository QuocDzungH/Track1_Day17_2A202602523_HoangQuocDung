# Bài lab: Problem Interview - Case A

## 1. Thông tin cá nhân và nhóm

- **Họ và tên:** Hoàng Quốc Dũng
- **Mã học viên (MHV):** 2A202602523
- **Tên nhóm:** Prompt Kiếm Tông
- **Thành viên nhóm:**
  - Hoàng Quốc Dũng
  - Trần Đình Hinh
  - Đinh Xuân Quyền
- **Case đã chọn:** Case A — AI Tutor: Diagnostic Refresher

## 2. Problem Hypothesis Brief (Kết quả Chặng 1)

### 2.1. Solution — Gỡ solution khỏi hình thức cụ thể
- **Solution directive (Nguyên văn Case A):** Thêm nút “Tôi vẫn chưa hiểu” vào bài học. Khi học viên bấm nút, AI Tutor sử dụng nội dung bài hiện tại, các câu trả lời gần đây và lịch sử học tập để: 1. Đặt 2–3 câu hỏi chẩn đoán ngắn. 2. Chọn một khái niệm nền để học viên ôn lại. 3. Tạo một phần giải thích ngắn. 4. Đưa học viên trở về bài đang học.
- **Capability trung tính:** Cung cấp sự hỗ trợ tức thời để chẩn đoán và khắc phục lỗ hổng kiến thức nền tảng ngay tại điểm người học gặp khó khăn, giúp họ tiếp tục tiến độ học tập.

### 2.2. Change — Chuỗi thay đổi được kỳ vọng
`Solution (Chẩn đoán & ôn kiến thức nền tại chỗ) → Người học phát hiện được gốc rễ phần kiến thức bị hổng và hiểu bài ngay → Không bị gián đoạn mạch học, không nản chí → Outcome (Tăng tỉ lệ hoàn thành bài học, hiểu bài sâu sắc và tự tin hơn)`
- **Các thay đổi được kỳ vọng:**
  1. Người học nhận diện được chính xác khái niệm tiên quyết (prerequisite) mà mình đang thiếu thay vì đoán mò.
  2. Thời gian loay hoay tìm kiếm tài liệu giải thích giảm từ hàng chục phút xuống chỉ còn vài phút.
  3. Người học giảm cảm giác hoang mang, sợ tụt hậu và không bỏ cuộc giữa chừng.

### 2.3. Actor — Xác định các nhóm người liên quan
| Actor | Họ đang làm gì? | Pain hoặc hậu quả có thể có | Họ hưởng lợi thế nào? |
| :--- | :--- | :--- | :--- |
| **Learner (Học viên)** *(Chọn điều tra)* | Tự học hoặc nghe giảng, làm bài tập | Kẹt bài, không biết mình hổng chỗ nào, sợ tụt lùi, nản chí | Được gỡ rối tức thì, theo kịp bài học |
| **Instructor / Giảng viên** | Soạn bài, giảng bài, trả lời thắc mắc | Bị quá tải khi nhiều học viên hỏi cùng câu hỏi cơ bản, ngắt quãng giờ giảng | Giảm tải việc giải đáp lặp đi lặp lại kiến thức nền |
| **Course Designer / Platform** | Tối ưu nội dung khóa học | Tỷ lệ drop-off cao ở các bài tập/khái niệm khó | Tăng retention rate và mức độ hài lòng của người học |

- **Actor nhóm chọn để điều tra trước:** Learner (Người học trực tiếp).
- **Vì sao chọn nhánh này:** Learner là người trực tiếp trải nghiệm sự bế tắc và chịu hậu quả trực tiếp (mất động lực, tụt hậu, bỏ học). Nếu không hiểu rõ hành vi tự xoay xở của learner thì mọi giải pháp hỗ trợ đều vô nghĩa.

### 2.4. Situation & Job
- **Mô tả Situation & Job:** Khi đang học bài mới và gặp một khái niệm hoặc bài tập khó hiểu, người học đang cố gắng tự hiểu và vượt qua điểm nghẽn bằng cách đọc lại tài liệu, tra cứu mạng hoặc hỏi người khác.
- **JTBD Hypothesis:** Khi gặp một khái niệm hoặc bài tập không hiểu trong lúc học, tôi muốn nhanh chóng gỡ rối và nắm được bản chất vấn đề, để có thể tiếp tục mạch học mà không bị nản chí hay tụt lùi so với tiến độ.

### 2.5. Pain — Hai cách giải thích cạnh tranh
- **Pain Hypothesis A (Giả thuyết kiến thức nền - Nhóm chọn):** Khi gặp một khái niệm/bài tập khó, người học gặp khó khăn trong việc hoàn thành bài học vì **không tự xác định được lỗ hổng kiến thức nền tảng của mình** (không biết những gì mình không biết), dẫn đến việc tra cứu mông lung, mất nhiều thời gian và dễ nản chí bỏ cuộc.
- **Pain Hypothesis B (Giả thuyết cách diễn đạt/tài liệu - Cạnh tranh):** Khi gặp khái niệm khó, người học không hiểu bài là vì **cách diễn đạt của giảng viên/tài liệu quá trừu tượng hoặc thiếu trực quan**, chứ không phải do thiếu kiến thức nền; chỉ cần một ví dụ minh họa trực quan hoặc một góc nhìn giải thích khác là hiểu ngay.
- **Giả thuyết nhóm chọn để điều tra trước:** Hypothesis A.
- **Lý do chọn:** Hypothesis A phản ánh giả định cốt lõi của tính năng "Diagnostic Refresher" (cần chẩn đoán kiến thức nền). Cần kiểm tra xem người học thực sự kẹt do kiến thức nền hay do nguyên nhân khác.

### 2.6. Evidence — Xác định điều cần tìm trước khi viết câu hỏi
| Cần kiểm tra | Evidence làm nhóm tin hơn | Evidence làm nhóm nghi ngờ hoặc bác bỏ |
| :--- | :--- | :--- |
| **Situation có thật** | User nhớ rõ tình huống gần đây (môn học cụ thể, slide/bài tập cụ thể) bị tắc nghẽn kiến thức. | User nói chung chung: "Lúc nào khó thì mình hỏi bạn", không nhớ được sự kiện cụ thể nào trong tuần qua. |
| **Pain có ý nghĩa** | Bị kẹt thật sự, cảm thấy bối rối, sợ tụt hậu, tốn nhiều thời gian xoay xở hoặc bỏ dở bài học. | Thấy bình thường, lướt qua luôn không cần hiểu, không ảnh hưởng gì tới việc học. |
| **Workaround tồn tại** | Đã chủ động thử nhiều cách: đọc lại slide, tra cứu từ khóa, hỏi AI, hỏi bạn bè, xem YouTube... | Ngồi đợi hoặc không làm gì cả; có gia sư/người kèm 1-1 giải đáp ngay lập tức. |
| **Consequence tồn tại** | Mất nhiều thời gian, lo lắng, hoang mang, mất mạch bài giảng phía sau. | Không có hậu quả gì, bài thi vẫn qua bình thường dù bỏ qua đoạn đó. |
| **Pattern có lặp** | Tình trạng này xảy ra định kỳ mỗi khi gặp kiến thức mới hoặc học môn có tính logic/kế thừa cao. | Chỉ là sự cố hãn hữu một lần duy nhất do lỗi mạng hoặc tài liệu in mờ. |

- **Điều gì phải đúng để giả thuyết đứng vững:** Người học thực sự có nỗ lực tự xoay xở khi kẹt bài, và việc không nhận diện được căn nguyên lỗ hổng kiến thức là rào cản chính khiến họ mất thời gian.
- **Điều gì có thể khiến nhóm sửa/bác bỏ giả thuyết:** Nếu người học thực tế biết rõ mình thiếu gì và chỉ cần ví dụ minh họa (ủng hộ Pain B); hoặc người học bị cản trở bởi rào cản xã hội/tâm lý (ngại làm phiền người khác) hơn là thiếu khả năng tự chẩn đoán.

### 2.7. Solution Parking Lot
1. **[AI]** Diagnostic Refresher: Đặt câu hỏi chẩn đoán và tóm tắt kiến thức nền tự động (theo directive gốc).
2. **[AI]** Multi-perspective Explainer: Tự động diễn giải lại đoạn văn bản/slide khó hiểu theo 3 cấp độ (cho người mới bắt đầu, ví dụ đời thực, ẩn dụ so sánh).
3. **[Không dùng AI]** Prerequisite Map & Glossary: Sơ đồ tri thức đính kèm cuối mỗi slide/bài học, gắn link nhảy thẳng về khái niệm nền tiên quyết cần nhớ.
4. **[Không dùng AI]** Anonymous Question Box: Nút bấm gửi câu hỏi ẩn danh tức thời đến giảng viên/trợ giảng trong lớp để tránh ngại ngùng làm phiền lớp học.
5. **[AI]** In-lecture Silent Buddy: AI bot trực tiếp giải nghĩa từ khóa/slide ngay trên giao diện học tập theo thời gian thực mà không ngắt quãng bài giảng.

---

## 3. Conversation Guide phiên bản cuối (Đã sửa sau khi luyện - Chặng 2 & 4)

### 3.1. Big 3 Điều quan trọng nhất cần học
| Điều cần học | Evidence cần tìm | Điều gì khiến nhóm xem lại giả thuyết? |
| :--- | :--- | :--- |
| **1. Hành vi xoay xở đầu tiên** | Hành động tức thời khi gặp chỗ khó (tự đọc lại, search, hỏi ai...). | Bỏ qua luôn hoặc có sẵn người kèm giải đáp ngay mà không cần tự mày mò. |
| **2. Quá trình & Rào cản tự tìm hiểu** | Cách họ tra cứu, vì sao chọn công cụ đó thay vì hỏi người khác; rào cản gặp phải. | Dễ dàng tìm ra lời giải đáp trong vài giây mà không gặp bất kỳ khó khăn hay nhầm lẫn nào. |
| **3. Cảm xúc & Hậu quả thực tế** | Cảm giác bế tắc, áp lực tâm lý, thời gian tiêu tốn, mức độ hiểu bài cuối cùng. | Coi việc không hiểu là chuyện nhỏ, không ảnh hưởng gì đến tiến độ hay tâm lý. |

### 3.2. Nội dung Conversation Guide
- **Tiêu chí tuyển người:** Cần nói chuyện với người đang đi học/tự học đã có lúc không hiểu một phần bài học và phải tìm cách xử lý trong vòng 7 ngày gần đây.
- **Recruitment check:** "Trong tuần qua, bạn có lúc nào đang học (trên trường, tự học online...) mà đọc/xem tài liệu nhưng bị khựng lại vì không hiểu một phần nội dung không?"
- **Lời mở đầu:**
  > "Chào bạn, nhóm mình đang làm một bài thực hành nghiên cứu về hành vi học tập. Mình muốn lắng nghe một câu chuyện thực tế gần đây của bạn về cách bạn xử lý khi gặp khó khăn lúc học. Cuộc trò chuyện rất thoải mái, không có đúng sai và chỉ mất tầm 10-15 phút thôi. Bạn cho mình xin phép ghi âm lại để về nhóm nghe lại nhé?"  
  *(TUYỆT ĐỐI KHÔNG NÓI: Nhóm mình đang làm AI chẩn đoán kiến thức, bạn thấy tính năng này thế nào).*
- **Story opener (Neo vào sự kiện cụ thể gần nhất):**  
  > "Kể mình nghe về lần gần nhất bạn đang học mà tự nhiên thấy mình không hiểu bài đi. Lúc đó bạn đang học môn gì, ở hoàn cảnh nào (tự học hay đang ngồi trên lớp)?"
- **Big 3 Questions (Hỏi đào sâu hành vi quá khứ):**
  1. *Hành vi xoay xở:* "Lúc tự nhiên thấy không hiểu đoạn đó, phản xạ đầu tiên của bạn là làm gì tiếp theo?"
  2. *Chi tiết quá trình:* "Tại sao bạn lại ưu tiên xử lý theo hướng đó thay vì các phương án khác (như hỏi thầy cô, hỏi bạn bè)?"
  3. *Hậu quả & Cảm xúc:* "Sau khi làm cách đó, bạn có hiểu được trọn vẹn phần đó không? Cảm giác của bạn lúc bị kẹt và sau khi giải quyết xong như thế nào?"
- **Probe bank (Đào sâu khi user trả lời ngắn):**
  - "Lúc đó chuyện gì xảy ra tiếp theo?"
  - "Bạn đã làm điều đó như thế nào?"
  - "Việc đó làm mất của bạn bao nhiêu thời gian?"
  - "Nếu bỏ qua đoạn đó thì sẽ ảnh hưởng gì đến đoạn sau?"
- **3 Phản xạ khi dữ liệu bắt đầu lệch chuẩn The Mom Test:**
  - *Khi user khen ngợi:* **Deflect** — Cảm ơn ngắn gọn rồi kéo về hành vi thực tế ("Cảm ơn bạn, mà ở lần gần nhất học bài đó thì bạn đã làm thế nào?").
  - *Khi user nói chung chung / tương lai:* **Anchor** — Kéo về quá khứ ("Lần gần nhất chuyện đó xảy ra cụ thể là hôm nào?").
  - *Khi user hiến kế / feature request:* **Dig** — Tìm hiểu gốc rễ nỗi đau ("Ý tưởng đó sẽ giúp bạn làm được gì mà hiện tại bạn chưa làm được?").

## 4. Practice Reflection (Kết quả Chặng 4)
*Đúc kết thực tế từ cuộc phỏng vấn thử nghiệm (bản ghi chép tại `interview/notes.md` và file ghi âm `interview/recording.m4a`):*
1. **Câu hỏi nào đã giúp user kể một tình huống cụ thể?**
   - **Câu hỏi mở đầu neo bối cảnh thực tế:** *"Kể cho mình nghe lần gần đây nhất bạn đang học mà thấy không hiểu bài thì lúc đó bạn đang học môn gì và trong hoàn cảnh nào?"*. Câu hỏi này rất hiệu quả vì giúp người được phỏng vấn lập tức nhớ lại sự kiện gần đây( điều đã được chị Mai hướng dẫn trong bài là tốt hơn)
   - **Câu hỏi đào sâu quá trình mày mò và lý do ưu tiên:** *"Bạn có thể miêu tả rõ cái quá trình tự mày mò đấy một cách cụ thể hơn không, hay là cho mình một ví dụ nào đó? Và tại sao bạn thường ưu tiên ChatGPT hơn là phương án khác?"*. Câu hỏi này đã khai thác chi tiết hành vi thực tế (highlight lại, note lại các thuật ngữ): slide bài giảng quá dài, khi lật ngược lại không tìm được chỗ phần cần đọc để hiểu nó, khiến người học tìm đến ChatGPT như một giải pháp cứu cánh nhanh và tiện.

2. **Chỗ nào mình cần làm tốt hơn ở lần phỏng vấn thật?**
   - **Tránh dồn nhiều câu hỏi cùng lúc (Question Stacking):** Ở lượt hỏi gần cuối, người phỏng vấn đã ghép 3 ý vào cùng một câu: *"Tức là chốt lại thì lần gần đây nhất đấy bạn có hiểu được phần đấy không hay là bạn bỏ qua luôn, và bạn cảm giác thế nào khi mà mình xem và mình không hiểu như thế?"*. Câu hỏi dồn dập khiến người trả lời bị ngợp, phải hỏi lại: *"Bạn hỏi cái gì nữa nhở?"*, buộc người phỏng vấn phải lặp lại câu hỏi về cảm xúc. Tôi cần hỏi từng câu đơn ngắn gọn và tổng quát hơn.
   - **Tránh sa đà vào câu hỏi so sánh công cụ/tính năng (Tool-centric):** Câu hỏi *"Thế thì chẳng hạn như là có Gemini này, Grok này, sao bạn lại không sử dụng, hoặc là Claude?"* Câu hỏi này không mang lại quá nhiều insight gì, nên tránh và đổi sang câu khác để khai thác thông tin.
   - **Hạn chế câu hỏi đóng mang tính xác nhận/dẫn dắt (Closed / Leading question):** Câu hỏi *"Tức là khi thấy không hiểu đoạn đó thì phản ứng đầu tiên của bạn sẽ là sử dụng ChatGPT?"* là câu hỏi đóng (Yes/No), dễ khiến user trả lời thụ động ("Ừ, hiện tại bây giờ là thế...").

3. **Sau khi luyện, nhóm đã sửa Conversation Guide ở đâu và vì sao?**
   - **Bổ sung câu hỏi probe về "bẫy tra cứu thuật ngữ" (Jargon rabbit hole) và sự ngắt quãng mạch tư duy:** Từ chia sẻ thực tế của user (*"có quá nhiều thuật ngữ không hiểu... mở nhiều tab tra cứu làm ngắt quãng dòng suy nghĩ và mất thời gian hiểu lại"*), nhóm đã bổ sung vào Guide câu probe: *"Khi công cụ giải thích bằng một thuật ngữ mới khác, bạn xử lý thế nào và việc phải tra cứu chéo nhiều tài liệu/tab ảnh hưởng ra sao đến mạch suy nghĩ của bạn?"*.
   - **Bổ sung câu hỏi về rào cản khi tìm lại kiến thức nền trong tài liệu học tập:** User chia sẻ *"slide khá là dài mà khi mình lật ngược lại mình không tìm được chỗ phần mình cần đọc để có thể hiểu được thuật ngữ đó"*. Đây là minh chứng thực tế củng cố cho giả thuyết Pain A (người học không định vị được lỗ hổng kiến thức nền). Nhóm đã bổ sung câu probe: *"Khi bạn muốn tự lật lại bài học cũ để tìm định nghĩa kiến thức nền, khó khăn lớn nhất khiến bạn không tìm thấy là gì?"*.
   - **Tách bạch hoàn toàn câu hỏi kiểm tra kết quả hiểu bài và câu hỏi bộc lộ cảm xúc:** Sửa Guide để tách thành 2 câu hỏi độc lập: (1) Đánh giá mức độ hiểu bài sau khi tự xoay xở (phần cơ bản vs phần chuyên sâu) và (2) Cảm xúc/sự ức chế khi bị ngắt quãng dòng suy nghĩ, giúp người trả lời không bị sót ý.
   - **Loại bỏ các câu hỏi khảo sát công cụ giải pháp:** Nhắc nhở người phỏng vấn bám sát nguyên tắc The Mom Test: chỉ tập trung vào hành vi quá khứ và rào cản thực tế của người học, tuyệt đối không sa vào so sánh công nghệ hay thăm dò tính năng tương lai.

## 5. AI Support Log
- **AI đã giúp gì:**
  - Hỗ trợ rà soát và tinh chỉnh ngôn từ trong câu hỏi phỏng vấn
  - Chuyển nội dung cuộc phỏng vấn thành văn bản
- **Điểm sai/hời hợt của AI & Cách tự sửa:**
  - *Điểm hạn chế của AI:* Mặc dù người dùng đã cung cấp câu hỏi phỏng vấn để AI sửa từ ngữ nhưng AI lại có xu hướng thêm câu hỏi, điều khiến câu hỏi trở nên phức tạp cho người nghe
  - *Cách tự sửa:* Chủ động phản biện và loại bỏ toàn bộ phần thừa của các câu hỏi cho phỏng vấn