# CHECKPOINT 1 — AI SUPPORT RADAR

## 1. Mục tiêu của Checkpoint 1

Mục tiêu của Checkpoint 1 là **mở lại toàn bộ logic đang bị nén trong solution directive** và chuyển solution ban đầu thành một **Problem Hypothesis đủ rõ, đủ cụ thể và có thể bị evidence làm thay đổi**.

Nhóm không xem solution được giao là đáp án đúng. Thay vào đó, nhóm đi ngược từ solution để xác định:

**Solution → Change → Actor → Situation & Job → Pain → Evidence**

Tất cả nội dung trong Checkpoint 1 đều là **hypothesis**, chưa phải fact về user.

---

# 2. Solution — Gỡ solution khỏi hình thức cụ thể

## Case đã chọn

**Case C — AI Support Radar**

## Solution directive

Sau mỗi phiên học, hệ thống phân tích các tín hiệu như:

- Di chuyển giữa slide.
- Dừng lâu hoặc xem lại.
- Highlight và ghi chú.
- Đánh dấu “Chưa hiểu”.
- Thay đổi câu trả lời.
- Nội dung trao đổi với AI Chat.

Sau đó, AI tạo một **Support Queue** cho giảng viên, gồm:

1. Những học viên có thể cần hỗ trợ.
2. Phần nội dung mà họ có thể đang gặp khó khăn.
3. Các tín hiệu dẫn đến nhận định đó.
4. Một hành động hỗ trợ được đề xuất.

Giảng viên xem lại và quyết định có liên hệ với học viên hay không.

## Capability trung tính

> **Giúp người phụ trách hỗ trợ học tập nhận biết và ưu tiên những học viên có khả năng đang gặp khó khăn, hiểu được bối cảnh của khó khăn đó và quyết định có cần can thiệp hay không.**

### Vì sao capability này là trung tính?

Capability trên không còn phụ thuộc vào:

- AI.
- Support Queue.
- Dashboard.
- Thuật toán scoring.
- Slide tracking.
- Push notification.
- Một giao diện hoặc tên feature cụ thể.

Điều này giúp nhóm không mặc định rằng AI Support Radar là cách duy nhất để giải quyết vấn đề.

---

# 3. Change — Làm lộ chuỗi thay đổi được kỳ vọng

Không nên giả định:

> AI Support Radar → Learner học tốt hơn.

Đây là một bước nhảy quá lớn giữa feature và outcome.

Chuỗi thay đổi hợp lý hơn là:

> **Solution**  
> → Instructor có thêm khả năng nhìn thấy các dấu hiệu learner có thể đang gặp khó khăn  
> → Instructor xác định nhanh hơn ai đáng được xem xét trước  
> → Instructor hiểu hơn learner có thể đang vướng ở nội dung nào  
> → Instructor quyết định có cần hỗ trợ hay không  
> → Instructor có thể hỗ trợ đúng người và đúng thời điểm hơn  
> → **Outcome: giảm số khó khăn học tập bị bỏ sót hoặc kéo dài mà không được hỗ trợ**

## Các thay đổi được kỳ vọng

### 1. Thay đổi về awareness

Instructor có khả năng nhận biết những trường hợp learner có thể đang gặp khó khăn nhưng chưa chủ động nói ra.

### 2. Thay đổi về decision

Instructor có thể ưu tiên tốt hơn câu hỏi:

> **“Tôi nên kiểm tra hoặc hỗ trợ ai trước?”**

thay vì phải rà soát mọi learner như nhau.

### 3. Thay đổi về action

Instructor có thể đưa ra hành động hỗ trợ phù hợp và kịp thời hơn đối với những trường hợp đáng quan tâm.

## Phân biệt Output và Outcome

### Output mà product có thể tạo ra

> Một tập thông tin giúp instructor nhận diện, đánh giá và ưu tiên các learner có khả năng cần hỗ trợ.

### Outcome mà product chỉ có thể ảnh hưởng

> Những khó khăn học tập quan trọng được phát hiện và xử lý sớm hơn.

### Assumption quan trọng

Nếu instructor nhận được thông tin tốt hơn nhưng **không thay đổi hành vi**, thì solution có thể tạo ra output nhưng không tạo ra outcome.

Do đó, một assumption cần kiểm chứng là:

