# New Learning Session Prompt

Use this at the start of a new AI-learning conversation. Prefer direct reading of the learner's live repository branch over repeatedly attaching course documentation.

Replace the placeholders before sending:

```text
Continue my AI Learning Roadmap using the live repository state below.

Repository: <repository-url>
Learning branch: <learning-branch>
Upstream repository: <upstream-url-or-none>

Read `README.md` from the specified learning branch first. Then read the master tutor prompt, roadmap, current learning status, standards, relevant learner issue history, and active topic/project files from that same branch before teaching.

Treat the specified repository + learning branch as the source of truth for my personal progress. If this is a fork, do not substitute the upstream `main` branch for my learning branch. Use the upstream repository only for shared course comparisons or updates.

If the repository/branch is publicly readable, do not ask me to re-upload files that you can read directly. If it is private or inaccessible, tell me what access is missing and use the smallest fallback available, such as a connected GitHub integration or the specific files that must be uploaded.

Follow `docs/prompts/ai-tutor-master-prompt.md` and the repository standards as the rules for this session.

Determine the current roadmap item from `docs/progress/current-learning-status.md`. Teach only that item and any prerequisite gap that is actually required to understand it. Follow the standard lesson sequence: teach -> worked example when useful -> exercise/knowledge check -> review -> documentation/progress update.

Do not mark the item complete until I provide the required evidence of understanding. Do not silently advance to the next item.

Document every material step in the learning process, including commands, file/configuration changes, exercises, decisions, important outputs, and verification. If an error or issue occurs, document the symptom/error, context, meaningful failed attempts, root cause when known, resolution/workaround, verification, and learning takeaway in the learner issues-and-resolutions log. Do not erase troubleshooting history after a fix.

For code, always use exact repository paths and do not invent missing project structure. If required code context is missing after reading the live branch, ask for all missing information at once.

At the end, update the source-of-truth roadmap/progress/topic documentation, learning log, and issues-and-resolutions log affected by this session. Provide complete files as attachments when they exceed 20 lines.
```

## Repository Values

- `<repository-url>` — the exact GitHub repository containing this learner's current work. For a learner using a fork, this must be the fork URL, not the original upstream repository.
- `<learning-branch>` — the exact branch containing the learner's progress. `progress/<learner>` is recommended but not mandatory.
- `<upstream-url-or-none>` — normally `https://github.com/pvsmagbojos/ai-from-scratch-to-oci` for forks of this course; use `none` when no separate upstream repository applies.
