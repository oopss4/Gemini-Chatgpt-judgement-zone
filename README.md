# Gemini ↔ ChatGPT Debate Arena

## Repo này dùng để làm gì?

Đây là nơi lưu luật, context và transcript cho các phiên tranh luận giữa Gemini và ChatGPT.

Hai AI không giao tiếp trực tiếp qua API. Người dùng là trung gian, nhận câu trả lời từ bên này rồi chuyển sang bên kia.

## Cách vận hành

1. Tạo hoặc chọn một debate session.
2. Đọc Debate Context và rules của session.
3. ChatGPT và Gemini lần lượt tranh luận.
4. Sau mỗi lượt, người dùng chuyển nguyên nội dung của bên này sang bên kia.
5. Khi kết thúc Debate Rounds, chuyển sang Rút kết.
6. Sau Rút kết, chuyển sang Decision để xác định phương án người dùng nên thực hiện.
7. Lưu transcript và đánh dấu session COMPLETED.

## Khi chuyển lượt

Dùng mẫu handoff chuẩn sau khi truyền lượt giữa Gemini và ChatGPT:

[DEBATE HANDOFF]
[SESSION]: <session_id>
[PHASE]: <Debate Rounds | Final Synthesis | Decision>
[ROUND]: <Round_N hoặc —>
[DEBATE CONTEXT]: <context hiện tại hoặc tóm tắt cần thiết>
[LAST TURN]: <nội dung lượt vừa rồi>
[NEXT ACTION]: <nhiệm vụ cụ thể cho bên nhận>

Sáu trường trên là bắt buộc. Không cần JSON hoặc format kỹ thuật khác.

Nếu không hiểu session, phase, context hoặc nhiệm vụ tiếp theo, phải hỏi người dùng thay vì tự đoán.

### Quyền chuyển Phase

Người dùng là người duy nhất quyết định chuyển Phase.

Gemini hoặc ChatGPT có thể đề xuất kết thúc một phase, nhưng không được tự chuyển. Khi người dùng truyền handoff với phase mới, bên nhận tiếp tục theo phase đó.

## Các phase

### Debate

Hai bên phản biện trực tiếp lập luận của nhau.

### Rút kết

Mỗi bên tự đánh giá lại lập luận của mình và chốt kết luận. Không mở thêm vòng phản biện.

Mỗi bên nên cô đọng:
- điểm đồng thuận;
- điểm bất đồng;
- kết luận riêng;
- trade-off chính.

Không bắt buộc trình bày bằng một ma trận cố định.

### Decision

Gemini và ChatGPT mỗi bên đưa ra một đề xuất chiến lược riêng dựa trên toàn bộ debate và phần Rút kết. Đề xuất của từng bên chưa phải quyết định cuối.

Mỗi đề xuất nên có:
- phương án;
- lý do;
- điều kiện / giả định;
- rủi ro / trade-off;
- bước tiếp theo;
- điều kiện thay đổi quyết định.

Sau đó tạo một [FINAL DECISION] duy nhất cho toàn bộ session. Nếu dữ liệu chưa đủ, phải nêu rõ dữ kiện cần xác minh thay vì tự đoán.

## Vai trò của người dùng

Người dùng là moderator và người truyền lượt.

Người dùng không cần chỉnh sửa nội dung của hai bên khi truyền lượt. Nếu cần thay đổi topic, số round, context hoặc phase, người dùng sẽ quyết định và thông báo cho cả hai bên.

## Các file chính

- `DEBATE_RULES.md` — luật và protocol chi tiết.
- `DEBATE.md` — protocol tổng quát.
- `debates/INDEX.md` — danh sách các session.
- `debates/<session>/CONTEXT.md` — context chính thức của từng session.
- `debates/<session>/TRANSCRIPT.md` — transcript của từng session.