> **Better information có dẫn đến better action hay không?**

---

# 4. Actor — Xác định các nhóm người có liên quan

| Actor | Họ đang làm gì? | Pain hoặc hậu quả có thể có | Họ hưởng lợi thế nào? |
|---|---|---|---|
| **Learner** | Học nội dung, trả lời câu hỏi, tự xử lý khi chưa hiểu | Có thể gặp khó khăn nhưng không chủ động hỏi hoặc không nhận ra mình cần hỗ trợ | Được hỗ trợ đúng lúc, giảm nguy cơ để lỗ hổng kiến thức kéo dài |
| **Instructor** | Theo dõi tiến độ và hỗ trợ nhiều learner | Khó biết ai thực sự cần chú ý và cần hỗ trợ ở nội dung nào | Giảm công sức rà soát và ưu tiên hỗ trợ tốt hơn |
| **Coach / TA** | Hỗ trợ learner theo yêu cầu hoặc theo phân công | Có thể thiếu context trước khi tiếp cận learner | Có context rõ hơn để hỗ trợ đúng vấn đề |

## Actor nhóm chọn để điều tra trước

> **Instructor / Coach chịu trách nhiệm theo dõi và hỗ trợ learner.**

## Vì sao chọn actor này trước?

Vì đây là actor:

1. Trực tiếp nhận giá trị từ capability.
2. Phải đưa ra quyết định **“có hỗ trợ hay không?”**.
3. Phải thay đổi hành vi thì outcome mới xảy ra.
4. Nếu actor này không có nhu cầu hoặc không tin tín hiệu, solution gần như mất giá trị.

Learner vẫn cần được interview vì learner là người:

- Trực tiếp trải nghiệm khó khăn học tập.
- Có thể không muốn bị can thiệp chỉ dựa trên tín hiệu hành vi.
- Có thể đã có cách tự xử lý khác.
- Có thể không xem việc instructor chủ động liên hệ là hữu ích.

Nếu vòng interview chỉ có learner, nhóm phải ghi rõ:

> **“Vòng này chỉ có learner-side evidence; instructor-side job chưa được kiểm chứng.”**

---

# 5. Situation & Job — User đang cố làm gì trong tình huống nào?

## Situation giả thuyết

Sau khi một nhóm learner vừa hoàn thành một phiên học, instructor cần quyết định:

- Có learner nào cần được theo dõi thêm không?
- Ai cần được ưu tiên?
- Họ có thể đang vướng ở đâu?
- Có cần chủ động hỗ trợ hay không?

## Cách instructor hiện tại có thể đang làm

Đây chỉ là hypothesis, chưa phải fact:

- Xem câu trả lời.
- Xem câu hỏi learner gửi.
- Xem chat.
- Nhớ lại tương tác trong buổi học.
- Chờ learner chủ động hỏi.
- Xem kết quả bài tập.
- Hỏi coach/TA.
- Ghi chú thủ công.
- Liên hệ trực tiếp với learner.

## Mô tả Situation & Job

> Khi **một phiên học vừa kết thúc**, **instructor** đang cố **xác định learner nào cần được hỗ trợ thêm và vấn đề của họ có thể nằm ở đâu**, bằng cách **tổng hợp những thông tin và tương tác mà mình hiện có về quá trình học của learner**.

## JTBD Hypothesis

> Khi **một phiên học vừa kết thúc**, tôi muốn **nhanh chóng xác định learner nào đáng được tôi chú ý và họ có thể đang vướng ở đâu**, để tôi có thể **dành thời gian hỗ trợ cho đúng người trước khi vấn đề kéo dài hoặc ảnh hưởng đến phần học tiếp theo**.

### Lưu ý

Job không phải:

> “Tôi muốn một AI Support Queue.”

Job thực sự là:

> **“Tôi muốn biết ai cần sự chú ý của mình và vì sao.”**

Job này vẫn tồn tại ngay cả khi bỏ AI và feature khỏi bối cảnh.

---

# 6. Pain — Viết các cách giải thích cạnh tranh

Nhóm không nên chỉ viết một pain hypothesis vì sẽ dễ rơi vào confirmation bias.

Cần ít nhất hai cách giải thích cạnh tranh.

## Pain Hypothesis A — Visibility / Prioritization Problem

