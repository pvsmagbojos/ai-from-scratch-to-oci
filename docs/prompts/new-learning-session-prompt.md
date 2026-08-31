# New Learning Session Prompt

Paste this at the start of a new conversation after attaching the relevant repository files.

```text
We are continuing my AI Learning Roadmap on my `progress/<learner>` branch. Do not place personal learning artifacts on `main`.

Use `docs/prompts/ai-tutor-master-prompt.md` and the repository standards as the rules for this session.

Current roadmap item:
[PASTE THE EXACT PHASE / SECTION / CHECKLIST ITEM]

I have attached or provided the current master roadmap, current learning status, relevant issue/resolution history, and any existing files for this topic.

Teach only the current item and any prerequisite gap that is actually required to understand it. Follow the standard lesson sequence: teach -> worked example when useful -> exercise/knowledge check -> review -> documentation/progress update.

Do not mark the item complete until I provide the required evidence of understanding. Do not silently advance to the next item.

Document every material step in the learning process, including commands, file/configuration changes, exercises, decisions, important outputs, and verification. If an error or issue occurs, document the symptom/error, context, meaningful failed attempts, root cause when known, resolution/workaround, verification, and learning takeaway in the canonical issues-and-resolutions log. Do not erase troubleshooting history after a fix.

For code, always use exact repository paths and do not invent missing project structure. If required code context is missing, ask for all missing information at once.

At the end, update the canonical roadmap/progress/topic documentation, learning log, and issues-and-resolutions log affected by this session. Provide complete files as attachments when they exceed 20 lines.
```
