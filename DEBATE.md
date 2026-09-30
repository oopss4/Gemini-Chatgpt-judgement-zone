# Gemini ↔ ChatGPT Debate Arena

This repository is the shared arena and transcript archive for debates between Gemini and ChatGPT.

## Current mode

No API automation.

- ChatGPT participates directly through the ChatGPT conversation.
- Gemini participates through Gemini web/app.
- GitHub is used to store topics, rules, and completed transcripts.
- The user manually passes each side's response to the other side.

## Debate protocol

1. Create or choose a debate topic.
2. Define the Debate Context and agreed number of rounds.
3. Run the Debate Rounds.
4. Ask Gemini and ChatGPT to respond directly to each other's arguments.
5. After the final Debate Round, stop direct rebuttal.
6. Run Final Synthesis / Rút kết:
   - Gemini gives its independent final synthesis.
   - ChatGPT gives its independent final synthesis.
7. Run Decision / Quyết định cuối:
   - Use the entire debate and both final syntheses.
   - Produce one recommended course of action.
   - State the rationale, conditions, risks/trade-offs, next action, and what would change the decision.
   - If the evidence is insufficient, state what must be verified before deciding.
8. Save the final transcript under `debates/`.
9. Mark the session COMPLETED after the final decision is recorded.

## Transcript format

```markdown
# AI Debate

## Topic
...

## Rules
...

## Gemini — Round 1
...

## ChatGPT — Round 1
...

## Gemini — Round 2
...

## ChatGPT — Round 2
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
```

## Roles

Gemini and ChatGPT are opposing debaters. Neither side should treat the other side's claims as established facts without checking them. For factual disputes, identify the claim, evidence, uncertainty, and strongest counterargument.

The human user is the moderator and decides the topic, number of rounds, and stopping point.