> Khi **một phiên học kết thúc**, **instructor** gặp khó khăn trong việc **xác định learner nào cần được hỗ trợ và cần hỗ trợ về nội dung nào**, vì **các dấu hiệu về khó khăn của learner có thể nằm rải rác trong nhiều tương tác và không phải learner nào cũng chủ động thể hiện rằng mình đang gặp vấn đề**, dẫn đến **một số trường hợp có thể không được chú ý hoặc chỉ được phát hiện khi vấn đề đã kéo dài**.

### Tóm tắt

> **Instructor không có đủ visibility để biết ai đáng được chú ý trước.**

---

## Pain Hypothesis B — Capacity Problem

> Khi **một phiên học kết thúc**, **instructor** gặp khó khăn trong việc **hỗ trợ đầy đủ những learner đang gặp khó khăn**, không nhất thiết vì họ không nhận biết được learner nào cần hỗ trợ, mà vì **thời gian và khả năng hỗ trợ có hạn**, dẫn đến việc **dù đã biết learner nào có vấn đề, instructor vẫn không thể can thiệp kịp thời cho tất cả các trường hợp**.

### Tóm tắt

> **Instructor biết ai cần hỗ trợ rồi; bottleneck thực sự là capacity chứ không phải visibility.**

### Vì sao Hypothesis B quan trọng?

Nếu Hypothesis B đúng, AI Support Radar có nguy cơ trở thành:

> **Một công cụ giúp instructor nhìn thấy thêm những việc mà họ vốn đã không có đủ thời gian để xử lý.**

Trong trường hợp đó, solution ban đầu có thể không giải đúng bottleneck.

---

# 7. Giả thuyết nhóm chọn để điều tra trước

> **Chọn Pain Hypothesis A — Visibility / Prioritization Problem.**

## Lý do chọn

Solution directive hiện tại dựa gần như toàn bộ trên assumption rằng:

> Nếu instructor có thêm các tín hiệu tốt hơn về learner, họ sẽ xác định được những trường hợp cần hỗ trợ tốt hơn.

Do đó, nhóm cần kiểm chứng assumption này trước.

Nếu instructor thực tế đã biết khá rõ ai đang gặp vấn đề, thì phần lớn giá trị cốt lõi của AI Support Radar sẽ bị đặt dấu hỏi.

---

# 8. Evidence — Xác định điều cần tìm trước khi viết câu hỏi interview

Evidence cần đến từ:

- Sự kiện thực tế đã xảy ra.
- Hành vi thực tế.
- Workaround.
- Effort.
- Consequence.
- Pattern lặp lại.

Không xem các câu trả lời mang tính opinion như:

> “Tôi thấy feature này hay.”

là evidence đủ mạnh.

## Evidence Map

| Cần kiểm tra | Evidence làm nhóm tin hơn | Evidence làm nhóm nghi ngờ hoặc bác bỏ |
|---|---|---|
| **Situation có thật** | Instructor thường xuyên phải xem xét sau buổi học xem ai cần hỗ trợ | Instructor không thực hiện job này hoặc không coi đây là trách nhiệm của mình |
| **Pain có ý nghĩa** | Có trường hợp instructor nhận ra learner gặp khó khăn khá muộn | Instructor thường biết ngay ai đang gặp vấn đề |
| **Visibility là barrier** | Instructor phải xem nhiều nguồn, nhớ thủ công hoặc chờ learner tự báo | Instructor đã có một chỉ báo rõ và đủ đáng tin |
| **Workaround tồn tại** | Instructor xem bài, chat, message, hỏi TA, spreadsheet, ghi chú riêng | Instructor không cố tìm learner gặp khó khăn vì việc này không quan trọng |
| **Consequence tồn tại** | Learner bị tụt lại, lặp lỗi, bỏ bài, hỏi muộn hoặc cần remediation sau đó | Không phát hiện sớm cũng không tạo hậu quả đáng kể |
| **Pattern có lặp** | Instructor kể được nhiều trường hợp tương tự ở các buổi hoặc lớp khác nhau | Chỉ xảy ra một vài trường hợp ngoại lệ |
| **Prioritization có giá trị** | Khi lớp đông, instructor phải quyết định ai cần được chú ý trước | Instructor có đủ thời gian để xem từng learner |
| **Instructor sẽ hành động** | Khi phát hiện learner có vấn đề, instructor thường follow-up | Instructor dù biết vẫn thường không can thiệp |
| **Learner chấp nhận support** | Learner từng muốn được instructor check-in khi mắc kẹt | Learner thấy kiểu can thiệp này gây khó chịu hoặc không hữu ích |

