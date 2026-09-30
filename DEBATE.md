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
2. Ask Gemini for its opening argument.
3. Paste Gemini's response into the ChatGPT conversation.
4. ChatGPT responds with a direct rebuttal.
5. Paste ChatGPT's response back into Gemini.
6. Continue for the agreed number of rounds.
7. Save the final transcript under `debates/`.

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

## Conclusion
...
```

## Roles

Gemini and ChatGPT are opposing debaters. Neither side should treat the other side's claims as established facts without checking them. For factual disputes, identify the claim, evidence, uncertainty, and strongest counterargument.

The human user is the moderator and decides the topic, number of rounds, and stopping point.
