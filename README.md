# 1 Thông tin thành viên nhóm

| STT | Họ và tên        | Mã học viên |
| --: | ---------------- | ----------- |
|   1 | Trần Hoàng Quân  | 2A202601805 |
|   2 | Trần Thị Hoa Mai | 2A202601317 |
|   3 | Nguyễn Minh Đức  | 2A202601946 |

**Case C — AI Support Radar**
Sau mỗi phiên học, hệ thống phân tích các tín hiệu như di chuyển giữa slide, dừng lâu hoặc xem lại, highlight và ghi chú, đánh dấu “Chưa hiểu”, thay đổi câu trả lời, và nội dung trao đổi với AI Chat.

AI tạo một _Support Queue_ cho giảng viên, gồm:

- Những học viên có thể cần hỗ trợ.
- Phần nội dung mà họ có thể đang gặp khó khăn.
- Các tín hiệu dẫn đến nhận định đó.
- Một hành động hỗ trợ được đề xuất.

Giảng viên xem lại và quyết định có liên hệ với học viên hay không.

# 2. Problem Hypothesis Brief

## 1. Solution - Gỡ solution khỏi hình thức cụ thể

### **Solution directive**

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

### **Capability trung tính**

Giúp giảng viên nhận biết những học viên có khả năng cần hỗ trợ, hiểu họ có thể đang gặp khó khăn ở nội dung nào và dựa trên những dấu hiệu nào, để giảng viên quyết định cách hỗ trợ phù hợp.

## 2. Change - Làm lộ chuỗi thay đổi được kỳ vọng

Các thay đổi được kỳ vọng:

- Giảng viên có thêm thông tin để nhận biết sớm những học viên có khả năng cần hỗ trợ, thay vì chỉ dựa vào việc học viên chủ động hỏi.
- Giảng viên thay đổi hành vi: chủ động kiểm tra các trường hợp được gợi ý và quyết định có liên hệ/hỗ trợ hay không thay vì chỉ bị động chờ được học viên hỏi.
- Học viên có khả năng nhận được hỗ trợ sớm và đúng vào phần đang gặp khó khăn hơn.
- Kết quả kỳ vọng: giảm số trường hợp học viên gặp khó khăn nhưng không được phát hiện hoặc hỗ trợ kịp thời.

## 3. Actor - Xác định các nhóm người có liên quan

| Actor          | Họ đang làm gì?                                       | Pain hoặc hậu quả có thể có                                                     | Họ hưởng lợi thế nào?                                           |
| -------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| **Learner**    | Học nội dung, trả lời câu hỏi, tự xử lý khi chưa hiểu | Có thể gặp khó khăn nhưng không chủ động hỏi hoặc không nhận ra mình cần hỗ trợ | Được hỗ trợ đúng lúc, giảm nguy cơ để lỗ hổng kiến thức kéo dài |
| **Instructor** | Theo dõi tiến độ và hỗ trợ nhiều learner              | Khó biết ai thực sự cần chú ý và cần hỗ trợ ở nội dung nào                      | Giảm công sức rà soát và ưu tiên hỗ trợ tốt hơn                 |
| **Coach / TA** | Hỗ trợ learner theo yêu cầu hoặc theo phân công       | Có thể thiếu context trước khi tiếp cận learner                                 | Có context rõ hơn để hỗ trợ đúng vấn đề                         |

### **Actor nhóm chọn để điều tra trước**

Instructor / Coach chịu trách nhiệm theo dõi và hỗ trợ learner.

### **Vì sao chọn nhánh này thay vì actor khác?**

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

## 4. Situation & Job — User đang cố làm gì trong tình huống nào?

Tình huống bắt đầu
→ Sau một phiên học hoặc khi cần rà soát tình hình học tập của lớp.

User muốn hoàn thành việc gì
→ Xác định học viên nào đang gặp khó khăn và cần được hỗ trợ trước.

Hiện tại họ làm như thế nào
→ Dựa vào quan sát trên lớp, câu hỏi học viên chủ động đặt ra, kết quả bài tập/quiz, trao đổi trực tiếp hoặc tự kiểm tra tiến độ từng học viên.

Điểm bắt đầu gặp vướng mắc
→ Khi số lượng học viên lớn hoặc học viên không chủ động thể hiện rằng mình đang gặp khó khăn, khiến giảng viên khó biết ai thực sự cần hỗ trợ và đang vướng ở phần nào.

### **Mô tả Situation & Job**

Khi kết thúc một phiên học và cần kiểm tra tình trạng của lớp, giảng viên đang cố xác định những học viên có thể đang gặp khó khăn để ưu tiên hỗ trợ bằng cách quan sát hành vi học tập, xem kết quả bài tập và dựa vào những trao đổi hoặc câu hỏi mà học viên chủ động đưa ra.

### **JTBD Hypothesis**

Khi tôi cần rà soát tình trạng học tập của lớp sau một phiên học, tôi muốn nhanh chóng nhận biết học viên nào có khả năng đang gặp khó khăn và khó khăn ở đâu, để có thể ưu tiên sự chú ý và hỗ trợ đúng người, đúng vấn đề, đúng thời điểm.

## 5. Pain - Viết các cách giải thích cạnh tranh

### Pain Hypothesis A — Thiếu khả năng quan sát

