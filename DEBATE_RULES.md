# Gemini ↔ ChatGPT Debate Rules

## 1. Mục đích

Repository này là nơi lưu trữ các phiên tranh luận giữa Gemini và ChatGPT.

Gemini và ChatGPT tranh luận trực tiếp về một chủ đề do người dùng đưa ra.
Người dùng đóng vai trò trung gian truyền lượt giữa hai AI.

GitHub chỉ dùng để lưu luật và transcript. Không yêu cầu Gemini có quyền ghi vào repository.

## 2. Vai trò

### Gemini
- Đại diện cho phía Gemini.
- Đưa ra lập luận, phản biện và bảo vệ quan điểm của mình.
- Khi nhận được câu trả lời của ChatGPT, phải phản hồi trực tiếp vào các điểm chính.
- Không được coi việc người dùng truyền nội dung qua lại là một phần của lập luận.

### ChatGPT
- Đại diện cho phía ChatGPT.
- Khi người dùng gửi nội dung được đánh dấu là lượt của Gemini, phải tiếp tục tranh luận từ đúng trạng thái hiện tại.
- Phải phản biện trực tiếp các lập luận của Gemini.
- Không được giả vờ rằng mình có thể giao tiếp trực tiếp với Gemini.
- Đồng thời giữ transcript của phiên tranh luận trong cuộc trò chuyện.

### Người dùng
- Chuyển câu trả lời của Gemini sang ChatGPT.
- Chuyển câu trả lời của ChatGPT sang Gemini.
- Không được tự ý thay đổi nội dung của hai bên khi truyền lượt.

## 3. Luật tranh luận

1. Hai bên phải tranh luận về cùng một chủ đề.
2. Mỗi lượt phải phản hồi vào lập luận của lượt trước, không chỉ lặp lại quan điểm ban đầu.
3. Ưu tiên lập luận có căn cứ và khả năng kiểm chứng.
4. Không được bịa nguồn, dữ kiện, trích dẫn hoặc trải nghiệm.
5. Khi phát hiện lập luận của chính mình sai, phải thừa nhận và điều chỉnh.
6. Phân biệt rõ:
   - dữ kiện
   - suy luận
   - giả định
   - ý kiến
7. Không công kích người dùng hoặc bên tranh luận thay vì phản biện lập luận.
8. Nếu chủ đề cần thông tin hiện tại, bên tranh luận phải kiểm chứng thông tin trước khi khẳng định.
9. Không cố thắng bằng cách kéo dài câu trả lời hoặc né câu hỏi.
10. Mỗi bên phải tập trung vào điểm mạnh nhất của lập luận đối phương.

## 4. Cấu trúc phiên

Một phiên gồm ba giai đoạn:

### Giai đoạn A — Debate Rounds

Mỗi hiệp gồm hai lượt:

- Gemini — Hiệp N
- ChatGPT — Hiệp N

Mặc định bắt đầu với ChatGPT.

Tiếp tục cho đến số hiệp đã định hoặc khi người dùng kết thúc phần tranh luận.

### Giai đoạn B — Final Synthesis / Rút kết

Sau khi kết thúc các Debate Rounds, hai bên thực hiện một lượt rút kết độc lập.

Mỗi bên phải nêu:

1. Những luận điểm của phía mình vẫn đứng vững.
2. Những luận điểm của phía mình đã bị bác bỏ hoặc phải điều chỉnh.
3. Những luận điểm của đối phương mà mình thừa nhận có giá trị.
4. Những vấn đề vẫn chưa được giải quyết.
5. Kết luận cuối cùng của phía mình dựa trên toàn bộ debate.

Giai đoạn Rút kết không phải là một vòng phản biện mới. Hai bên không tiếp tục tranh luận trực tiếp với nhau trong giai đoạn này.

### Giai đoạn C — Decision / Quyết định cuối

Sau khi cả hai bên hoàn thành Rút kết, chuyển từ phân tích sang ra quyết định.

Hai bên phải dùng toàn bộ kết quả của debate và phần Rút kết để xác định phương án hành động phù hợp nhất với mục tiêu và điều kiện đã đặt ra.

Giai đoạn này phải tạo ra một output quyết định duy nhất, gồm:

1. Phương án được đề xuất.
2. Lý do chọn phương án đó.
3. Điều kiện và giả định khiến phương án đó phù hợp.
4. Rủi ro và trade-off chính.
5. Bước hành động tiếp theo.
6. Điều kiện hoặc dữ kiện nào có thể khiến phải đổi phương án.

Nếu dữ liệu chưa đủ để chọn một phương án, phải nói rõ chưa thể quyết định và xác định chính xác dữ kiện cần có trước khi quyết định.

Không bắt buộc tuyên bố bên thắng. Mục tiêu của Giai đoạn C là xác định người dùng nên làm gì dựa trên toàn bộ debate, không phải xác định AI nào thắng.

Sau khi Decision hoàn tất, phiên được chuyển sang COMPLETED.

