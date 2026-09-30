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

Bên gửi nên cho bên nhận biết:

- Session nào.
- Phase nào.
- Round/lượt nào.
- Context cần thiết.
- Lượt vừa rồi của đối phương.
- Bên nhận cần làm gì tiếp theo.

Không cần format kỹ thuật phức tạp. Chỉ cần thông tin đủ rõ để bên nhận tiếp tục đúng trạng thái.

Nếu không hiểu session, phase, context hoặc nhiệm vụ tiếp theo, phải hỏi người dùng thay vì tự đoán.

## Các phase

### Debate

Hai bên phản biện trực tiếp lập luận của nhau.

### Rút kết

Mỗi bên tự đánh giá lại lập luận của mình và chốt kết luận. Không mở thêm vòng phản biện.

### Decision

Dựa trên toàn bộ debate và hai phần Rút kết để xác định phương án hành động phù hợp nhất cho người dùng.

Decision phải đưa ra phương án, lý do, điều kiện, rủi ro/trade-off, bước tiếp theo và điều kiện khiến quyết định cần thay đổi.

## Vai trò của người dùng

Người dùng là moderator và người truyền lượt.

Người dùng không cần chỉnh sửa nội dung của hai bên khi truyền lượt. Nếu cần thay đổi topic, số round, context hoặc phase, người dùng sẽ quyết định và thông báo cho cả hai bên.

## Các file chính

- `DEBATE_RULES.md` — luật và protocol chi tiết.
- `DEBATE.md` — protocol tổng quát.
- `debates/INDEX.md` — danh sách các session.
- `debates/<session>/CONTEXT.md` — context chính thức của từng session.
- `debates/<session>/TRANSCRIPT.md` — transcript của từng session.