---

# 9. Ví dụ về evidence mạnh và evidence yếu

## Evidence mạnh ủng hộ Hypothesis A

Ví dụ instructor kể:

> “Tuần trước có một bạn làm sai ba bài liên tiếp nhưng không hỏi gì. Tôi chỉ phát hiện cuối tuần khi bạn ấy nhắn lại, lúc đó mới biết bạn ấy đã không hiểu từ lesson trước.”

Evidence này mạnh vì có:

**Event → Behavior → Delay → Consequence**

---

## Evidence mạnh chống lại Hypothesis A

Ví dụ instructor kể:

> “Tôi nhìn assignment là biết ngay ai đang yếu. Vấn đề không phải phát hiện. Tôi chỉ có khoảng 30 phút mỗi ngày nên không thể hỗ trợ hết.”

Evidence này:

- Làm yếu Hypothesis A.
- Làm mạnh Hypothesis B.

---

# 10. Problem Hypothesis nhóm mang sang Chặng 2

> **Sau một phiên học có nhiều learner, instructor có thể gặp khó khăn trong việc xác định ai cần được hỗ trợ trước và họ đang vướng ở nội dung nào, vì những dấu hiệu về khó khăn của learner không phải lúc nào cũng được thể hiện trực tiếp và có thể phân tán trong nhiều tương tác học tập. Điều này có thể khiến một số khó khăn không được nhận biết hoặc được xử lý muộn hơn mức cần thiết.**

### Vì sao dùng ngôn ngữ “có thể”?

Vì đây vẫn là **Problem Hypothesis**, chưa phải kết luận.

Nhóm chưa có đủ evidence để khẳng định:

- Problem chắc chắn tồn tại.
- Problem đủ lớn.
- Problem lặp đủ thường xuyên.
- Instructor hiện không có cách giải quyết tốt.
- AI là hướng phù hợp.

---

# 11. Điều gì phải đúng để giả thuyết đứng vững?

Ít nhất các điều sau phải đúng:

## 1. Job thực sự tồn tại

Instructor thực sự có trách nhiệm hoặc nhu cầu nhận biết learner nào cần hỗ trợ sau phiên học.

## 2. Visibility hiện tại chưa đủ

Có những trường hợp instructor khó nhận ra learner đang gặp khó khăn.

## 3. Pain có consequence

Việc không phát hiện hoặc phát hiện muộn tạo ra hậu quả đáng kể.

Ví dụ:

- Learner tụt lại.
- Lặp lỗi.
- Không hiểu phần học tiếp theo.
- Hỏi quá muộn.
- Cần hỗ trợ bổ sung nhiều hơn.

## 4. Problem xảy ra đủ thường xuyên

Không phải một edge case chỉ xảy ra rất hiếm.

## 5. Better information có khả năng thay đổi action

Nếu instructor biết chính xác hơn ai cần hỗ trợ, instructor thực sự sẽ:

- Kiểm tra.
- Liên hệ.
- Ưu tiên.
- Hỗ trợ.
- Chuyển cho coach/TA.
- Điều chỉnh nội dung.

Nếu:

> **Better insight ≠ Better action**

thì solution có thể tạo output nhưng không tạo outcome.

---

# 12. Điều gì có thể khiến nhóm sửa hoặc bác bỏ giả thuyết?

Nhóm sẽ sửa hoặc bác bỏ Problem Hypothesis nếu evidence cho thấy một hoặc nhiều điều sau:

1. Instructor **đã có thể nhận biết khá chính xác** learner đang gặp khó khăn bằng công cụ hoặc quy trình hiện tại.
2. Bottleneck thực sự là **thiếu thời gian hoặc capacity hỗ trợ**, không phải thiếu visibility.
3. Learner thường xuyên chủ động báo khi gặp vấn đề, nên instructor không bị thiếu thông tin đáng kể.
4. Những hành vi như xem lại slide, dừng lâu, highlight hoặc đổi đáp án **không phản ánh đáng tin cậy** việc learner đang không hiểu.
5. False positive có thể khiến instructor mất nhiều thời gian hơn giá trị nhận được.
6. Learner không muốn instructor chủ động can thiệp dựa trên các tín hiệu hành vi.
7. Hậu quả của việc phát hiện muộn không đủ lớn.
8. Situation xảy ra quá hiếm để đáng đầu tư.
9. Instructor không có hành động khả thi ngay cả khi được cung cấp thông tin tốt hơn.

---

# 13. Solution Parking Lot

Sau khi park solution ban đầu, nhóm brainstorm nhiều hướng giải quyết.

Yêu cầu: ít nhất 5 hướng, trong đó có ít nhất 1 hướng không sử dụng AI.

| # | Hướng giải quyết có thể có | AI / Không AI |
|---|---|---|
| 1 | **Learner check-in cuối buổi:** hỏi learner “Phần nào bạn chưa tự tin?” hoặc “Bạn có cần hỗ trợ ở phần nào không?” | Không AI |
| 2 | **Dashboard tổng hợp tín hiệu học tập quan trọng** cho instructor | Không nhất thiết AI |
| 3 | **Rule-based flags:** ví dụ sai nhiều câu cùng concept, nhiều lần đổi đáp án, đánh dấu “Chưa hiểu” | Không AI |
| 4 | **AI Support Radar:** tổng hợp nhiều learning signals và đề xuất learner cần được xem xét | AI |
| 5 | **AI summary cho instructor:** tóm tắt learner, possible issue và supporting evidence | AI |
| 6 | **Learner self-reflection cuối session:** learner tự xác nhận phần mình còn chưa chắc | Không AI |
| 7 | **Scheduled support / office-hour matching:** đề xuất slot hỗ trợ phù hợp | Có thể không AI |
| 8 | **Peer-support / coach routing:** chuyển learner cần hỗ trợ tới coach, TA hoặc peer phù hợp | Có thể AI hoặc không AI |

### Nguyên tắc

AI Support Radar hiện tại chỉ là:

> **Một solution option trong nhiều solution option.**

Nhóm chưa có đủ evidence để khẳng định đây là solution tốt nhất.

---

# 14. CHECKPOINT 1 — Bản chốt

## Problem Hypothesis

> **Sau một phiên học có nhiều learner, instructor có thể gặp khó khăn trong việc xác định ai cần được hỗ trợ trước và họ đang vướng ở nội dung nào, vì những dấu hiệu về khó khăn của learner không phải lúc nào cũng được thể hiện trực tiếp và có thể phân tán trong nhiều tương tác học tập. Điều này có thể khiến một số khó khăn không được nhận biết hoặc được xử lý muộn hơn mức cần thiết.**

## Competing Hypotheses

### A — Visibility / Prioritization

> Instructor không có đủ visibility để biết learner nào cần được chú ý trước.

### B — Capacity

> Instructor đã biết learner nào cần hỗ trợ nhưng không có đủ thời gian hoặc nguồn lực để hỗ trợ.

## Hypothesis chọn để điều tra trước

> **A — Visibility / Prioritization**

## Evidence cần tìm

Nhóm cần tìm evidence về:

- Sự kiện gần đây.
- Hành vi thực tế.
- Cách instructor hiện tại nhận biết learner gặp khó khăn.
- Workaround.
- Effort.
- Consequence.
- Pattern lặp lại.
- Việc instructor có thực sự hành động khi biết learner cần hỗ trợ hay không.

## Evidence có thể bác bỏ hypothesis

> Nếu instructor đã có visibility tốt và bottleneck thực sự là capacity, hoặc nếu những khó khăn không được phát hiện sớm không tạo ra consequence đáng kể, nhóm sẽ sửa hoặc bác bỏ hypothesis.

---

# 15. Logic toàn bộ Checkpoint 1