## 5. Format truyền lượt

Người dùng có thể gửi:

[GEMINI — HIỆP N]

<nội dung Gemini>

ChatGPT phải hiểu đây là lượt chính thức của Gemini và tiếp tục ngay từ đó.

Khi cần chuyển sang Gemini, ChatGPT xuất ra phần trả lời của mình với nhãn:

[CHATGPT — HIỆP N]

<nội dung ChatGPT>

Trong giai đoạn Rút kết, sử dụng:

[GEMINI — RÚT KẾT]

<nội dung Gemini>

và:

[CHATGPT — RÚT KẾT]

<nội dung ChatGPT>

Trong giai đoạn Decision, sử dụng:

[FINAL DECISION]

<nội dung quyết định cuối>

## 5.5. Communication / Handoff

ChatGPT và Gemini giao tiếp thông qua người dùng. Mỗi khi chuyển lượt, bên gửi phải cung cấp đủ thông tin để bên nhận hiểu phiên đang ở đâu và cần làm gì tiếp theo.

Khi chuyển một lượt, ưu tiên cung cấp:

- Session hiện tại.
- Phase hiện tại: Debate, Rút kết hoặc Decision.
- Số hiệp/lượt hiện tại nếu có.
- Debate Context hiện tại hoặc phần context cần thiết.
- Nội dung lượt vừa rồi của bên gửi.
- Yêu cầu rõ ràng đối với bên nhận.

Bên nhận phải tiếp tục từ đúng trạng thái được cung cấp, không tự tạo một session mới hoặc tự chuyển phase nếu chưa có căn cứ.

Nếu thiếu thông tin quan trọng hoặc không xác định được trạng thái của phiên, bên nhận phải hỏi người dùng để làm rõ thay vì tự đoán.

Không yêu cầu một format kỹ thuật cố định như JSON. Mục tiêu của handoff là để cả hai bên hiểu chính xác context, trạng thái và nhiệm vụ tiếp theo.

Khi chuyển sang Rút kết hoặc Decision, phải ghi rõ phase mới để bên nhận không tiếp tục một Debate Round thông thường.

## 6. Ghi chép transcript

Mỗi phiên tranh luận là một phiên độc lập.

Không gộp nhiều chủ đề hoặc nhiều phiên tranh luận khác nhau vào cùng một transcript.

Mỗi phiên phải có khu vực lưu trữ riêng, ví dụ:

debates/<ten-phien>/
- CONTEXT.md
- TRANSCRIPT.md

Tên phiên phải mô tả được chủ đề hoặc mục đang tranh luận.

Mỗi phiên có Debate Context riêng và transcript riêng. Khi bắt đầu một phiên mới, không được mặc định mang Debate Context hoặc transcript của phiên cũ sang, trừ khi người dùng yêu cầu.

ChatGPT chịu trách nhiệm duy trì transcript của phiên hiện tại trong cuộc trò chuyện và khi người dùng yêu cầu ghi vào repository, lưu transcript vào thư mục riêng của phiên đó.

Transcript có cấu trúc:

# Debate: <chủ đề>

## Gemini — Hiệp 1
...

## ChatGPT — Hiệp 1
...

## Gemini — Hiệp 2
...

## ChatGPT — Hiệp 2
...

# Final Synthesis / Rút kết

## Gemini — Rút kết
...

## ChatGPT — Rút kết
...

# Final Decision / Quyết định cuối

## Phương án được đề xuất
...

## Lý do
...

## Điều kiện / giả định
...

## Rủi ro / trade-off
...

## Bước tiếp theo
...

## Điều kiện thay đổi quyết định
...

Không tự ý sửa nội dung đã được ghi nhận của một bên.

## 7. Kết thúc phiên

Khi người dùng nói kết thúc phần tranh luận, ChatGPT phải:

1. Dừng việc tạo Debate Round mới.
2. Chuyển sang Final Synthesis / Rút kết.
3. Hoàn thiện phần Rút kết của hai bên.
4. Chuyển sang Decision / Quyết định cuối.
5. Tạo một output quyết định duy nhất dựa trên toàn bộ debate và hai phần Rút kết.
6. Giữ nguyên nội dung các lượt đã diễn ra.
7. Chuyển phiên sang COMPLETED sau khi Decision hoàn tất.

Mặc định không tuyên bố bên nào thắng.

## 8. Nguyên tắc của người trung gian

ChatGPT không được lợi dụng vai trò ghi chép để thay đổi luật tranh luận hoặc chỉnh sửa lập luận của Gemini.

Nếu người dùng gửi nội dung không rõ là lượt của Gemini hay yêu cầu khác, ChatGPT phải xử lý theo ngữ cảnh hiện tại thay vì tự tạo một lượt tranh luận mới.

## 9. Debate Context

Mỗi phiên tranh luận có một "Debate Context" chính thức.

Debate Context là nguồn sự thật chung của cả Gemini và ChatGPT, dùng để tránh việc hai bên có context khác nhau.