Khi cần rà soát tình hình học tập của lớp sau một phiên học, giảng viên gặp khó khăn trong việc xác định học viên nào đang gặp khó khăn và cần được ưu tiên hỗ trợ vì nhiều dấu hiệu khó khăn không được học viên chủ động thể hiện và giảng viên không thể quan sát đầy đủ từng người, dẫn đến một số học viên cần hỗ trợ có thể bị phát hiện muộn hoặc bị bỏ sót.

**Ý của A là**

Barrier: thiếu thông tin / thiếu visibility
→ Giảng viên muốn hỗ trợ nhưng không biết ai cần hỗ trợ.

### Pain Hypothesis B — Biết nhưng không đủ khả năng xử lý

Khi cần rà soát tình hình học tập của lớp sau một phiên học, giảng viên gặp khó khăn trong việc hỗ trợ kịp thời những học viên đang gặp khó khăn vì thời gian và nguồn lực hỗ trợ có hạn, trong khi có nhiều học viên và nhiều vấn đề cần xử lý, dẫn đến giảng viên phải trì hoãn hoặc bỏ qua một số trường hợp dù đã nhận biết được học viên đang cần hỗ trợ.

Ý của B là:

Barrier: thiếu thời gian / capacity
→ Giảng viên đã biết ai cần hỗ trợ nhưng không đủ khả năng hỗ trợ hết.

### Giả thuyết nhóm chọn để điều tra trước: A

Lý do:

A nên được kiểm chứng trước vì AI Support Radar đang ngầm giả định rằng vấn đề chính là giảng viên thiếu khả năng nhận biết học viên cần hỗ trợ. Nếu thực tế giảng viên đã nhận biết khá tốt nhưng vấn đề nằm ở thiếu thời gian hoặc nguồn lực để can thiệp, việc cung cấp thêm một Support Queue có thể không giải quyết pain, thậm chí còn tạo thêm workload.

Đây cũng chính là giá trị của yêu cầu “cách giải thích cạnh tranh”: không cố chứng minh solution đúng, mà tìm xem nguyên nhân thật sự của hành vi/problem là gì.

## 6. Evidence - Xác định điều cần tìm trước khi viết câu hỏi

| Cần kiểm tra            | Evidence làm nhóm tin hơn                                                                                                           | Evidence làm nhóm nghi ngờ hoặc bác bỏ                                                                                 |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **Situation có thật**   | Giảng viên kể được một tình huống gần đây sau buổi học mà họ phải rà soát xem học viên nào đang gặp khó khăn                        | Giảng viên hiếm khi hoặc không có nhu cầu rà soát tình trạng từng học viên sau buổi học                                |
| **Pain có ý nghĩa**     | Giảng viên nói họ thường không chắc ai thực sự cần hỗ trợ, phải mất nhiều thời gian kiểm tra hoặc từng bỏ sót học viên              | Giảng viên cho rằng hiện tại họ đã dễ dàng biết ai cần hỗ trợ và việc này không gây nhiều khó khăn                     |
| **Workaround tồn tại**  | Giảng viên đang tự xem quiz, hỏi từng học viên, xem trao đổi, ghi chú riêng hoặc nhờ coach theo dõi để phát hiện người gặp khó khăn | Giảng viên không làm gì thêm vì họ không thấy việc phát hiện học viên gặp khó khăn đủ quan trọng                       |
| **Consequence tồn tại** | Có trường hợp học viên chỉ được phát hiện khi đã tụt tiến độ, làm sai nhiều lần, chủ động cầu cứu hoặc đến kỳ đánh giá              | Không có hậu quả đáng kể khi giảng viên không phát hiện sớm; học viên vẫn tự giải quyết hoặc được hỗ trợ qua kênh khác |
| **Pattern có lặp**      | Giảng viên kể được nhiều trường hợp tương tự ở nhiều buổi học hoặc với nhiều học viên khác nhau                                     | Đây chỉ là sự cố hiếm gặp, xảy ra với một vài trường hợp đặc biệt và không tạo thành pattern                           |

### Problem Hypothesis nhóm mang sang Chặng 2:

Khi cần rà soát tình hình học tập của lớp sau một phiên học, giảng viên gặp khó khăn trong việc xác định học viên nào đang gặp khó khăn và cần được ưu tiên hỗ trợ vì không thể quan sát đầy đủ các dấu hiệu của từng học viên, đặc biệt khi học viên không chủ động thể hiện rằng mình đang gặp vấn đề, dẫn đến một số học viên có thể được phát hiện muộn hoặc bị bỏ sót.

### Điều gì phải đúng để giả thuyết đứng vững

Tình huống này phải thực sự xảy ra và lặp lại; giảng viên phải có nhu cầu nhận biết học viên cần hỗ trợ nhưng hiện tại thiếu đủ tín hiệu hoặc mất đáng kể công sức để làm việc đó; đồng thời việc phát hiện muộn hoặc bỏ sót phải tạo ra hậu quả có ý nghĩa cho giảng viên hoặc học viên.

### Điều gì có thể khiến nhóm sửa hoặc bác bỏ giả thuyết

Nhóm nên sửa hoặc bác bỏ giả thuyết nếu phát hiện rằng giảng viên hiện đã nhận biết khá chính xác học viên nào cần hỗ trợ, hoặc việc bỏ sót hiếm và không tạo hậu quả đáng kể; đặc biệt, nếu barrier thực tế không phải thiếu thông tin mà là thiếu thời gian hoặc nguồn lực để hỗ trợ những học viên mà giảng viên đã biết, thì problem hypothesis cần chuyển sang hướng khác.

# 3. Conversation Guide phiên bản cuối
