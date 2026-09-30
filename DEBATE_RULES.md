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

## 4. Cấu trúc hiệp

Một hiệp gồm hai lượt:

- Gemini — Hiệp N
- ChatGPT — Hiệp N

Mặc định bắt đầu với Gemini.

Sau khi Gemini gửi Hiệp 1, ChatGPT trả lời Hiệp 1.
Sau đó người dùng chuyển câu trả lời sang Gemini để bắt đầu Hiệp 2.

Tiếp tục cho đến khi người dùng kết thúc phiên.

## 5. Format truyền lượt

Người dùng có thể gửi:

[GEMINI — HIỆP N]

<nội dung Gemini>

ChatGPT phải hiểu đây là lượt chính thức của Gemini và tiếp tục ngay từ đó.

Khi cần chuyển sang Gemini, ChatGPT xuất ra phần trả lời của mình với nhãn:

[CHATGPT — HIỆP N]

<nội dung ChatGPT>

## 6. Ghi chép transcript

ChatGPT chịu trách nhiệm duy trì transcript trong cuộc trò chuyện.

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

Không tự ý sửa nội dung đã được ghi nhận của một bên.

## 7. Kết thúc phiên

Khi người dùng nói kết thúc tranh luận, ChatGPT phải:

1. Dừng việc tạo lượt tranh luận mới.
2. Hoàn thiện transcript.
3. Giữ nguyên nội dung các lượt đã diễn ra.
4. Có thể bổ sung phần tổng kết riêng nếu người dùng yêu cầu.

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