### 9.1. Context gồm

- Chủ đề tranh luận.
- Câu hỏi/đề bài gốc.
- Các định nghĩa đã thống nhất.
- Các điều kiện và giả định của cuộc tranh luận.
- Các dữ kiện do người dùng cung cấp.
- Các dữ kiện quan trọng đã được hai bên xác nhận.
- Các điểm đã được thừa nhận.
- Các điểm đang bị tranh chấp.
- Tóm tắt các lập luận quan trọng của từng bên.

### 9.2. Context của cuộc trò chuyện

ChatGPT có thể sử dụng context của cuộc trò chuyện hiện tại để hiểu ý định, lịch sử trao đổi và các thông tin liên quan.

Tuy nhiên, thông tin chỉ tồn tại trong context riêng của ChatGPT không mặc nhiên được xem là thông tin mà Gemini biết.

Nếu một thông tin từ context của ChatGPT có ảnh hưởng trực tiếp đến tranh luận, ChatGPT phải đưa thông tin đó vào Debate Context hoặc yêu cầu người dùng xác nhận trước khi sử dụng như một tiền đề chung.

### 9.3. Context truyền sang Gemini

Khi người dùng chuyển lượt ChatGPT sang Gemini, người dùng nên truyền:

1. Debate Context hiện tại.
2. Lượt ChatGPT vừa rồi.
3. Nếu cần, các lượt trước đó có liên quan.

Không cần truyền toàn bộ lịch sử cuộc trò chuyện nếu Debate Context đã chứa đủ thông tin cần thiết.

### 9.4. Context không được dùng để tạo lợi thế

Không bên nào được sử dụng thông tin mà đối phương không có để tạo ra một phản biện giả định đối phương đã biết thông tin đó.

Nếu thông tin mới xuất hiện, thông tin đó trở thành một phần của Debate Context sau khi được xác định là có liên quan.

### 9.5. Context Snapshot

Sau mỗi 2 hiệp, ChatGPT có thể tạo một Context Snapshot ngắn:

## Debate Context
- Chủ đề:
- Mục tiêu câu hỏi:
- Giả định:
- Dữ kiện đã xác nhận:
- Gemini đã lập luận:
- ChatGPT đã lập luận:
- Điểm Gemini đang phản bác:
- Điểm ChatGPT đang phản bác:
- Điểm đã thống nhất:
- Điểm chưa giải quyết:

Context Snapshot được dùng làm context gọn để tiếp tục phiên tranh luận.

## 10. Trạng thái phiên debate

Mỗi phiên debate phải có trạng thái rõ ràng để Gemini và ChatGPT biết phiên nào đang diễn ra.

Các trạng thái hợp lệ:

- **SCHEDULED** — phiên đã được tạo nhưng chưa bắt đầu.
- **ACTIVE** — phiên đang diễn ra.
- **COMPLETED** — phiên đã kết thúc.
- **CANCELLED** — phiên đã bị hủy.

Mỗi phiên phải ghi rõ:

- Status
- Scheduled start (nếu có)
- Actual start
- Actual end (nếu đã kết thúc)
- Chủ đề
- Số hiệp đã hoàn thành

Ví dụ:

## Debate Status

- Status: ACTIVE
- Scheduled start: 2026-09-30 11:30 +07:00
- Actual start: 2026-09-30 11:34 +07:00
- Actual end: —
- Rounds completed: 1

### Quy tắc trạng thái

1. Khi phiên bắt đầu, chuyển từ SCHEDULED sang ACTIVE và ghi Actual start.
2. Khi người dùng tuyên bố kết thúc hoặc phiên được kết thúc theo luật, chuyển sang COMPLETED và ghi Actual end.
3. Phiên COMPLETED không được tiếp tục nhận lượt mới.
4. Phiên SCHEDULED không được coi là đang tranh luận.
5. Chỉ một phiên được đánh dấu ACTIVE tại một thời điểm, trừ khi người dùng chủ động yêu cầu chạy nhiều phiên song song.
6. Gemini và ChatGPT phải kiểm tra trạng thái của phiên trước khi tiếp tục một lượt.
7. Nếu người dùng bắt đầu một chủ đề mới, tạo một phiên mới thay vì ghi tiếp vào phiên cũ.

## 11. Danh mục phiên debate

Repository nên có một file index ở:

debates/INDEX.md

File này theo dõi toàn bộ phiên:

| Session | Topic | Status | Start | End |
|---|---|---|---|---|
| <session> | <topic> | SCHEDULED / ACTIVE / COMPLETED / CANCELLED | <time> | <time> |

Gemini có thể dùng INDEX.md để xác định:
- phiên nào đã hoàn thành;
- phiên nào đang hoạt động;
- phiên nào sắp diễn ra;
- phiên nào không còn hiệu lực.

INDEX.md không thay thế CONTEXT.md hoặc TRANSCRIPT.md của từng phiên.