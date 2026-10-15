---
name: whiteboard
description: After finishing a task, interview the user about the code and logic to check they understand it and could explain it. Use when the user says "whiteboard", "whiteboard me", "quiz me on this" or "do I understand this?".
---

# Whiteboard

Your goal is to check that the user has cognitive ownership of the code that was
just written: that they could explain how it works and defend the decisions behind
it, without needing line-level detail.

## How to do it

- Look at the changes (diff, touched files) and understand what was done and why.
- Run it like a whiteboard interview: ask one question at a time, grounded in the
  actual code, and let the user answer in free-form prose. Ask about the decisions
  in the diff, not about function names or implementation details.
- Cover what matters in this case: why X instead of Y, what data structures it
  relies on and why, how it flows, where it fails, and what happens if an actor
  behaves maliciously. You don't need to cover everything; focus where
  misunderstanding is most likely.
- When it helps, draw a diagram of the flow the user described (not of what is
  correct) and ask whether that's what they meant. Use ASCII by default, or Mermaid
  if your environment says it renders it.
- If an answer has gaps, follow up or give a hint before explaining. If they're
  still stuck, explain it with file and line references.
- Don't give answers away and don't accept vague explanations.
- Respond in the user's language.
- Finish when it's clear they own it, or with a short summary of what's solid and
  what they should review.