```text
AI Support Radar
        ↓ reverse
Capability trung tính:
Giúp instructor nhận biết và ưu tiên learner có thể cần hỗ trợ
        ↓
Actor:
Instructor / Coach
        ↓
Situation:
Sau một phiên học
        ↓
Job:
Xác định ai cần được chú ý và họ có thể đang vướng ở đâu
        ↓
Pain A:
Thiếu visibility / prioritization
        ↕ competing
Pain B:
Thiếu capacity hỗ trợ
        ↓
Evidence từ hành vi và sự kiện thực tế
        ↓
Xác nhận / sửa / bác bỏ Problem Hypothesis
        ↓
Park solution ban đầu
        ↓ forward
Brainstorm nhiều Solution Options
        ↓
Chỉ lựa chọn solution sau khi problem đã được kiểm chứng
```

---

# 16. Bản trình bày ngắn 1–2 phút

> **Solution ban đầu của nhóm là AI Support Radar. Khi reverse từ solution, nhóm nhận thấy capability cốt lõi không phải là “dùng AI tạo Support Queue”, mà là giúp instructor biết learner nào đáng được chú ý và vì sao.**
>
> **Actor nhóm ưu tiên điều tra là instructor hoặc coach, trong tình huống sau một phiên học khi họ cần xác định learner nào cần hỗ trợ thêm.**
>
> Nhóm hiện có hai cách giải thích cạnh tranh.
>
> **Hypothesis A:** instructor gặp vấn đề về visibility và prioritization — họ không dễ nhận biết learner nào đang gặp khó khăn nếu learner không chủ động thể hiện.
>
> **Hypothesis B:** instructor thực ra đã biết learner nào đang gặp vấn đề, nhưng bottleneck nằm ở capacity — họ không có đủ thời gian để hỗ trợ.
>
> Nhóm chọn **Hypothesis A để kiểm chứng trước**, vì đây là assumption quan trọng nhất đứng sau AI Support Radar.
>
> Evidence nhóm cần không phải là việc user nói họ “thích feature”, mà là các sự kiện thực tế trong quá khứ: instructor từng bỏ sót learner nào, phát hiện bằng cách nào, phát hiện lúc nào, đã dùng workaround gì và việc phát hiện muộn gây hậu quả gì.
>
> Nếu evidence cho thấy instructor đã có visibility tốt và bottleneck thực sự là capacity, nhóm sẽ sửa hoặc bác bỏ hypothesis.
>
> Sau khi park solution ban đầu, nhóm giữ nhiều hướng giải quyết như learner check-in, rule-based flagging, dashboard, self-reflection và AI Support Radar. Chỉ sau khi problem được evidence xác nhận, nhóm mới tiếp tục đánh giá solution phù hợp nhất.

---

# 17. Tiêu chí tự kiểm trước khi qua Checkpoint 1

Nhóm chỉ nên coi Checkpoint 1 là hoàn thành khi có thể trả lời rõ tất cả các câu sau:

- [x] Đã gỡ solution khỏi tên feature, giao diện và công nghệ cụ thể chưa?
- [x] Đã mô tả capability trung tính chưa?
- [x] Đã chỉ ra chuỗi thay đổi từ solution đến outcome chưa?
- [x] Đã phân biệt output và outcome chưa?
- [x] Đã xác định các actor liên quan chưa?
- [x] Đã chọn actor ưu tiên để điều tra chưa?
- [x] Đã mô tả Situation & Job mà không phụ thuộc vào AI chưa?
- [x] Đã có ít nhất hai Pain Hypothesis cạnh tranh chưa?
- [x] Đã chọn một hypothesis để điều tra trước và giải thích lý do chưa?
- [x] Đã xác định evidence làm hypothesis mạnh hơn chưa?
- [x] Đã xác định evidence có thể khiến hypothesis bị sửa hoặc bác bỏ chưa?
- [x] Đã viết Problem Hypothesis đủ cụ thể nhưng chưa biến nó thành fact chưa?
- [x] Đã park solution ban đầu chưa?
- [x] Đã brainstorm ít nhất 5 solution options, trong đó có hướng không sử dụng AI chưa?

---

## Kết luận

Checkpoint 1 không nhằm chứng minh **AI Support Radar là đúng**.

Mục tiêu là:

> **Biến một solution directive thành một Problem Hypothesis có thể kiểm chứng và có thể sai.**

Tư duy cốt lõi của nhóm là:

> **Không đi tìm evidence để bảo vệ solution.  
> Đi tìm evidence đủ mạnh để problem và solution ban đầu có quyền bị thay đổi.**
